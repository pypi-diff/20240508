# Comparing `tmp/pyconcept-0.1.2.tar.gz` & `tmp/pyconcept-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconcept-0.1.2.tar", last modified: Thu Apr 18 12:04:06 2024, max compression
+gzip compressed data, was "pyconcept-0.1.3.tar", last modified: Tue May  7 23:18:13 2024, max compression
```

## Comparing `pyconcept-0.1.2.tar` & `pyconcept-0.1.3.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.680248 pyconcept-0.1.2/
--rw-rw-rw-   0        0        0      637 2024-04-18 12:02:25.000000 pyconcept-0.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0      955 2024-04-18 08:33:13.000000 pyconcept-0.1.2/CMakeLists.txt
--rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2024-04-18 12:04:06.680248 pyconcept-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.2/README.md
--rw-rw-rw-   0        0        0        5 2024-04-18 07:32:53.000000 pyconcept-0.1.2/VERSION
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.136412 pyconcept-0.1.2/ccl/
--rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.2/ccl/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.008403 pyconcept-0.1.2/ccl/cclCommons/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.008403 pyconcept-0.1.2/ccl/cclCommons/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.143409 pyconcept-0.1.2/ccl/cclCommons/include/ccl/
--rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclCommons/include/ccl/Strings.hpp
--rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclCommons/include/ccl/Substitutes.hpp
--rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclChange.hpp
--rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclMeta.hpp
--rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclTypes.hpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.010406 pyconcept-0.1.2/ccl/cclGraph/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.009405 pyconcept-0.1.2/ccl/cclGraph/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.144405 pyconcept-0.1.2/ccl/cclGraph/include/ccl/
--rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclGraph/include/ccl/Entity.hpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.144405 pyconcept-0.1.2/ccl/cclGraph/include/ccl/graph/
--rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclGraph/include/ccl/graph/CGraph.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.145404 pyconcept-0.1.2/ccl/cclGraph/src/
--rw-rw-rw-   0        0        0     9186 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclGraph/src/CGraph.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.013404 pyconcept-0.1.2/ccl/cclLang/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.011407 pyconcept-0.1.2/ccl/cclLang/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.011407 pyconcept-0.1.2/ccl/cclLang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.157406 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/
--rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
--rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/LexicalTerm.h
--rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/Literals.h
--rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/ManagedText.h
--rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/Morphology.h
--rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/Reference.h
--rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/RefsManager.h
--rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/TextEnvironment.h
--rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/TextProcessor.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.166411 pyconcept-0.1.2/ccl/cclLang/src/
--rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/LexicalTerm.cpp
--rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/ManagedText.cpp
--rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/Morphology.cpp
--rw-rw-rw-   0        0        0     7462 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/Reference.cpp
--rw-rw-rw-   0        0        0     6535 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/RefsManager.cpp
--rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/TextEnvironment.cpp
--rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/src/TextProcessor.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.167407 pyconcept-0.1.2/ccl/cclLang/unity/
--rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cclLang/unity/cclLang.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.169407 pyconcept-0.1.2/ccl/cmake/
--rw-rw-rw-   0        0        0     1541 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.048412 pyconcept-0.1.2/ccl/core/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.018409 pyconcept-0.1.2/ccl/core/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.177412 pyconcept-0.1.2/ccl/core/include/ccl/
--rw-rw-rw-   0        0        0     2124 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/Operation.hpp
--rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/Source.hpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.179406 pyconcept-0.1.2/ccl/core/include/ccl/api/
--rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/api/RSFormJA.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.182409 pyconcept-0.1.2/ccl/core/include/ccl/env/
--rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/env/SourceManager.hpp
--rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/env/cclEnvironment.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.190412 pyconcept-0.1.2/ccl/core/include/ccl/ops/
--rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/ops/EquationOptions.h
--rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/ops/RSAggregator.h
--rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/ops/RSEquationProcessor.h
--rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/ops/RSOperations.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.205910 pyconcept-0.1.2/ccl/core/include/ccl/oss/
--rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/OSSchema.h
--rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/OperationProcessor.hpp
--rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/Pict.hpp
--rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/RSSynthesProcessor.h
--rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/ossGraphFacet.h
--rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/ossGridFacet.h
--rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/ossOperationsFacet.h
--rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/oss/ossSourceFacet.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.232251 pyconcept-0.1.2/ccl/core/include/ccl/semantic/
--rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/ConceptRecord.h
--rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstFilters.hpp
--rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstList.h
--rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstType.hpp
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/IdentityManager.h
--rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/InterpretationStorage.h
--rw-rw-rw-   0        0        0     1069 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSConcept.h
--rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSCore.h
--rw-rw-rw-   0        0        0     3437 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSForm.h
--rw-rw-rw-   0        0        0     3019 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSModel.h
--rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/Schema.h
--rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/TextConcept.h
--rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/TextData.hpp
--rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/Thesaurus.h
--rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsCalculationFacet.h
--rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsModificationFacet.h
--rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsOperationFacet.h
--rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsValuesFacet.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.239249 pyconcept-0.1.2/ccl/core/include/ccl/tools/
--rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/tools/CstNameGenerator.h
--rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/tools/EntityGenerator.h
--rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/tools/EnumJSON.hpp
--rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/ccl/tools/JSON.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.241247 pyconcept-0.1.2/ccl/core/include/nlohmann/
--rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/include/nlohmann/json.hpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.243245 pyconcept-0.1.2/ccl/core/src/
--rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/JSON.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.245250 pyconcept-0.1.2/ccl/core/src/api/
--rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/api/RSFormJA.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.246251 pyconcept-0.1.2/ccl/core/src/env/
--rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/env/cclEnvironment.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.252248 pyconcept-0.1.2/ccl/core/src/ops/
--rw-rw-rw-   0        0        0     1764 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/ops/EquationOptions.cpp
--rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/ops/RSAggregator.cpp
--rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/ops/RSEquationProcessor.cpp
--rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/ops/RSOperations.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.278246 pyconcept-0.1.2/ccl/core/src/oss/
--rw-rw-rw-   0        0        0     7275 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/OSSchema.cpp
--rw-rw-rw-   0        0        0     2812 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/RSSynthesProcessor.cpp
--rw-rw-rw-   0        0        0     4326 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/ossGraphFacet.cpp
--rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/ossGridFacet.cpp
--rw-rw-rw-   0        0        0    11663 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/ossOperationsFacet.cpp
--rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/oss/ossSourceFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.040408 pyconcept-0.1.2/ccl/core/src/semantic/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.283250 pyconcept-0.1.2/ccl/core/src/semantic/rscore/
--rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rscore/ConceptRecord.cpp
--rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rscore/CstList.cpp
--rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rscore/IdentityManager.cpp
--rw-rw-rw-   0        0        0    10261 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rscore/RSCore.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.286253 pyconcept-0.1.2/ccl/core/src/semantic/rsform/
--rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsform/RSForm.cpp
--rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
--rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.290247 pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/
--rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
--rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/RSModel.cpp
--rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
--rw-rw-rw-   0        0        0     6819 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.292247 pyconcept-0.1.2/ccl/core/src/semantic/schema/
--rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/schema/RSConcept.cpp
--rw-rw-rw-   0        0        0    13468 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/schema/Schema.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.307253 pyconcept-0.1.2/ccl/core/src/semantic/thesaurus/
--rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/thesaurus/TextConcept.cpp
--rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.309248 pyconcept-0.1.2/ccl/core/src/tools/
--rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/tools/CstNameGenerator.cpp
--rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/src/tools/EntityGenerator.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.310248 pyconcept-0.1.2/ccl/core/unity/
--rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/core/unity/CCL.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.056409 pyconcept-0.1.2/ccl/rslang/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.318249 pyconcept-0.1.2/ccl/rslang/header/
--rw-rw-rw-   0        0        0     1362 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/ASTNormalizer.h
--rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/AsciiLexerImpl.hpp
--rw-rw-rw-   0        0        0     2359 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/GeneratorImplAST.h
--rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/MathLexerImpl.hpp
--rw-rw-rw-   0        0        0      958 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/NameCollector.h
--rw-rw-rw-   0        0        0    22132 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/RSParserImpl.h
--rw-rw-rw-   0        0        0     5452 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/header/SDImplementation.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.051408 pyconcept-0.1.2/ccl/rslang/import/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.053409 pyconcept-0.1.2/ccl/rslang/import/reflex/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.052414 pyconcept-0.1.2/ccl/rslang/import/reflex/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.425250 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/
--rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/abslexer.h
--rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/absmatcher.h
--rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/bits.h
--rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
--rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/convert.h
--rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/debug.h
--rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/error.h
--rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/flexlexer.h
--rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/input.h
--rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/linematcher.h
--rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/matcher.h
--rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/pattern.h
--rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
--rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/posix.h
--rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/ranges.h
--rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/setop.h
--rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/simd.h
--rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
--rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/timer.h
--rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/traits.h
--rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/unicode.h
--rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/utf8.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.508244 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/
--rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/convert.cpp
--rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/debug.cpp
--rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/error.cpp
--rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/input.cpp
--rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher.cpp
--rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
--rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
--rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/pattern.cpp
--rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/posix.cpp
--rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/simd_avx2.cpp
--rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
--rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/unicode.cpp
--rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/lib/utf8.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.514246 pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/
--rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/block_scripts.cpp
--rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/composer.cpp
--rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/language_scripts.cpp
--rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.054407 pyconcept-0.1.2/ccl/rslang/include/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.055413 pyconcept-0.1.2/ccl/rslang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.556251 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/
--rw-rw-rw-   0        0        0     3600 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
--rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/AsciiLexer.h
--rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Auditor.h
--rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/DataContext.hpp
--rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Error.hpp
--rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ErrorLogger.h
--rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Interpreter.h
--rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/LexerBase.hpp
--rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Literals.h
--rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/MathLexer.h
--rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Parser.h
--rw-rw-rw-   0        0        0     1526 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ParserState.hpp
--rw-rw-rw-   0        0        0     6805 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
--rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSExpr.h
--rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSGenerator.h
--rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSParser.h
--rw-rw-rw-   0        0        0     4689 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSToken.h
--rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/SDataCompact.h
--rw-rw-rw-   0        0        0     1953 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Structure.hpp
--rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/StructuredData.h
--rw-rw-rw-   0        0        0    12948 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/SyntaxTree.h
--rw-rw-rw-   0        0        0     5270 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/TypeAuditor.h
--rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/TypeContext.hpp
--rw-rw-rw-   0        0        0     3754 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Typification.h
--rw-rw-rw-   0        0        0     4297 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ValueAuditor.h
--rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ValueClass.hpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.607252 pyconcept-0.1.2/ccl/rslang/src/
--rw-rw-rw-   0        0        0    19985 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/ASTInterpreter.cpp
--rw-rw-rw-   0        0        0     5997 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/ASTNormalizer.cpp
--rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/AsciiLexer.cpp
--rw-rw-rw-   0        0        0     1238 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/Auditor.cpp
--rw-rw-rw-   0        0        0     1413 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/ErrorLogger.cpp
--rw-rw-rw-   0        0        0     7204 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/GeneratorImplAST.cpp
--rw-rw-rw-   0        0        0     1115 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/Interpreter.cpp
--rw-rw-rw-   0        0        0     2046 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/MathLexer.cpp
--rw-rw-rw-   0        0        0     3273 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/NameCollector.cpp
--rw-rw-rw-   0        0        0     3907 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/Parser.cpp
--rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/RSExpr.cpp
--rw-rw-rw-   0        0        0     8152 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/RSGenerator.cpp
--rw-rw-rw-   0        0        0     8280 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/RSParser.cpp
--rw-rw-rw-   0        0        0    60161 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/RSParserImpl.cpp
--rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/RSToken.cpp
--rw-rw-rw-   0        0        0     6882 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/SDImplementation.cpp
--rw-rw-rw-   0        0        0     7535 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/SDataCompact.cpp
--rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/StructuredData.cpp
--rw-rw-rw-   0        0        0     6353 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/SyntaxTree.cpp
--rw-rw-rw-   0        0        0    29818 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/TypeAuditor.cpp
--rw-rw-rw-   0        0        0     3844 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/Typification.cpp
--rw-rw-rw-   0        0        0     6264 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/src/ValueAuditor.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.612251 pyconcept-0.1.2/ccl/rslang/unity/
--rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/unity/RSlang.cpp
--rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/unity/RSlang2.cpp
--rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/unity/reflex_unity1.cpp
--rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.2/ccl/rslang/unity/reflex_unity2.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.613250 pyconcept-0.1.2/cmake/
--rw-rw-rw-   0        0        0     1490 2024-04-15 19:05:00.000000 pyconcept-0.1.2/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.2/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.615254 pyconcept-0.1.2/include/
--rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.2/include/pyconcept.h
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.679249 pyconcept-0.1.2/pyconcept.egg-info/
--rw-rw-rw-   0        0        0      953 2024-04-18 12:04:05.000000 pyconcept-0.1.2/pyconcept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8509 2024-04-18 12:04:05.000000 pyconcept-0.1.2/pyconcept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 12:04:05.000000 pyconcept-0.1.2/pyconcept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-18 12:04:05.000000 pyconcept-0.1.2/pyconcept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      860 2024-04-18 12:04:06.682256 pyconcept-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.621251 pyconcept-0.1.2/src/
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.2/src/pyconcept.cpp
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.624254 pyconcept-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.653247 pyconcept-0.1.2/tests/__pycache__/
--rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.2/tests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.2/tests/__pycache__/testBinding.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 12:04:06.678250 pyconcept-0.1.2/tests/data/
--rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.2/tests/data/Schema1.trs
--rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.2/tests/testBinding.py
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.603200 pyconcept-0.1.3/
+-rw-rw-rw-   0        0        0      637 2024-04-18 12:02:25.000000 pyconcept-0.1.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0      955 2024-04-19 23:54:16.000000 pyconcept-0.1.3/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      953 2024-05-07 23:18:13.603200 pyconcept-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.3/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-07 23:12:08.000000 pyconcept-0.1.3/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.288475 pyconcept-0.1.3/ccl/
+-rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.3/ccl/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.259911 pyconcept-0.1.3/ccl/cclCommons/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.259911 pyconcept-0.1.3/ccl/cclCommons/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.291475 pyconcept-0.1.3/ccl/cclCommons/include/ccl/
+-rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/Strings.hpp
+-rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/Substitutes.hpp
+-rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclChange.hpp
+-rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclMeta.hpp
+-rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclTypes.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.260912 pyconcept-0.1.3/ccl/cclGraph/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.260912 pyconcept-0.1.3/ccl/cclGraph/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.292476 pyconcept-0.1.3/ccl/cclGraph/include/ccl/
+-rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclGraph/include/ccl/Entity.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.293475 pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/
+-rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/CGraph.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.293475 pyconcept-0.1.3/ccl/cclGraph/src/
+-rw-rw-rw-   0        0        0     9187 2024-05-06 12:39:34.000000 pyconcept-0.1.3/ccl/cclGraph/src/CGraph.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.302476 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/
+-rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
+-rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/LexicalTerm.h
+-rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Literals.h
+-rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/ManagedText.h
+-rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Morphology.h
+-rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Reference.h
+-rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/RefsManager.h
+-rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextEnvironment.h
+-rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextProcessor.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.308475 pyconcept-0.1.3/ccl/cclLang/src/
+-rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/LexicalTerm.cpp
+-rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/ManagedText.cpp
+-rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/Morphology.cpp
+-rw-rw-rw-   0        0        0     7475 2024-05-06 12:47:43.000000 pyconcept-0.1.3/ccl/cclLang/src/Reference.cpp
+-rw-rw-rw-   0        0        0     6529 2024-05-06 12:48:14.000000 pyconcept-0.1.3/ccl/cclLang/src/RefsManager.cpp
+-rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/TextEnvironment.cpp
+-rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/TextProcessor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.309476 pyconcept-0.1.3/ccl/cclLang/unity/
+-rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/unity/cclLang.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.310475 pyconcept-0.1.3/ccl/cmake/
+-rw-rw-rw-   0        0        0     1541 2024-04-19 23:11:05.000000 pyconcept-0.1.3/ccl/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.267910 pyconcept-0.1.3/ccl/core/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.263912 pyconcept-0.1.3/ccl/core/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.312474 pyconcept-0.1.3/ccl/core/include/ccl/
+-rw-rw-rw-   0        0        0     2124 2024-05-06 15:23:11.000000 pyconcept-0.1.3/ccl/core/include/ccl/Operation.hpp
+-rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/Source.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.313477 pyconcept-0.1.3/ccl/core/include/ccl/api/
+-rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/api/RSFormJA.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.314475 pyconcept-0.1.3/ccl/core/include/ccl/env/
+-rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/env/SourceManager.hpp
+-rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/env/cclEnvironment.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.317476 pyconcept-0.1.3/ccl/core/include/ccl/ops/
+-rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/EquationOptions.h
+-rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSAggregator.h
+-rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSEquationProcessor.h
+-rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSOperations.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.323475 pyconcept-0.1.3/ccl/core/include/ccl/oss/
+-rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/OSSchema.h
+-rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/OperationProcessor.hpp
+-rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/Pict.hpp
+-rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/RSSynthesProcessor.h
+-rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGraphFacet.h
+-rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGridFacet.h
+-rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossOperationsFacet.h
+-rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossSourceFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.362672 pyconcept-0.1.3/ccl/core/include/ccl/semantic/
+-rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/ConceptRecord.h
+-rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstFilters.hpp
+-rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstList.h
+-rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstType.hpp
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/IdentityManager.h
+-rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/InterpretationStorage.h
+-rw-rw-rw-   0        0        0     1095 2024-05-06 14:59:52.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSConcept.h
+-rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSCore.h
+-rw-rw-rw-   0        0        0     3430 2024-05-06 15:04:15.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSForm.h
+-rw-rw-rw-   0        0        0     3012 2024-05-06 15:04:05.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSModel.h
+-rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/Schema.h
+-rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextConcept.h
+-rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextData.hpp
+-rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/Thesaurus.h
+-rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsCalculationFacet.h
+-rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsModificationFacet.h
+-rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsOperationFacet.h
+-rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsValuesFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.392677 pyconcept-0.1.3/ccl/core/include/ccl/tools/
+-rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/CstNameGenerator.h
+-rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/EntityGenerator.h
+-rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/EnumJSON.hpp
+-rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/JSON.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.393672 pyconcept-0.1.3/ccl/core/include/nlohmann/
+-rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/nlohmann/json.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.395672 pyconcept-0.1.3/ccl/core/src/
+-rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/JSON.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.403672 pyconcept-0.1.3/ccl/core/src/api/
+-rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/api/RSFormJA.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.405674 pyconcept-0.1.3/ccl/core/src/env/
+-rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/env/cclEnvironment.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.416672 pyconcept-0.1.3/ccl/core/src/ops/
+-rw-rw-rw-   0        0        0     1772 2024-05-06 14:58:07.000000 pyconcept-0.1.3/ccl/core/src/ops/EquationOptions.cpp
+-rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSAggregator.cpp
+-rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSEquationProcessor.cpp
+-rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSOperations.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.421673 pyconcept-0.1.3/ccl/core/src/oss/
+-rw-rw-rw-   0        0        0     7258 2024-05-06 15:10:47.000000 pyconcept-0.1.3/ccl/core/src/oss/OSSchema.cpp
+-rw-rw-rw-   0        0        0     2812 2024-05-06 15:23:33.000000 pyconcept-0.1.3/ccl/core/src/oss/RSSynthesProcessor.cpp
+-rw-rw-rw-   0        0        0     4305 2024-05-06 15:06:48.000000 pyconcept-0.1.3/ccl/core/src/oss/ossGraphFacet.cpp
+-rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/oss/ossGridFacet.cpp
+-rw-rw-rw-   0        0        0    11652 2024-05-06 15:05:23.000000 pyconcept-0.1.3/ccl/core/src/oss/ossOperationsFacet.cpp
+-rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/oss/ossSourceFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.267910 pyconcept-0.1.3/ccl/core/src/semantic/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.440267 pyconcept-0.1.3/ccl/core/src/semantic/rscore/
+-rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/ConceptRecord.cpp
+-rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/CstList.cpp
+-rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/IdentityManager.cpp
+-rw-rw-rw-   0        0        0    10403 2024-05-06 15:01:20.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/RSCore.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.442268 pyconcept-0.1.3/ccl/core/src/semantic/rsform/
+-rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/RSForm.cpp
+-rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
+-rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.445266 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/
+-rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
+-rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/RSModel.cpp
+-rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
+-rw-rw-rw-   0        0        0     6866 2024-05-06 13:08:18.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.446267 pyconcept-0.1.3/ccl/core/src/semantic/schema/
+-rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/schema/RSConcept.cpp
+-rw-rw-rw-   0        0        0    13468 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/schema/Schema.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.448269 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/
+-rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/TextConcept.cpp
+-rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.450267 pyconcept-0.1.3/ccl/core/src/tools/
+-rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/tools/CstNameGenerator.cpp
+-rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/tools/EntityGenerator.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.450267 pyconcept-0.1.3/ccl/core/unity/
+-rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/unity/CCL.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.272910 pyconcept-0.1.3/ccl/rslang/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.470832 pyconcept-0.1.3/ccl/rslang/header/
+-rw-rw-rw-   0        0        0     1363 2024-05-06 10:35:16.000000 pyconcept-0.1.3/ccl/rslang/header/ASTNormalizer.h
+-rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/AsciiLexerImpl.hpp
+-rw-rw-rw-   0        0        0     2359 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/GeneratorImplAST.h
+-rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/MathLexerImpl.hpp
+-rw-rw-rw-   0        0        0      958 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/NameCollector.h
+-rw-rw-rw-   0        0        0    32035 2024-05-05 13:23:08.000000 pyconcept-0.1.3/ccl/rslang/header/RSParserImpl.h
+-rw-rw-rw-   0        0        0     5446 2024-05-05 13:20:57.000000 pyconcept-0.1.3/ccl/rslang/header/SDImplementation.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.269911 pyconcept-0.1.3/ccl/rslang/import/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.270910 pyconcept-0.1.3/ccl/rslang/import/reflex/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.269911 pyconcept-0.1.3/ccl/rslang/import/reflex/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.488827 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/
+-rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/abslexer.h
+-rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/absmatcher.h
+-rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/bits.h
+-rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
+-rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/convert.h
+-rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/debug.h
+-rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/error.h
+-rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/flexlexer.h
+-rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/input.h
+-rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/linematcher.h
+-rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/matcher.h
+-rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pattern.h
+-rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
+-rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/posix.h
+-rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/ranges.h
+-rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/setop.h
+-rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/simd.h
+-rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
+-rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/timer.h
+-rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/traits.h
+-rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/unicode.h
+-rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/utf8.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.515829 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/
+-rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/convert.cpp
+-rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/debug.cpp
+-rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/error.cpp
+-rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/input.cpp
+-rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher.cpp
+-rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
+-rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
+-rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/pattern.cpp
+-rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/posix.cpp
+-rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx2.cpp
+-rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
+-rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/unicode.cpp
+-rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/utf8.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.519952 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/
+-rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/block_scripts.cpp
+-rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/composer.cpp
+-rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/language_scripts.cpp
+-rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.271913 pyconcept-0.1.3/ccl/rslang/include/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.271913 pyconcept-0.1.3/ccl/rslang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.539955 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/
+-rw-rw-rw-   0        0        0     3600 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
+-rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/AsciiLexer.h
+-rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Auditor.h
+-rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/DataContext.hpp
+-rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Error.hpp
+-rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ErrorLogger.h
+-rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Interpreter.h
+-rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/LexerBase.hpp
+-rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Literals.h
+-rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/MathLexer.h
+-rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Parser.h
+-rw-rw-rw-   0        0        0     1667 2024-05-05 09:01:01.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ParserState.hpp
+-rw-rw-rw-   0        0        0     6503 2024-05-07 22:51:03.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
+-rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSExpr.h
+-rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSGenerator.h
+-rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSParser.h
+-rw-rw-rw-   0        0        0     4722 2024-05-06 14:48:08.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSToken.h
+-rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SDataCompact.h
+-rw-rw-rw-   0        0        0     1953 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Structure.hpp
+-rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/StructuredData.h
+-rw-rw-rw-   0        0        0    12948 2024-05-07 16:08:23.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SyntaxTree.h
+-rw-rw-rw-   0        0        0     5373 2024-05-07 15:46:38.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeAuditor.h
+-rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeContext.hpp
+-rw-rw-rw-   0        0        0     3875 2024-05-07 15:17:48.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Typification.h
+-rw-rw-rw-   0        0        0     4297 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueAuditor.h
+-rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueClass.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.557952 pyconcept-0.1.3/ccl/rslang/src/
+-rw-rw-rw-   0        0        0    19744 2024-05-06 10:32:45.000000 pyconcept-0.1.3/ccl/rslang/src/ASTInterpreter.cpp
+-rw-rw-rw-   0        0        0     5991 2024-05-06 14:51:18.000000 pyconcept-0.1.3/ccl/rslang/src/ASTNormalizer.cpp
+-rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/AsciiLexer.cpp
+-rw-rw-rw-   0        0        0     1222 2024-05-06 14:50:47.000000 pyconcept-0.1.3/ccl/rslang/src/Auditor.cpp
+-rw-rw-rw-   0        0        0     1375 2024-05-06 10:40:35.000000 pyconcept-0.1.3/ccl/rslang/src/ErrorLogger.cpp
+-rw-rw-rw-   0        0        0     7204 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/GeneratorImplAST.cpp
+-rw-rw-rw-   0        0        0     1122 2024-05-06 13:10:50.000000 pyconcept-0.1.3/ccl/rslang/src/Interpreter.cpp
+-rw-rw-rw-   0        0        0     2067 2024-05-07 15:44:11.000000 pyconcept-0.1.3/ccl/rslang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/MathLexer.cpp
+-rw-rw-rw-   0        0        0     3266 2024-05-06 10:24:04.000000 pyconcept-0.1.3/ccl/rslang/src/NameCollector.cpp
+-rw-rw-rw-   0        0        0     3907 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/Parser.cpp
+-rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/RSExpr.cpp
+-rw-rw-rw-   0        0        0     7626 2024-05-06 14:51:49.000000 pyconcept-0.1.3/ccl/rslang/src/RSGenerator.cpp
+-rw-rw-rw-   0        0        0     8365 2024-05-05 12:24:50.000000 pyconcept-0.1.3/ccl/rslang/src/RSParser.cpp
+-rw-rw-rw-   0        0        0    64296 2024-05-07 08:26:17.000000 pyconcept-0.1.3/ccl/rslang/src/RSParserImpl.cpp
+-rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/RSToken.cpp
+-rw-rw-rw-   0        0        0     6872 2024-05-05 13:20:57.000000 pyconcept-0.1.3/ccl/rslang/src/SDImplementation.cpp
+-rw-rw-rw-   0        0        0     7639 2024-05-06 13:10:17.000000 pyconcept-0.1.3/ccl/rslang/src/SDataCompact.cpp
+-rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/StructuredData.cpp
+-rw-rw-rw-   0        0        0     6348 2024-05-06 14:51:57.000000 pyconcept-0.1.3/ccl/rslang/src/SyntaxTree.cpp
+-rw-rw-rw-   0        0        0    31033 2024-05-07 22:48:22.000000 pyconcept-0.1.3/ccl/rslang/src/TypeAuditor.cpp
+-rw-rw-rw-   0        0        0     4000 2024-05-07 15:55:27.000000 pyconcept-0.1.3/ccl/rslang/src/Typification.cpp
+-rw-rw-rw-   0        0        0     6172 2024-05-06 12:22:18.000000 pyconcept-0.1.3/ccl/rslang/src/ValueAuditor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.560952 pyconcept-0.1.3/ccl/rslang/unity/
+-rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/RSlang.cpp
+-rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/RSlang2.cpp
+-rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/reflex_unity1.cpp
+-rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/reflex_unity2.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.573627 pyconcept-0.1.3/cmake/
+-rw-rw-rw-   0        0        0     1490 2024-04-19 23:11:03.000000 pyconcept-0.1.3/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.3/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.574629 pyconcept-0.1.3/include/
+-rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.3/include/pyconcept.h
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.602202 pyconcept-0.1.3/pyconcept.egg-info/
+-rw-rw-rw-   0        0        0      953 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8509 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      860 2024-05-07 23:18:13.604200 pyconcept-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.577628 pyconcept-0.1.3/src/
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.3/src/pyconcept.cpp
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.579628 pyconcept-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.597202 pyconcept-0.1.3/tests/__pycache__/
+-rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.3/tests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.3/tests/__pycache__/testBinding.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.601205 pyconcept-0.1.3/tests/data/
+-rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.3/tests/data/Schema1.trs
+-rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.3/tests/testBinding.py
```

### Comparing `pyconcept-0.1.2/CHANGELOG.md` & `pyconcept-0.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/CMakeLists.txt` & `pyconcept-0.1.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/LICENSE` & `pyconcept-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/PKG-INFO` & `pyconcept-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.2
+Version: 0.1.3
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.2/ccl/CMakeLists.txt` & `pyconcept-0.1.3/ccl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclCommons/include/ccl/Strings.hpp` & `pyconcept-0.1.3/ccl/cclCommons/include/ccl/Strings.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclCommons/include/ccl/Substitutes.hpp` & `pyconcept-0.1.3/ccl/cclCommons/include/ccl/Substitutes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclChange.hpp` & `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclChange.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclMeta.hpp` & `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclMeta.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclCommons/include/ccl/cclTypes.hpp` & `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclTypes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclGraph/include/ccl/Entity.hpp` & `pyconcept-0.1.3/ccl/cclGraph/include/ccl/Entity.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclGraph/include/ccl/graph/CGraph.h` & `pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/CGraph.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclGraph/src/CGraph.cpp` & `pyconcept-0.1.3/ccl/cclGraph/src/CGraph.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         if (!marked[child]) {
           toVisit.push_back(child);
           marked[child] = true;
         }
       }
     }
     if (size(component) != 1 || HasEdge(index, index)) {
-      result.push_back({});
+      result.emplace_back();
       result.back().reserve(size(component));
       for (const auto item : component) {
         result.back().emplace(graph[item].uid);
       }
     }
   }
   return result;
```

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/LexicalTerm.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/LexicalTerm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/ManagedText.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/ManagedText.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/Morphology.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Morphology.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/Reference.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Reference.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/RefsManager.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/RefsManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/TextEnvironment.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/include/ccl/lang/TextProcessor.h` & `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/LexicalTerm.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/LexicalTerm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/ManagedText.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/ManagedText.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/Morphology.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/Morphology.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/Reference.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/Reference.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     return Morphology{ tags };
   }
 }
 
 [[nodiscard]] UTF8Iterator ReferenceStart(const std::string_view refStr, const StrPos start) noexcept {
   for (auto iter = UTF8Iterator(refStr, start); iter != UTF8End(refStr); ++iter) {
     if (*iter == '@') {
-      if (++iter == UTF8End(refStr) || *iter == '{') {
+      ++iter;
+      if (iter == UTF8End(refStr) || *iter == '{') {
         return iter;
       }
     }
   }
   return UTF8End(refStr);
 }
```

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/RefsManager.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/RefsManager.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 std::string RefsManager::OutputRefs(const std::string& normStr, const StrRange subRange) const {
   std::string result{};
   auto curPos = subRange.start;
   auto finish = subRange.finish;
   for (const auto& ref : refs) {
     const auto intersection = subRange.Intersect(ref.position);
-    if (!intersection.has_value() || intersection->length() == 0) {
+    if (!intersection.has_value() || intersection->empty()) {
       if (subRange.IsBefore(ref.position)) {
         break;
       }
     } else if (intersection->length() * 2 < ref.position.length()) {
       if (ref.position.finish >= finish) {
         finish = std::min(finish, ref.position.start);
         break;
```

### Comparing `pyconcept-0.1.2/ccl/cclLang/src/TextProcessor.cpp` & `pyconcept-0.1.3/ccl/cclLang/src/TextProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/cmake/CXXTargets.cmake` & `pyconcept-0.1.3/ccl/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/Operation.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/Operation.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/Source.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/Source.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/api/RSFormJA.h` & `pyconcept-0.1.3/ccl/core/include/ccl/api/RSFormJA.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/env/SourceManager.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/env/SourceManager.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/env/cclEnvironment.h` & `pyconcept-0.1.3/ccl/core/include/ccl/env/cclEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/ops/EquationOptions.h` & `pyconcept-0.1.3/ccl/core/include/ccl/ops/EquationOptions.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/ops/RSAggregator.h` & `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSAggregator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/ops/RSEquationProcessor.h` & `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSEquationProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/ops/RSOperations.h` & `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSOperations.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/OSSchema.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/OSSchema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/OperationProcessor.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/OperationProcessor.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/Pict.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/Pict.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/RSSynthesProcessor.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/RSSynthesProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/ossGraphFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGraphFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/ossGridFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGridFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/ossOperationsFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossOperationsFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/oss/ossSourceFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossSourceFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/ConceptRecord.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/ConceptRecord.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstFilters.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstFilters.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstList.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstList.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/CstType.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstType.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/IdentityManager.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/IdentityManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/InterpretationStorage.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/InterpretationStorage.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSCore.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSCore.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSForm.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSForm.h`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   [[nodiscard]] RSCore& LoadCore() noexcept { return core; }
   
   // Note: hashes ignore ordering
   [[nodiscard]] change::Hash CoreHash() const;
   [[nodiscard]] change::Hash FullHash() const;
 
 private:
-  [[nodiscard]] inline bool NotifyAndReturn(const bool result) {
+  [[nodiscard]] bool NotifyAndReturn(const bool result) {
     if (result) {
       NotifyModification();
     }
     return result;
   }
   [[nodiscard]] bool EraseInternal(EntityUID target);
   EntityTranslation DeleteDuplicatesInternal();
```

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/RSModel.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSModel.h`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
   // Note: use only for creating from empty state
   EntityUID Load(ConceptRecord&& cst);
   [[nodiscard]] RSCore& LoadCore() noexcept { return core; }
   void FinalizeLoadingCore();
   void UpdateState();
 
 private:
-  [[nodiscard]] inline bool NotifyAndReturn(const bool result) {
+  [[nodiscard]] bool NotifyAndReturn(const bool result) {
     if (result) {
       NotifyModification();
     }
     return result;
   }
   void AfterInsert(EntityUID target);
   void ResetDependants(EntityUID target);
```

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/Schema.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/Schema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/TextConcept.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/TextData.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextData.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/Thesaurus.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/Thesaurus.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsCalculationFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsCalculationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsModificationFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsModificationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsOperationFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsOperationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/semantic/rsValuesFacet.h` & `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsValuesFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/tools/CstNameGenerator.h` & `pyconcept-0.1.3/ccl/core/include/ccl/tools/CstNameGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/tools/EntityGenerator.h` & `pyconcept-0.1.3/ccl/core/include/ccl/tools/EntityGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/tools/EnumJSON.hpp` & `pyconcept-0.1.3/ccl/core/include/ccl/tools/EnumJSON.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/ccl/tools/JSON.h` & `pyconcept-0.1.3/ccl/core/include/ccl/tools/JSON.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/include/nlohmann/json.hpp` & `pyconcept-0.1.3/ccl/core/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/JSON.cpp` & `pyconcept-0.1.3/ccl/core/src/JSON.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/api/RSFormJA.cpp` & `pyconcept-0.1.3/ccl/core/src/api/RSFormJA.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/env/cclEnvironment.cpp` & `pyconcept-0.1.3/ccl/core/src/env/cclEnvironment.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/ops/EquationOptions.cpp` & `pyconcept-0.1.3/ccl/core/src/ops/EquationOptions.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -13,25 +13,28 @@
     return translation == other->translation && properties == other->properties;
   }
 }
 
 bool EquationOptions::SwapKeyVal(const EntityUID key) {
   if (!ContainsKey(key)) {
     return false;
-  } else if (const auto val = translation(key); ContainsKey(translation(key))) {
+  }
+  const auto newKey = translation(key);
+  if (ContainsKey(newKey)) {
     return false;
-  } else {
-    Equation props = properties[key];
-    if (props.mode != Equation::Mode::createNew) {
-      props.mode = props.mode == Equation::Mode::keepHier ? Equation::Mode::keepDel : Equation::Mode::keepHier;
-    }
-    Erase(key);
-    Insert(val, key, props);
-    return true;
   }
+
+  Equation props = properties[key];
+  if (props.mode != Equation::Mode::createNew) {
+    props.mode = props.mode == Equation::Mode::keepHier ? Equation::Mode::keepDel : Equation::Mode::keepHier;
+  }
+  Erase(key);
+  const auto newValue = key;
+  Insert(newKey, newValue, props);
+  return true;
 }
 
 const Equation& EquationOptions::PropsFor(const EntityUID key) const {
   return properties.at(key);
 }
 
 bool EquationOptions::ContainsValue(const EntityUID value) const {
```

### Comparing `pyconcept-0.1.2/ccl/core/src/ops/RSAggregator.cpp` & `pyconcept-0.1.3/ccl/core/src/ops/RSAggregator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/ops/RSEquationProcessor.cpp` & `pyconcept-0.1.3/ccl/core/src/ops/RSEquationProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/ops/RSOperations.cpp` & `pyconcept-0.1.3/ccl/core/src/ops/RSOperations.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/OSSchema.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/OSSchema.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,20 @@
 void OSSchema::SetPictLink(const PictID target, const MediaLink& lnk) {
   if (auto* pict = Access(target); pict != nullptr && pict->lnk != lnk) {
     pict->lnk = lnk;
     NotifyModification();
   }
 }
 
-const Pict& OSSchema::LoadPict(Pict&& pict, GridPosition pos, const src::Handle& handle, 
-                           std::unique_ptr<OperationHandle> params) {
+// NOLINTNEXTLINE(cppcoreguidelines-rvalue-reference-param-not-moved)
+const Pict& OSSchema::LoadPict(
+  Pict&& pict, GridPosition pos,
+  const src::Handle& handle, 
+  std::unique_ptr<OperationHandle> params
+) {
   if (Grid()(pos).has_value()) {
     pos = Grid().ClosestFreePos(pos);
   }
   if (idGen.IsTaken(pict.uid)) {
     pict.uid = idGen.NewUID();
   }
   const auto pid = pict.uid;
@@ -145,18 +149,20 @@
   } else if (!Contains(operand1) || !Contains(operand2)) {
     return nullptr;
   } else {
     const auto newID = idGen.NewUID();
     graph->AddItem(newID, { operand1, operand2 });
 
     const auto newPos = Grid().ChildPosFor(operand1, operand2);
-    InsertInternal(Pict{ newID },
-                   newPos,
-                   src::Handle{ src::SrcType::rsDoc },
-                   std::make_unique<OperationHandle>());
+    InsertInternal(
+      Pict{ newID },
+      newPos,
+      src::Handle{ src::SrcType::rsDoc },
+      std::make_unique<OperationHandle>()
+    );
 
     NotifyModification();
     return &storage.at(newID);
   }
 }
 
 PictPtr OSSchema::InsertBase() {
@@ -164,17 +170,20 @@
   const auto newID = idGen.NewUID();
   InsertInternal(Pict{ newID }, newPos, src::Handle{ src::SrcType::rsDoc }, nullptr);
 
   NotifyModification();
   return &storage.at(newID);
 }
 
-void OSSchema::InsertInternal(const Pict& pict, GridPosition pos,
-                              const src::Handle& srcHandle,
-                              std::unique_ptr<OperationHandle> opHandle) {
+void OSSchema::InsertInternal(
+  const Pict& pict,
+  GridPosition pos,
+  const src::Handle& srcHandle,
+  std::unique_ptr<OperationHandle> opHandle
+) {
   const auto pid = pict.uid;
 
   idGen.AddUID(pid);
   storage.emplace(pid, pict);
   Grid().SetPosFor(pid, pos);
   Src().sources.emplace(pid, srcHandle);
   if (opHandle != nullptr) {
```

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/RSSynthesProcessor.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/RSSynthesProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/ossGraphFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/ossGraphFacet.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     }
     ++index;
   }
   return std::nullopt;
 }
 
 size_t ossGraphFacet::InsertKeyValue(const PictID item) {
-  graph.emplace_back(std::vector<size_t>{});
+  graph.emplace_back();
   items.emplace_back(item);
   return size(items) - 1U;
 }
 
 size_t ossGraphFacet::Item2ID(const PictID item) {
   if (const auto index = FindItemIndex(item); index.has_value()) {
     return index.value();
```

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/ossGridFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/ossGridFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/ossOperationsFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/ossOperationsFacet.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -212,17 +212,20 @@
   const auto& pict = *core.Access(pid);
   ossSourceFacet::WriteAttribute({ src::DataStream::Attribute::title, pict.title }, data);
   ossSourceFacet::WriteAttribute({ src::DataStream::Attribute::alias, pict.alias }, data);
   ossSourceFacet::WriteAttribute({ src::DataStream::Attribute::comment, pict.comment }, data);
   return opResult;
 }
 
-bool ossOperationsFacet::SaveOperationResult(const PictID pid, 
-                                             const EntityTranslation& old2New, 
-                                             ops::Result&& opResult) {
+// NOLINTNEXTLINE(cppcoreguidelines-rvalue-reference-param-not-moved)
+bool ossOperationsFacet::SaveOperationResult(
+  const PictID pid,
+  const EntityTranslation& old2New,
+  ops::Result&& opResult
+) {
   auto& opHandle = operations.at(pid);
   assert(opHandle != nullptr);
   const auto guard = core.DndGuard();
   if (!core.Src().InputData(pid, std::move(opResult.value))) {
     opHandle->broken = true;
     return false;
   } else {
```

### Comparing `pyconcept-0.1.2/ccl/core/src/oss/ossSourceFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/oss/ossSourceFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rscore/ConceptRecord.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rscore/ConceptRecord.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rscore/CstList.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rscore/CstList.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rscore/IdentityManager.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rscore/IdentityManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rscore/RSCore.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rscore/RSCore.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
   const auto newID = identifiers.GenerateNewID(type);
   schema.Emplace(newID.uid, newID.alias, type, definition);
   thesaurus.Emplace(newID.uid, newID.alias);
   cstList.Insert(newID.uid);
   return newID.uid;
 }
 
+// NOLINTNEXTLINE(cppcoreguidelines-rvalue-reference-param-not-moved)
 EntityUID RSCore::Insert(ConceptRecord&& cst) {
   RSConcept newRS{cst.uid, cst.alias, cst.type, std::move(cst.rs), std::move(cst.convention) };
   TextConcept newText{cst.uid, cst.alias, std::move(cst.term), std::move(cst.definition) };
   const auto newID = identifiers.RegisterID(newRS.uid, newRS.alias, newRS.type);
   newRS.uid = newID.uid;
   newRS.alias = newID.alias;
   newText.uid = newID.uid;
@@ -209,14 +210,15 @@
       Translate(uid, translator);
     }
   }
   UpdateState();
   return result;
 }
 
+// NOLINTNEXTLINE(cppcoreguidelines-rvalue-reference-param-not-moved)
 EntityUID RSCore::Load(ConceptRecord&& cst) {
   RSConcept newRS{ cst.uid, cst.alias, cst.type, std::move(cst.rs), std::move(cst.convention) };
   TextConcept newText{ cst.uid, cst.alias, std::move(cst.term), std::move(cst.definition) };
   const auto newID = identifiers.RegisterID(newRS.uid, newRS.alias, newRS.type);
   newRS.uid = newID.uid;
   newRS.alias = newID.alias;
   newText.uid = newID.uid;
```

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsform/RSForm.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsform/RSForm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsform/rsModificationFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsModificationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsform/rsOperationFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsOperationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/RSModel.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/RSModel.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
 void rsValuesFacet::PruneStructure(const EntityUID target) {
   const auto oldData = SDataFor(target);
   if (!oldData.has_value()) {
     return;
   } 
   const auto& typeValue = core.GetParse(target).exprType;
   assert(typeValue.has_value());
-  const auto& type = std::get<rslang::Typification>(typeValue.value()); // NOLINT(bugprone-exception-escape)
+  // NOLINTNEXTLINE(bugprone-exception-escape, bugprone-unchecked-optional-access)
+  const auto& type = std::get<rslang::Typification>(typeValue.value());
   if (!oldData->IsCollection()) {
     if (!CheckBasicElements(oldData.value(), type)) {
       storage->Erase(target);
     }
   } else {
     auto newData = object::Factory::EmptySet();
     for (const auto& element : oldData->B()) {
```

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/schema/RSConcept.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/schema/RSConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/schema/Schema.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/schema/Schema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/thesaurus/TextConcept.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/TextConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/semantic/thesaurus/Thesaurus.cpp` & `pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/Thesaurus.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/tools/CstNameGenerator.cpp` & `pyconcept-0.1.3/ccl/core/src/tools/CstNameGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/src/tools/EntityGenerator.cpp` & `pyconcept-0.1.3/ccl/core/src/tools/EntityGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/core/unity/CCL.cpp` & `pyconcept-0.1.3/ccl/core/unity/CCL.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/header/ASTNormalizer.h` & `pyconcept-0.1.3/ccl/rslang/header/ASTNormalizer.h`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 public:
   void Normalize(SyntaxTree::Node& root);
 
 private:
   void Quantifier(SyntaxTree::Node& quant);
   static void EnumDeclaration(SyntaxTree::Node& quant);
-  void TupleDeclaration(SyntaxTree::Node& declaration, SyntaxTree::Node& predicat);
+  void TupleDeclaration(SyntaxTree::Node& declaration, SyntaxTree::Node& predicate);
   void TupleDeclaration(SyntaxTree::Node& target);
 
   [[nodiscard]] std::string CreateTupleName(const SyntaxTree::Node& root);
   void SubstituteTupleVariables(SyntaxTree::Node& target, const std::string& newName);
 
   void Function(SyntaxTree::Node& func);
   [[nodiscard]] static std::vector<std::string> ArgNames(const SyntaxTree::Node& declaration);
```

### Comparing `pyconcept-0.1.2/ccl/rslang/header/AsciiLexerImpl.hpp` & `pyconcept-0.1.3/ccl/rslang/header/AsciiLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/header/GeneratorImplAST.h` & `pyconcept-0.1.3/ccl/rslang/header/GeneratorImplAST.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/header/MathLexerImpl.hpp` & `pyconcept-0.1.3/ccl/rslang/header/MathLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/header/NameCollector.h` & `pyconcept-0.1.3/ccl/rslang/header/NameCollector.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/header/SDImplementation.h` & `pyconcept-0.1.3/ccl/rslang/header/SDImplementation.h`

 * *Files 4% similar despite different names*

```diff
@@ -150,15 +150,15 @@
   class Iterator {
     const SDDecartian* decartian{ nullptr };
     std::vector<SDIterator> componentIters{};
     bool isCompleted{ true };
     uint32_t counter{ 0 };
 
   public:
-    explicit Iterator(const SDDecartian& decartaian, bool isCompleted = false);
+    explicit Iterator(const SDDecartian& base, bool isCompleted = false);
 
   public:
     using iterator_category = std::forward_iterator_tag;
     using value_type = StructuredData;
     using difference_type = std::ptrdiff_t;
     using pointer = const StructuredData*;
     using reference = const StructuredData&;
```

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/abslexer.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/abslexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/absmatcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/absmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/bits.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/bits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/boostmatcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/boostmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/convert.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/convert.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/debug.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/debug.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/error.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/error.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/flexlexer.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/flexlexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/input.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/input.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/linematcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/linematcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/matcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/pattern.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pattern.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/posix.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/posix.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/ranges.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/ranges.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/setop.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/setop.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/simd.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/simd.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/stdmatcher.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/stdmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/timer.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/timer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/traits.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/traits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/unicode.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/unicode.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/include/reflex/utf8.h` & `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/utf8.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/convert.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/convert.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/debug.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/debug.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/error.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/error.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/input.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/input.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher_avx2.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/pattern.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/pattern.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/posix.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/posix.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/simd_avx2.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/unicode.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/unicode.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/lib/utf8.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/utf8.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/block_scripts.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/block_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/composer.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/composer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/language_scripts.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/language_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/import/reflex/unicode/letter_scripts.cpp` & `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/letter_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ASTInterpreter.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ASTInterpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/AsciiLexer.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/AsciiLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Auditor.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Auditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Error.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Error.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ErrorLogger.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ErrorLogger.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Interpreter.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Interpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/LexerBase.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/LexerBase.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/MathLexer.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/MathLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Parser.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Parser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ParserState.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ParserState.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #pragma once
 
 #include "ccl/rslang/SyntaxTree.h"
 #include "ccl/rslang/Error.hpp"
 #include "ccl/rslang/RSErrorCodes.hpp"
 
 #include <functional>
+#include <optional>
 
 namespace ccl::rslang::detail {
 
 struct Node;
 using RawNode = std::shared_ptr<Node>;
 
 struct Node {
   Token token{};
   std::vector<RawNode> children{};
 
 public:
   explicit Node(Token token) noexcept
     : token{ std::move(token) } {}
+  explicit Node(TokenID id, StrRange pos, TokenData val = {}) noexcept 
+    : Node(Token(id, pos, std::move(val))) {}
 };
 
 struct ParserState {
   meta::UniqueCPPtr<SyntaxTree> parsedTree{ nullptr };
   int32_t currentPosition{ 0 };
   int32_t countCriticalErrors{ 0 };
```

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 enum class LexerEID : uint32_t {
   unknownSymbol = 0x8203, // Неизвестный символ
 };
 
 //! Syntactic errors enumeration
 enum class ParseEID : uint32_t {
   syntax = 0x8400, // Неизвестная синтаксическая ошибка
-  missingParanthesis = 0x8406,      // Пропущена скобка ')'
+  missingParenthesis = 0x8406,      // Пропущена скобка ')'
   missingCurlyBrace = 0x8407,       // Пропущена скобка '}'
   invalidQuantifier = 0x8408,       // Некорректная кванторная декларация
   expectedDeclaration = 0x8414,     // Ожидалось объявление аргументов
   expectedLocal = 0x8415,           // Ожидалось имя локальной переменной
 };
 
 //! Semantic errors enumeration
@@ -38,26 +38,24 @@
   invalidDebool = 0x8809,            // Дебулеан берется от немножества
   globalFuncMissing = 0x880A,        // Неизвестное имя функции
   globalFuncWithoutArgs = 0x880B,    // Некорректное использование имени функции без аргументов
   invalidReduce = 0x8810,            // Red можно брать только от двойного булеана
   invalidProjectionTuple = 0x8811,  // Не определена проекция
   invalidProjectionSet = 0x8812,    // Большая проекция определена только для множеств!
   invalidEnumeration = 0x8813,      // Типизация аргументов перечисления не совпадает
-  ivalidBinding = 0x8814,           // Количество переменных в кортеже не соответствует размерности декартова произведения
+  invalidBinding = 0x8814,           // Количество переменных в кортеже не соответствует размерности декартова произведения
   localOutOfScope = 0x8815,         // Использование имени вне области видимости
-  invalidElementPredicat = 0x8816,  // Несоответствие типов для проверки принадлежности
-  invalidArgsArtity = 0x8818,       // Некорректное количество аргументов терм-функции
+  invalidElementPredicate = 0x8816,  // Несоответствие типов для проверки принадлежности
+  invalidArgsArity = 0x8818,       // Некорректное количество аргументов терм-функции
   invalidArgumentType = 0x8819,     // Типизация аргумента не совпадает с объявленной
-  invalidEqualsEmpty = 0x881A,      // Сравнение с пустым множеством не множества
   globalStructure = 0x881C,         // Родовая структура должна быть ступенью
 
   // TODO: следующий идентификатор сейчас не используется. Нужно подобрать место для проверки
   globalExpectedFunction = 0x881F,  // Ожидалось выражение объявления функции
 
-  emptySetUsage = 0x8820,           // Некорректное использование пустого множества как типизированного выражения
   radicalUsage = 0x8821,            // Радикалы запрещены вне деклараций терм-функций
   invalidFilterArgumentType = 0x8822, // Типизация аргумента фильтра не корректна
   invalidFilterArity = 0x8823,      // Количество параметров фильра не соответствует количеству индексов
   arithmeticNotSupported = 0x8824,  // Для данного типа не поддерживается арифметика
   typesNotCompatible = 0x8825,      // Типы не совместимы в данном контексте
   orderingNotSupported = 0x8826,    // Для данного типа не поддерживается порядок элементов
```

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSExpr.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSExpr.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSGenerator.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSParser.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSParser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/RSToken.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSToken.h`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 enum class Syntax : uint8_t {
   UNDEF,
   MATH,      // Math syntax using UTF8 symbols
   ASCII      // Pure ASCII encoded syntax
 };
 
 //! RS language token types enumeration
-enum class TokenID : uint32_t {
+enum class TokenID : uint32_t { // NOLINT(performance-enum-size)
   // Global, local IDs and literals
   ID_LOCAL = 258,
   ID_GLOBAL,
   ID_FUNCTION,
   ID_PREDICATE,
   ID_RADICAL,
   LIT_INTEGER,
```

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/SDataCompact.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SDataCompact.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Structure.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Structure.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/StructuredData.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/StructuredData.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/SyntaxTree.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SyntaxTree.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/TypeAuditor.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeAuditor.h`

 * *Files 4% similar despite different names*

```diff
@@ -50,40 +50,42 @@
 
   ExpressionType currentType{};
 
   std::vector<LocalData> localVars{};
   std::vector<size_t> functionArgsID{};
   FunctionArguments functionArgs{};
 
+  bool isTypification{ false };
   types::GuardableBool isArgDeclaration{ false };
   types::GuardableBool isLocalDeclaration{ false };
   types::GuardableBool isFuncDeclaration{ false };
 
 public:
   explicit TypeAuditor(const TypeContext& context) noexcept
     : env{ context } {}
   explicit TypeAuditor(const TypeContext& context, ErrorReporter reporter) noexcept
     : env{ context }, reporter{ std::move(reporter) } {}
 
 public:
   [[nodiscard]] bool CheckType(const SyntaxTree& tree);
   [[nodiscard]] const FunctionArguments& GetDeclarationArgs() const noexcept { return functionArgs; }
   [[nodiscard]] const ExpressionType& GetType() const noexcept;
+  void SetExepectTypification(const bool value = true) noexcept;
 
 protected:
   bool ViGlobalDefinition(Cursor iter);
 
   bool ViFunctionDefinition(Cursor iter);
   bool ViFunctionCall(Cursor iter);
 
   bool ViGlobal(Cursor iter);
   bool ViLocal(Cursor iter);
   bool ViInteger(Cursor /*iter*/) { return VisitAndReturn(Typification::Integer()); }
   bool ViIntegerSet(Cursor /*iter*/) { return VisitAndReturn(Typification::Integer().Bool()); }
-  bool ViEmptySet(Cursor iter);
+  bool ViEmptySet(Cursor /*iter*/);
 
   bool ViLocalBind(Cursor iter);
   bool ViLocalEnum(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
   bool ViArgumentsEnum(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
   bool ViArgument(Cursor iter);
 
   bool ViArithmetic(Cursor iter);
```

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/TypeContext.hpp` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/Typification.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Typification.h`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,29 @@
 };
 
 //! Typification
 class Typification : public Structured<EchelonBase, EchelonTuple, EchelonBool> {
 public:
   static constexpr Index PR_START = 1;
   static constexpr std::string_view integerTypeName = "Z";
+  static constexpr std::string_view anyTypificationName = "R0";
 
 private:
   using Structured::Structured;
 
 public:
   explicit Typification(std::string baseTag) noexcept
     : Structured(EchelonBase(std::move(baseTag))) {}
 
   explicit Typification(std::vector<Typification> factors) noexcept
     : Structured(EchelonTuple(std::move(factors))) {}
 
   [[nodiscard]] static Typification Tuple(std::vector<Typification> factors);
   [[nodiscard]] static const Typification& Integer();
+  [[nodiscard]] static const Typification& EmptySet();
 
 public:
   using Substitutes = std::unordered_map<std::string, Typification>;
 
   Typification& ApplyBool();
   [[nodiscard]] Typification Bool() const;
```

### Comparing `pyconcept-0.1.2/ccl/rslang/include/ccl/rslang/ValueAuditor.h` & `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueAuditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/ASTInterpreter.cpp` & `pyconcept-0.1.3/ccl/rslang/src/ASTInterpreter.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "ccl/rslang/ASTInterpreter.h"
 
 #include "NameCollector.h"
 
 #include <stack>
+#include <optional>
 
 #ifdef _MSC_VER
   #pragma warning( push )
   #pragma warning( disable : 26446 ) // Do not warn about operator[] access
 #endif
 
 using ccl::object::StructuredData;
@@ -90,19 +91,19 @@
     return current + 1 >= imperative.ChildrenCount();
   }
 
   [[nodiscard]] bool SaveElement() {
     auto element = parent.EvaluateChild(imperative, 0);
     if (!element.has_value()) {
       return false;
-    } else {
-      value.ModifyB().AddElement(std::get<StructuredData>(element.value()));
-      incrementIter = true;
-      return true;
     }
+
+    value.ModifyB().AddElement(std::get<StructuredData>(element.value()));
+    incrementIter = true;
+    return true;
   }
 
   [[nodiscard]] bool ProcessBlock() {
     auto child = imperative;
     child.MoveToChild(static_cast<Index>(current + 1));
     auto& meta = metaData.at(static_cast<size_t>(current));
 
@@ -184,16 +185,15 @@
   if (reporter.has_value()) {
     std::invoke(reporter.value(), err);
   }
 }
 
 std::optional<ExpressionValue> ASTInterpreter::Evaluate(const rslang::SyntaxTree& tree) {
   Clear();
-  if (!NameCollector{ *this }.Visit(tree.Root())
-      || !tree.Root().DispatchVisit(*this)) {
+  if (!NameCollector{ *this }.Visit(tree.Root()) || !tree.Root().DispatchVisit(*this)) {
     AfterVisit(false);
     return std::nullopt;
   } else {
     AfterVisit(true);
     return curValue;
   }
 }
@@ -243,101 +243,108 @@
 }
 
 bool ASTInterpreter::ViEmptySet(Cursor /*iter*/) {
   return VisitAndReturn(Factory::EmptySet());
 }
 
 bool ASTInterpreter::ViArithmetic(Cursor iter) {
-  if (const auto val1 = EvaluateChild(iter, 0); !val1.has_value()) {
+  const auto val1 = EvaluateChild(iter, 0);
+  if (!val1.has_value()) {
     return false;
-  } else if (const auto val2 = EvaluateChild(iter, 1); !val2.has_value()) {
+  }
+  const auto val2 = EvaluateChild(iter, 1);
+  if (!val2.has_value()) {
     return false;
-  } else {
-    const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
-    const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
-    switch (iter->id) {
-    default:
-    case TokenID::PLUS:
-      return VisitAndReturn(Factory::Val(op1 + op2));
-    case TokenID::MINUS:
-      return VisitAndReturn(Factory::Val(op1 - op2));
-    case TokenID::MULTIPLY:
-      return VisitAndReturn(Factory::Val(op1 * op2));
-    }
+  }
+  const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
+  const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
+  switch (iter->id) {
+  default:
+  case TokenID::PLUS:
+    return VisitAndReturn(Factory::Val(op1 + op2));
+  case TokenID::MINUS:
+    return VisitAndReturn(Factory::Val(op1 - op2));
+  case TokenID::MULTIPLY:
+    return VisitAndReturn(Factory::Val(op1 * op2));
   }
 }
 
 bool ASTInterpreter::ViCard(Cursor iter) {
-  if (const auto base = EvaluateChild(iter, 0); !base.has_value()) {
+  const auto base = EvaluateChild(iter, 0);
+  if (!base.has_value()) {
     return false;
-  } else if (const auto size = std::get<StructuredData>(base.value()).B().Cardinality();
-             size == StructuredData::SET_INFINITY) {
+  }
+  const auto size = std::get<StructuredData>(base.value()).B().Cardinality();
+  if (size == StructuredData::SET_INFINITY) {
     OnError(ValueEID::typedOverflow, iter->pos.start, std::to_string(StructuredData::SET_INFINITY));
     return false;
-  } else {
-    return VisitAndReturn(Factory::Val(size));
   }
+  return VisitAndReturn(Factory::Val(size));
 }
 
 bool ASTInterpreter::ViQuantifier(Cursor iter) {
-  const auto quantorDomain = ExtractDomain(iter);
-  if (!quantorDomain.has_value()) {
+  const auto domain = ExtractDomain(iter);
+  if (!domain.has_value()) {
     return false;
   }
 
   const auto varID = *begin(nodeVars[iter.Child(0).get()]);
-  const auto quantorForAll = iter->id == TokenID::FORALL;
-  for (const auto& child : quantorDomain->B()) {
+  const auto isUniversal = iter->id == TokenID::FORALL;
+  for (const auto& child : domain->B()) {
     if (++iterationCounter > MAX_ITERATIONS) {
       OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
       return false;
     }
     idsData[varID] = child;
     if (const auto iterationValue = EvaluateChild(iter, 2); !iterationValue.has_value()) {
       return false;
-    } else if (std::get<bool>(iterationValue.value()) != quantorForAll) {
-      return VisitAndReturn(!quantorForAll);
+    } else if (std::get<bool>(iterationValue.value()) != isUniversal) {
+      return VisitAndReturn(!isUniversal);
     }
   }
-  return VisitAndReturn(quantorForAll);
+  return VisitAndReturn(isUniversal);
 }
 
 std::optional<StructuredData> ASTInterpreter::ExtractDomain(Cursor iter) {
   if (!VisitChild(iter, 1)) {
     return std::nullopt;
-  } else {
-    return std::optional<StructuredData>{std::get<StructuredData>(curValue)};
   }
+  return std::optional<StructuredData>{std::get<StructuredData>(curValue)};
 }
 
 bool ASTInterpreter::ViNegation(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(!std::get<bool>(childValue.value()));
   }
+  return VisitAndReturn(!std::get<bool>(childValue.value()));
 }
 
 bool ASTInterpreter::ViLogicBinary(Cursor iter) {
-  if (const auto val1 = EvaluateChild(iter, 0); !val1.has_value()) {
+  const auto val1 = EvaluateChild(iter, 0);
+  if (!val1.has_value()) {
     return false;
-  } else if (TryEvaluateFromFirstArg(iter->id, std::get<bool>(val1.value()))) {
+  }
+
+  if (TryEvaluateFromFirstArg(iter->id, std::get<bool>(val1.value()))) {
     return true;
-  } else if (const auto val2 = EvaluateChild(iter, 1); !val2.has_value()) {
+  } 
+
+  const auto val2 = EvaluateChild(iter, 1);
+  if (!val2.has_value()) {
     return false;
-  } else {
-    const auto op1 = std::get<bool>(val1.value());
-    const auto op2 = std::get<bool>(val2.value());
-    switch (iter->id) {
+  }
+  const auto op1 = std::get<bool>(val1.value());
+  const auto op2 = std::get<bool>(val2.value());
+  switch (iter->id) {
     default:
     case TokenID::AND: curValue = op1 && op2;  return true;
     case TokenID::OR: curValue = op1 || op2;  return true;
     case TokenID::IMPLICATION: curValue = !op1 || op2;  return true;
-    case TokenID::EQUIVALENT: curValue = op1 == op2;  return true;
-    }
+    case TokenID::EQUIVALENT: curValue = op1 == op2; return true;
   }
 }
 
 bool ASTInterpreter::TryEvaluateFromFirstArg(TokenID operation, bool firstArgValue) noexcept {
   if ((operation == TokenID::AND && !firstArgValue) ||
     (operation == TokenID::OR && firstArgValue)) {
     return VisitAndReturn(firstArgValue);
@@ -345,38 +352,42 @@
     return VisitAndReturn(!firstArgValue);
   } else {
     return false;
   }
 }
 
 bool ASTInterpreter::ViEquals(Cursor iter) {
-  if (const auto val1 = EvaluateChild(iter, 0); !val1.has_value()) {
+  const auto val1 = EvaluateChild(iter, 0);
+  if (!val1.has_value()) {
     return false;
-  } else if (const auto val2 = EvaluateChild(iter, 1); !val2.has_value()) {
+  }
+  const auto val2 = EvaluateChild(iter, 1);
+  if (!val2.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn((val1 == val2) != (iter->id == TokenID::NOTEQUAL));
   }
+  return VisitAndReturn((val1 == val2) != (iter->id == TokenID::NOTEQUAL));
 }
 
 bool ASTInterpreter::ViOrdering(Cursor iter) {
-  if (const auto val1 = EvaluateChild(iter, 0); !val1.has_value()) {
+  const auto val1 = EvaluateChild(iter, 0);
+  if (!val1.has_value()) {
     return false;
-  } else if (const auto val2 = EvaluateChild(iter, 1); !val2.has_value()) {
+  }
+  const auto val2 = EvaluateChild(iter, 1);
+  if (!val2.has_value()) {
     return false;
-  } else {
-    const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
-    const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
-    switch (iter->id) {
+  }
+  const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
+  const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
+  switch (iter->id) {
     default:
     case TokenID::GREATER: return VisitAndReturn(op1 > op2);
     case TokenID::LESSER: return VisitAndReturn(op1 < op2);
     case TokenID::GREATER_OR_EQ: return VisitAndReturn(op1 >= op2);
     case TokenID::LESSER_OR_EQ: return VisitAndReturn(op1 <= op2);
-    }
   }
 }
 
 bool ASTInterpreter::ViDeclarative(Cursor iter) {
   const auto setDomain = ExtractDomain(iter);
   if (!setDomain.has_value()) {
     return false;
@@ -385,30 +396,31 @@
   auto result = Factory::EmptySet();
   for (const auto& child : setDomain->B()) {
     if (++iterationCounter > MAX_ITERATIONS) {
       OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
       return false;
     }
     idsData[varID] = child;
-    if (const auto predicatValue = EvaluateChild(iter, 2); !predicatValue.has_value()) {
+    const auto predicatValue = EvaluateChild(iter, 2);
+    if (!predicatValue.has_value()) {
       return false;
-    } else if (std::get<bool>(predicatValue.value())) {
+    }
+    if (std::get<bool>(predicatValue.value())) {
       result.ModifyB().AddElement(child);
     }
   }
   return VisitAndReturn(std::move(result));
 }
 
 bool ASTInterpreter::ViImperative(const Cursor iter) {
   ImpEvaluator eval{ *this, iter };
   if (!eval.Evaluate()) {
     return false;
-  } else {
-    return VisitAndReturn(eval.value);
   }
+  return VisitAndReturn(eval.value);
 }
 
 bool ASTInterpreter::ViRecursion(Cursor iter) {
   const auto initial = ExtractDomain(iter);
   if (!initial.has_value()) {
     return false;
   }
@@ -418,17 +430,19 @@
     if (++iterationCounter > MAX_ITERATIONS) {
       OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
       return false;
     }
 
     idsData[varID] = current;
     if (iter->id == TokenID::NT_RECURSIVE_FULL) {
-      if (const auto predicat = EvaluateChild(iter, 2); !predicat.has_value()) {
+      const auto predicat = EvaluateChild(iter, 2);
+      if (!predicat.has_value()) {
         return false;
-      } else if (!std::get<bool>(predicat.value())) {
+      }
+      if (!std::get<bool>(predicat.value())) {
         break;
       }
     }
 
     if (!VisitChild(iter, iter->id == TokenID::NT_RECURSIVE_FULL ? 3 : 2)) {
       return false;
     }
@@ -447,94 +461,103 @@
     }
   }
 
   curValue = Factory::Decartian(args);
   if (std::get<StructuredData>(curValue).B().Cardinality() == StructuredData::SET_INFINITY) {
     OnError(ValueEID::typedOverflow, iter->pos.start, std::to_string(StructuredData::SET_INFINITY));
     return false;
-  } else {
-    return true;
   }
+  return true;
 }
 
 bool ASTInterpreter::ViBoolean(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else if (const auto value = std::get<StructuredData>(childValue.value());
-             (iter.IsRoot() || (iter.Parent().id != TokenID::IN && iter.Parent().id != TokenID::NT_DECLARATIVE_EXPR)) &&
-             value.B().Cardinality() >= StructuredData::BOOL_INFINITY) {
-    OnError(ValueEID::booleanLimit, iter->pos.start, std::to_string(StructuredData::BOOL_INFINITY));
+  }
+  const auto value = std::get<StructuredData>(childValue.value());
+  if (
+      (iter.IsRoot() || (iter.Parent().id != TokenID::IN && iter.Parent().id != TokenID::NT_DECLARATIVE_EXPR)) &&
+      value.B().Cardinality() >= StructuredData::BOOL_INFINITY
+    ) {
+    OnError(
+      ValueEID::booleanLimit,
+      iter->pos.start,
+      std::to_string(StructuredData::BOOL_INFINITY)
+    );
     return false;
-  } else {
-    return VisitAndReturn(Factory::Boolean(value));
   }
+  return VisitAndReturn(Factory::Boolean(value));
 }
 
 bool ASTInterpreter::ViTuple(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
-    if (const auto childValue = EvaluateChild(iter, child); !childValue.has_value()) {
+    const auto childValue = EvaluateChild(iter, child);
+    if (!childValue.has_value()) {
       return false;
-    } else {
-      args.emplace_back(std::get<StructuredData>(childValue.value()));
     }
+    args.emplace_back(std::get<StructuredData>(childValue.value()));
   }
   return VisitAndReturn(Factory::Tuple(args));
 }
 
 bool ASTInterpreter::ViSetEnum(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
-    if (const auto childValue = EvaluateChild(iter, child); !childValue.has_value()) {
+    const auto childValue = EvaluateChild(iter, child);
+    if (!childValue.has_value()) {
       return false;
-    } else {
-      args.emplace_back(std::get<StructuredData>(childValue.value()));
     }
+    args.emplace_back(std::get<StructuredData>(childValue.value()));
   }
   return VisitAndReturn(Factory::Set(args));
 }
 
 bool ASTInterpreter::ViBool(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(Factory::Singleton(std::get<StructuredData>(childValue.value())));
   }
+  return VisitAndReturn(Factory::Singleton(std::get<StructuredData>(childValue.value())));
 }
 
 bool ASTInterpreter::ViTypedBinary(Cursor iter) {
-  if (const auto val1 = EvaluateChild(iter, 0); !val1.has_value()) {
+  const auto val1 = EvaluateChild(iter, 0);
+  if (!val1.has_value()) {
     return false;
-  } else if (const auto val2 = EvaluateChild(iter, 1); !val2.has_value()) {
+  }
+  const auto val2 = EvaluateChild(iter, 1); 
+  if (!val2.has_value()) {
     return false;
-  } else {
-    const auto& op1 = std::get<StructuredData>(val1.value());
-    const auto& op2 = std::get<StructuredData>(val2.value());
-    switch (iter->id) {
+  }
+
+  const auto& op1 = std::get<StructuredData>(val1.value());
+  const auto& op2 = std::get<StructuredData>(val2.value());
+  switch (iter->id) {
     default:
     case TokenID::UNION: return VisitAndReturn(op1.B().Union(op2.B()));
     case TokenID::INTERSECTION: return VisitAndReturn(op1.B().Intersect(op2.B()));
     case TokenID::SET_MINUS: return VisitAndReturn(op1.B().Diff(op2.B()));
     case TokenID::SYMMINUS: return VisitAndReturn(op1.B().SymDiff(op2.B()));
 
     case TokenID::IN: return VisitAndReturn(op2.B().Contains(op1));
     case TokenID::NOTIN: return VisitAndReturn(!op2.B().Contains(op1));
     case TokenID::SUBSET: return VisitAndReturn(!(op1 == op2) && op1.B().IsSubsetOrEq(op2.B()));
     case TokenID::NOTSUBSET: return VisitAndReturn(op1 == op2 || !op1.B().IsSubsetOrEq(op2.B()));
     case TokenID::SUBSET_OR_EQ: return VisitAndReturn(op1.B().IsSubsetOrEq(op2.B()));
-    }
   }
 }
 
 bool ASTInterpreter::ViProjectSet(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Projection(iter->data.ToTuple()));
   }
+  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Projection(iter->data.ToTuple()));
 }
 
 bool ASTInterpreter::ViProjectTuple(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
@@ -558,17 +581,19 @@
     return VisitAndReturn(Factory::EmptySet());
   }
 
   const auto& indicies = iter->data.ToTuple();
   std::vector<StructuredData> params{};
   params.reserve(size(indicies));
   for (Index child = 0; child < iter.ChildrenCount() - 1; ++child) {
-    if (const auto param = EvaluateChild(iter, child); !param.has_value()) {
+    const auto param = EvaluateChild(iter, child);
+    if (!param.has_value()) {
       return false;
-    } else if (const auto val = std::get<StructuredData>(param.value()); val.B().IsEmpty()) {
+    } 
+    if (const auto val = std::get<StructuredData>(param.value()); val.B().IsEmpty()) {
       return VisitAndReturn(Factory::EmptySet());
     } else {
       params.emplace_back(val);
     }
   }
 
   auto result = Factory::EmptySet();
@@ -584,31 +609,32 @@
       result.ModifyB().AddElement(element);
     }
   }
   return VisitAndReturn(std::move(result));
 }
 
 bool ASTInterpreter::ViReduce(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Reduce());
   }
+  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Reduce());
 }
 
 bool ASTInterpreter::ViDebool(Cursor iter) {
-  if (const auto childValue = EvaluateChild(iter, 0); !childValue.has_value()) {
+  const auto childValue = EvaluateChild(iter, 0);
+  if (!childValue.has_value()) {
     return false;
-  } else if (const auto value = std::get<StructuredData>(childValue.value());
-             value.B().Cardinality() != 1) {
+  }
+  const auto value = std::get<StructuredData>(childValue.value());
+  if (value.B().Cardinality() != 1) {
     OnError(ValueEID::invalidDebool, iter->pos.start);
     return false;
-  } else {
-    return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Debool());
   }
+  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Debool());
 }
 
 std::optional<ExpressionValue> ASTInterpreter::EvaluateChild(Cursor iter, const Index index) {
   assert(iter.ChildrenCount() > index);
 
   ExpressionValue result = curValue;
   iter.MoveToChild(index);
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/ASTNormalizer.cpp` & `pyconcept-0.1.3/ccl/rslang/src/ASTNormalizer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,23 @@
   } else {
     newQuant->At(0) = newQuant->At(0)(1);
   }
   quant.AdoptChild(std::move(newQuant));
   quant(0) = quant(0)(0);
 }
 
-void Normalizer::TupleDeclaration(SyntaxTree::Node& declaration,
-                                  SyntaxTree::Node& predicat) {
+void Normalizer::TupleDeclaration(
+  SyntaxTree::Node& declaration,
+  SyntaxTree::Node& predicate
+) {
   const auto newName = CreateTupleName(declaration);
   declaration.RemoveAll();
   declaration.token.data = TokenData{ newName };
   declaration.token.id = TokenID::ID_LOCAL;
-
-  SubstituteTupleVariables(predicat, newName);
+  SubstituteTupleVariables(predicate, newName);
 }
 
 void Normalizer::TupleDeclaration(SyntaxTree::Node& target) {
   const auto token = target.token.id;
   auto newName = CreateTupleName(target(0));
 
   target(0).RemoveAll();
@@ -87,15 +88,15 @@
 std::string Normalizer::CreateTupleName(const SyntaxTree::Node& root) {
   tuples.clear();
   std::string newName{ '@' };
 
   std::stack<const SyntaxTree::Node*> nodeStack{};
   std::stack<std::vector<Index>> pathStack{};
   nodeStack.push(&root);
-  pathStack.push({});
+  pathStack.emplace();
   while (!std::empty(nodeStack)) {
     auto curPath = pathStack.top();
     pathStack.pop();
     const auto* curNode = nodeStack.top();
     nodeStack.pop();
     if (curNode->token.id == TokenID::ID_LOCAL) {
       const auto& name = curNode->token.data.ToText();
@@ -112,15 +113,16 @@
   }
   return newName;
 }
 
 void Normalizer::SubstituteTupleVariables(SyntaxTree::Node& target, const std::string& newName) {
   for (Index child = 0; child < target.ChildrenCount(); ++child) {
     if (target(child).token.id == TokenID::ID_LOCAL) {
-      if (const auto& localName = target(child).token.data.ToText(); tuples.contains(localName)) {
+      const auto& localName = target(child).token.data.ToText();
+      if (tuples.contains(localName)) {
         const auto& indexes = tuples.at(localName);
         target(child).token.data = TokenData{ newName };
         for (const auto prIndex : indexes) {
           target.ExtendChild(child, TokenID::SMALLPR);
           target(child).token.pos = target(child)(0).token.pos;
           target(child).token.data = TokenData{ std::vector<Index>{ prIndex } };
         }
@@ -160,20 +162,22 @@
 void Normalizer::SubstituteArgs(SyntaxTree::Node& target, const StrRange pos) {
   target.token.pos = pos;
   if (target.token.id != TokenID::ID_LOCAL) {
     for (Index child = 0; child < target.ChildrenCount(); ++child) {
       SubstituteArgs(target(child), pos);
     }
   } else {
-    if (const auto& localName = target.token.ToString(); nodes.contains(localName)) {
+    const auto& localName = target.token.ToString();
+    if (nodes.contains(localName)) {
       target = *nodes.at(localName);
     } else {
       const auto& oldName = target.token.ToString();
       std::string newName{};
-      if (const auto iter = nameSubstitutes.find(oldName); iter == std::end(nameSubstitutes)) {
+      const auto iter = nameSubstitutes.find(oldName);
+      if (iter == std::end(nameSubstitutes)) {
         ++localVarBase;
         newName = R"(__var)" + std::to_string(localVarBase);
         nameSubstitutes.insert(make_pair(oldName, newName));
       } else {
         newName = iter->second;
       }
       target.token.data = TokenData{ newName };
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/AsciiLexer.cpp` & `pyconcept-0.1.3/ccl/rslang/src/AsciiLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/Auditor.cpp` & `pyconcept-0.1.3/ccl/rslang/src/Auditor.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#pragma once
-
 #include "ccl/rslang/Auditor.h"
 
 namespace ccl::rslang {
 
 
 Auditor::Auditor(const TypeContext& types, ValueClassContext globalClass, SyntaxTreeContext globalAST)
   : typeAuditor{ types, parser.log.SendReporter() },
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/ErrorLogger.cpp` & `pyconcept-0.1.3/ccl/rslang/src/ErrorLogger.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -17,33 +17,46 @@
 }
 
 void ErrorLogger::LogError(const Error& error) {
   errors.emplace_back(error);
 }
 
 int32_t ErrorLogger::Count(const ErrorStatus status) const {
-  return static_cast<int32_t>(std::count_if(begin(errors), end(errors), 
-                   [&](const Error& error) noexcept 
-                   { return ResolveErrorType(error.eid) == status; }));
+  return static_cast<int32_t>(
+    std::count_if(
+      begin(errors),
+      end(errors), 
+      [&](const Error& error) noexcept {
+        return ResolveErrorType(error.eid) == status;
+      }
+    )
+  );
 }
 
 ErrorReporter ErrorLogger::SendReporter() {
   return [log = this](const Error& err) { log->LogError(err); };
 }
 
 StrPos ErrorLogger::FirstErrorPos() const {
   if (std::empty(errors)) {
     return 0;
-  } else {
-    return std::accumulate(next(begin(errors)), end(errors), begin(errors)->position,
-                           [](StrPos minimum, const Error& error) 
-                           { return std::min(error.position, minimum); });
   }
+  return std::accumulate(
+    next(begin(errors)),
+    end(errors),
+    begin(errors)->position,
+    [](StrPos minimum, const Error& error) {
+      return std::min(error.position, minimum);
+    });
 }
 
 bool ErrorLogger::HasCriticalErrors() const {
-  return std::any_of(begin(errors), end(errors), 
-                     [](const Error& error) noexcept 
-                     { return error.IsCritical(); });
+  return std::any_of(
+    begin(errors),
+    end(errors), 
+    [](const Error& error) noexcept {
+      return error.IsCritical();
+    }
+  );
 }
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/GeneratorImplAST.cpp` & `pyconcept-0.1.3/ccl/rslang/src/GeneratorImplAST.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/Interpreter.cpp` & `pyconcept-0.1.3/ccl/rslang/src/Interpreter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#pragma once
-
 #include "ccl/rslang/Interpreter.h"
 
+#include <optional>
+
 namespace ccl::rslang {
 
 Interpreter::Interpreter(const TypeContext& types, SyntaxTreeContext ast, DataContext data)
   : auditor{ types, parser.log.SendReporter() }, 
     interpreter{ std::move(data), parser.log.SendReporter() },
     astContext{ std::move(ast) } {}
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/Literals.cpp` & `pyconcept-0.1.3/ccl/rslang/src/Literals.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -37,33 +37,39 @@
 
 } // unnamed namespace
 
 Typification operator""_t(const char* input, const size_t /*size*/) {
   static detail::AsciiLexer lexer{};
   static detail::RSParser parser{};
   static EchoTypeEnvironment env{};
-  static TypeAuditor analyse{ env };
+  static TypeAuditor analyser{ env };
+  analyser.SetExepectTypification();
 
   env.Clear();
   if (!parser.Parse(lexer(input).Stream())) {
     assert(false);
     return Typification::Integer();
-  } else if (!analyse.CheckType(parser.AST())) {
+  } 
+  if (!analyser.CheckType(parser.AST())) {
     assert(false);
     return Typification::Integer();
-  } else if (const auto& result = analyse.GetType();
-             !std::holds_alternative<Typification>(result)) {
+  } 
+
+  const auto& result = analyser.GetType();
+  if (!std::holds_alternative<Typification>(result)) {
     assert(false);
     return Typification::Integer();
-  } else if (const auto& type = std::get<Typification>(result); !type.IsCollection()) {
+  } 
+
+  const auto& type = std::get<Typification>(result); 
+  if (!type.IsCollection()) {
     assert(false);
     return Typification::Integer();
-  } else {
-    return type.B().Base();
   }
+  return type.B().Base();
 }
 
 std::string operator"" _rs(const char* input, const size_t size) {
   return ConvertTo(std::string(input, size), Syntax::MATH);
 }
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/MathLexer.cpp` & `pyconcept-0.1.3/ccl/rslang/src/MathLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/NameCollector.cpp` & `pyconcept-0.1.3/ccl/rslang/src/NameCollector.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -45,22 +45,23 @@
   if (parent.idsBase.contains(idName)) {
     parent.nodeVars[iter.get()] = { parent.idsBase[idName] };
     return true;
   }
 
   const auto nextID = static_cast<uint32_t>(size(parent.idsData));
   parent.idsBase.insert({ idName, nextID });
-  if (const auto data = parent.context(iter->data.ToText()); data.has_value()) {
-    parent.idsData.emplace_back(data.value());
-    parent.nodeVars[iter.get()] = { nextID };
-    return true;
-  } else {
+  const auto data = parent.context(iter->data.ToText());
+  if (!data.has_value()) {
     parent.OnError(ValueEID::globalMissingValue, iter->pos.start, iter->data.ToText());
     return false;
-  }
+    
+  } 
+  parent.idsData.emplace_back(data.value());
+  parent.nodeVars[iter.get()] = { nextID };
+  return true;
 }
 
 bool ASTInterpreter::NameCollector::ViLocal(Cursor iter) {
   const auto& idName = iter->data.ToText();
   if (parent.idsBase.contains(idName)) {
     parent.nodeVars[iter.get()] = { parent.idsBase[idName] };
   } else {
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/Parser.cpp` & `pyconcept-0.1.3/ccl/rslang/src/Parser.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/RSExpr.cpp` & `pyconcept-0.1.3/ccl/rslang/src/RSExpr.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/RSGenerator.cpp` & `pyconcept-0.1.3/ccl/rslang/src/RSGenerator.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 #include "GeneratorImplAST.h"
 
 #include "ccl/Substitutes.hpp"
 #include "ccl/rslang/RSExpr.h"
 #include "ccl/rslang/Parser.h"
 
+#include <string_view>
+
 namespace ccl::rslang {
 
 namespace {
 
+using Description = Generator::StructureDescription;
+
 [[nodiscard]] size_t FindArgumentSectionEnd(const std::string& input) {
   auto counter = 0;
   for (auto iter = UTF8Iterator(input); iter != UTF8End(input); ++iter) {
     if (*iter == '[') {
       ++counter;
     } else if (*iter == ']') {
       if (counter == 1) {
@@ -22,89 +26,102 @@
         --counter;
       }
     }
   }
   return std::string::npos;
 }
 
-[[nodiscard]] std::string SubstituteInPrefix(const StrSubstitutes& substitutes,
-                                             const std::vector<std::string>& args, const TypeContext& env) {
+[[nodiscard]] std::string SubstituteInPrefix(
+  const StrSubstitutes& substitutes,
+  const std::vector<std::string>& args,
+  const TypeContext& env
+) {
   FunctionArguments argsTypes{};
   for (const auto& argName : args) {
-    if (const auto* type = env.TypeFor(argName); type == nullptr) {
+    const auto* type = env.TypeFor(argName);
+    if (type == nullptr) {
       return {};
-    } else {
-      const auto& newName = substitutes.at(argName);
-      argsTypes.emplace_back(TypedID{ newName, std::get<Typification>(*type) });
     }
+    const auto& newName = substitutes.at(argName);
+    argsTypes.emplace_back(newName, std::get<Typification>(*type));
   }
   return Generator::CreatePrefix(argsTypes);
 }
 
-class StructureContextGenerator final {
+class StructureGenerator final {
 private:
-  Generator::StructureDescription structure{};
+  Description structure{};
 
 public:
-  [[nodiscard]] static Generator::StructureDescription GenerateFor(const std::string& cstName, 
-                                                                   const Typification& type);
+  [[nodiscard]] static Description GenerateFor(
+    const std::string& cstName,
+    const Typification& type
+  );
 
 private:
   void GenerateRecursive(const std::string& currentStr, const Typification& type);
   void GenerateReduce(const std::string& currentStr, const Typification& type);
   void GenerateProjection(const std::string& currentStr, const Typification& type);
-  void CallRecursionForToken(const std::string& tokenText,
-                             const std::string& currentStr,
-                             const Typification& type);
+  void CallRecursionForToken(
+    const std::string& tokenText,
+    const std::string& currentStr,
+    const Typification& type
+  );
 };
 
-Generator::StructureDescription StructureContextGenerator::GenerateFor(const std::string& cstName, 
-                                                                       const Typification& type) {
-  static StructureContextGenerator generator{};
+Description StructureGenerator::GenerateFor(
+  const std::string& cstName,
+  const Typification& type
+) {
+  static StructureGenerator generator{};
   generator.structure.clear();
   generator.GenerateRecursive(cstName, type);
   return generator.structure;
 }
 
-void StructureContextGenerator::GenerateRecursive(const std::string& currentStr, const Typification& type) {
+void StructureGenerator::GenerateRecursive(const std::string& currentStr, const Typification& type) {
   if (!empty(currentStr) && type.IsCollection()) {
     const auto& elementType = type.B().Base();
     switch (elementType.Structure()) {
     case rslang::StructureType::basic: return;
     case rslang::StructureType::collection: GenerateReduce(currentStr, elementType); break;
     case rslang::StructureType::tuple: GenerateProjection(currentStr, elementType); break;
     }
   }
 }
 
-void StructureContextGenerator::GenerateReduce(const std::string& currentStr, const Typification& type) {
+void StructureGenerator::GenerateReduce(const std::string& currentStr, const Typification& type) {
   CallRecursionForToken(rslang::Token::Str(rslang::TokenID::REDUCE), currentStr, type);
 }
 
-void StructureContextGenerator::GenerateProjection(const std::string& currentStr, const Typification& type) {
+void StructureGenerator::GenerateProjection(const std::string& currentStr, const Typification& type) {
   for (Index i = 0; i < type.T().Arity(); ++i) {
     Typification component = type.T().Component(Typification::PR_START + i); // NOLINT
     const auto tokenText = rslang::Token::Str(rslang::TokenID::BIGPR) + std::to_string(Typification::PR_START + i);
     CallRecursionForToken(tokenText, currentStr, component.ApplyBool());
   }
 }
 
-void StructureContextGenerator::CallRecursionForToken(const std::string& tokenText,
-                                                      const std::string& currentStr,
-                                                      const Typification& type) {
+void StructureGenerator::CallRecursionForToken(
+  const std::string& tokenText,
+  const std::string& currentStr,
+  const Typification& type
+) {
   std::string newStr = tokenText;
   newStr += '(';
   newStr += currentStr;
   newStr += ')';
   structure.emplace_back(newStr, type);
   GenerateRecursive(newStr, type);
 }
 
-[[nodiscard]] StrSubstitutes UniqueSubstitutes(const std::vector<std::string>& args,
-                                    const std::unordered_set<std::string>& takenNames) {
+[[nodiscard]] StrSubstitutes UniqueSubstitutes(
+  const std::vector<std::string>& args,
+  const std::unordered_set<std::string>& takenNames
+) {
   static constexpr auto LOCAL_ID_BASE = 1;
   static const std::string_view LOCAL_NAME_BASE = "arg";
   StrSubstitutes substitutes{};
   auto id = LOCAL_ID_BASE;
   for (const auto& argName : args) {
     std::string localName{};
     do {
@@ -148,16 +165,18 @@
   if (prefixEnd == std::string::npos) {
     return {};
   } else {
     return declaration.substr(0, prefixEnd);
   }
 }
 
-std::string Generator::FunctionFromExpr(const std::vector<std::string>& args, 
-                                        const std::string& expression) const {
+std::string Generator::FunctionFromExpr(
+  const std::vector<std::string>& args, 
+  const std::string& expression
+) const {
   if (empty(args) || empty(expression)) {
     return expression;
   }
   
   const auto substitutes = UniqueSubstitutes(args, rslang::ExtractULocals(expression));
   std::string funcExpression = expression;
   SubstituteGlobals(funcExpression, substitutes);
@@ -179,17 +198,19 @@
         return result;
       }
     );
   }
   return funcName + '[' + argString + ']';
 }
 
-std::string Generator::TermFromFunction(const std::string& funcName, 
-                                        const std::string& expression,
-                                        const std::vector<std::string>& args) const {
+std::string Generator::TermFromFunction(
+  const std::string& funcName, 
+  const std::string& expression,
+  const std::vector<std::string>& args
+) const {
   const auto* argsTypes = environment.FunctionArgsFor(funcName);
   if (argsTypes == nullptr || ssize(*argsTypes) != ssize(args)) {
     return {};
   }
   const auto prefixEnd = FindArgumentSectionEnd(expression);
   if (prefixEnd == std::string::npos || prefixEnd == std::size(expression)) {
     return {};
@@ -204,17 +225,19 @@
   for (auto i = 0U; i < size(args); ++i) {
     replMap.insert({ argsTypes->at(i).name, args.at(i) });
   }
   TranslateRS(result, TFFactory::FilterIdentifiers(), CreateTranslator(replMap));
   return result;
 }
 
-Generator::StructureDescription Generator::StructureFor(const std::string& globalName, 
-                                                        const Typification& type) {
-  return StructureContextGenerator::GenerateFor(globalName, type);
+Generator::StructureDescription Generator::StructureFor(
+  const std::string& globalName, 
+  const Typification& type
+) {
+  return StructureGenerator::GenerateFor(globalName, type);
 }
 
 std::string ConvertTo(const std::string& input, const Syntax targetSyntax) {
   Parser parser{};
   const auto initialSyntax = targetSyntax == Syntax::MATH ? Syntax::ASCII : Syntax::MATH;
   if (!parser.Parse(input, initialSyntax)) {
     return input;
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/RSParser.cpp` & `pyconcept-0.1.3/ccl/rslang/src/RSParser.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 
 #ifdef _MSC_VER
   #pragma warning( push )
   #pragma warning( disable : 26418 26415 26440 )
 #endif
 
+#include <optional>
+
 namespace ccl::rslang::detail {
 
 RSParser::RSParser(std::optional<ErrorReporter> reporter)
   : state{ reporter }, impl{ std::make_unique<RSParserImpl>(&state) } {}
 
 RSParser::~RSParser() = default;
 RSParser::RSParser(RSParser&& rhs) noexcept = default;
@@ -54,23 +56,21 @@
     return static_cast<int>(token.id);
   }
 }
 
 void RSParserImpl::error(const std::string& /*msg*/) {}
 
 RawNode AddNode(const TokenID token, RawNode son) {
-  auto result = std::make_shared<Node>(Token(token, son->token.pos));
-
+  auto result = std::make_shared<Node>(token, son->token.pos);
   result->children.emplace_back(son);
   return result;
 }
 
 RawNode AddNode(const TokenID token, RawNode son1, RawNode son2) {
-  auto result = std::make_shared<Node>(
-    Token{ token, StrRange{ son1->token.pos.start, son2->token.pos.finish } });
+  auto result = std::make_shared<Node>(token, StrRange{ son1->token.pos.start, son2->token.pos.finish });
   result->children.emplace_back(son1);
   result->children.emplace_back(son2);
   return result;
 }
 
 RawNode BinaryOperation(RawNode op1, RawNode operation, RawNode op2) {
   operation->token.pos = StrRange{ op1->token.pos.start, op2->token.pos.finish };
@@ -83,27 +83,27 @@
   operation->token.pos.finish = operand->token.pos.finish;
   operation->children.emplace_back(operand);
   return operation;
 }
 
 RawNode RemoveBrackets(RawNode br1, RawNode operand, RawNode br2) {
   operand->token.pos = StrRange{ br1->token.pos.start, br2->token.pos.finish };
-  auto bracketNode = std::make_shared<Node>(Token(TokenID::PUNC_PL, operand->token.pos));
+  auto bracketNode = std::make_shared<Node>(TokenID::PUNC_PL, operand->token.pos);
   bracketNode->children.emplace_back(operand);
   return bracketNode;
 }
 
 RawNode ReplaceBrackets(const TokenID token, RawNode br1, RawNode argList, RawNode br2) {
-  auto result = std::make_shared<Node>(Token(token, StrRange{ br1->token.pos.start, br2->token.pos.finish }));
+  auto result = std::make_shared<Node>(token, StrRange{ br1->token.pos.start, br2->token.pos.finish });
   result->children = argList->children;
   return result;
 }
 
 RawNode Enumeration(const TokenID token, RawNode el1, RawNode el2) {
-  auto result = std::make_shared<Node>(Token(token, StrRange{ el1->token.pos.start, el2->token.pos.finish }));
+  auto result = std::make_shared<Node>(token, StrRange{ el1->token.pos.start, el2->token.pos.finish });
   if (el1->token.id != token) {
     result->children.emplace_back(el1);
   } else {
     result->children = el1->children;
   }
   if (el2->token.id != token) {
     result->children.emplace_back(el2);
@@ -117,87 +117,120 @@
   quant->token.pos.finish = predicate->token.pos.finish;
   quant->children.emplace_back(declaration);
   quant->children.emplace_back(domain);
   quant->children.emplace_back(predicate);
   return quant;
 }
 
-RawNode FunctionDeclaration(RawNode start, RawNode argdecl, RawNode expr) {
+RawNode FunctionDeclaration(RawNode start, RawNode argumentsDeclaration, RawNode expr) {
   auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_FUNC_DEFINITION,  StrRange{ start->token.pos.start, expr->token.pos.finish } });
-  result->children.emplace_back(argdecl);
+    TokenID::NT_FUNC_DEFINITION,
+    StrRange{ start->token.pos.start, expr->token.pos.finish }
+  );
+  result->children.emplace_back(argumentsDeclaration);
   result->children.emplace_back(expr);
   return result;
 }
 
 RawNode FunctionCall(RawNode function, RawNode args, RawNode rs) {
   auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_FUNC_CALL,  StrRange{ function->token.pos.start, rs->token.pos.finish } });
+    TokenID::NT_FUNC_CALL,
+    StrRange{ function->token.pos.start, rs->token.pos.finish }
+  );
   result->children.emplace_back(function);
-  result->children.insert(end(result->children), begin(args->children), end(args->children));
+  result->children.insert(
+    end(result->children),
+    begin(args->children),
+    end(args->children)
+  );
   return result;
 }
 
 RawNode FilterCall(RawNode filter, RawNode params, RawNode argument, RawNode rp) {
   filter->token.pos.finish = rp->token.pos.finish;
   filter->children = params->children;
   filter->children.emplace_back(argument);
   return filter;
 }
 
-RawNode TextOperator(RawNode oper, RawNode args, RawNode rp) {
-  oper->token.pos.finish = rp->token.pos.finish;
-  oper->children.emplace_back(args);
-  return oper;
+RawNode TextOperator(RawNode operatorName, RawNode args, RawNode rp) {
+  operatorName->token.pos.finish = rp->token.pos.finish;
+  operatorName->children.emplace_back(args);
+  return operatorName;
 }
 
-RawNode Decartian(RawNode op1, RawNode decart, RawNode op2) {
+RawNode Decartian(RawNode op1, RawNode decartian, RawNode op2) {
   if (op1->token.id == TokenID::DECART) {
     auto result = std::move(op1);
     result->token.pos.finish = op2->token.pos.finish;
     result->children.emplace_back(op2);
     return result;
   } else {
-    return BinaryOperation(std::move(op1), std::move(decart), std::move(op2));
+    return BinaryOperation(std::move(op1), std::move(decartian), std::move(op2));
   }
 }
 
-RawNode TermDeclaration(RawNode lc, RawNode declaration, RawNode domain, RawNode predicate, RawNode rc) {
-  auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_DECLARATIVE_EXPR,  StrRange{ lc->token.pos.start, rc->token.pos.finish } });
+RawNode TermDeclaration(
+  RawNode lc,
+  RawNode declaration,
+  RawNode domain,
+  RawNode predicate,
+  RawNode rc
+) {
+  auto result = std::make_shared<Node>(
+    TokenID::NT_DECLARATIVE_EXPR,
+    StrRange{ lc->token.pos.start, rc->token.pos.finish }
+  );
   result->children.emplace_back(declaration);
   result->children.emplace_back(domain);
   result->children.emplace_back(predicate);
   return result;
 }
 
-RawNode FullRecursion(RawNode rec, RawNode localid, 
-                      RawNode domain, RawNode condition, RawNode iteration, RawNode rc) {
-  auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_RECURSIVE_FULL, StrRange{ rec->token.pos.start, rc->token.pos.finish } });
-  result->children.emplace_back(localid);
+RawNode FullRecursion(
+  RawNode rec,
+  RawNode declaration, 
+  RawNode domain,
+  RawNode condition,
+  RawNode iteration,
+  RawNode rc
+) {
+  auto result = std::make_shared<Node>(
+    TokenID::NT_RECURSIVE_FULL,
+    StrRange{ rec->token.pos.start, rc->token.pos.finish }
+  );
+  result->children.emplace_back(declaration);
   result->children.emplace_back(domain);
   result->children.emplace_back(condition);
   result->children.emplace_back(iteration);
   return result;
 }
 
-RawNode ShortRecursion(RawNode rec, RawNode localid, 
-                       RawNode domain, RawNode iteration, RawNode rc) {
-  auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_RECURSIVE_SHORT, StrRange{ rec->token.pos.start, rc->token.pos.finish } });
-  result->children.emplace_back(localid);
+RawNode ShortRecursion(
+  RawNode rec,
+  RawNode declaration, 
+  RawNode domain,
+  RawNode iteration,
+  RawNode rc
+) {
+  auto result = std::make_shared<Node>(
+    TokenID::NT_RECURSIVE_SHORT,
+    StrRange{ rec->token.pos.start, rc->token.pos.finish }
+  );
+  result->children.emplace_back(declaration);
   result->children.emplace_back(domain);
   result->children.emplace_back(iteration);
   return result;
 }
 
 RawNode Imperative(RawNode imp, RawNode value, RawNode actions, RawNode rc) {
   auto result = std::make_shared<Node>(
-    Token{ TokenID::NT_IMPERATIVE_EXPR, StrRange{ imp->token.pos.start, rc->token.pos.finish } });
+    TokenID::NT_IMPERATIVE_EXPR,
+    StrRange{ imp->token.pos.start, rc->token.pos.finish }
+  );
   result->children.emplace_back(value);
   result->children.insert(end(result->children), begin(actions->children), end(actions->children));
   return result;
 }
 
 SyntaxTree::RawNode CreateNodeRecursive(Node& astNode) {
   if (astNode.token.id == TokenID::PUNC_PL) {
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/RSParserImpl.cpp` & `pyconcept-0.1.3/ccl/rslang/src/RSParserImpl.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// A Bison parser, made by GNU Bison 3.3.2.
+// A Bison parser, made by GNU Bison 3.7.4.
 
 // Skeleton implementation for Bison LALR(1) parsers in C++
 
-// Copyright (C) 2002-2015, 2018-2019 Free Software Foundation, Inc.
+// Copyright (C) 2002-2015, 2018-2020 Free Software Foundation, Inc.
 
 // This program is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
 
 // This program is distributed in the hope that it will be useful,
@@ -26,23 +26,24 @@
 // special exception, which will cause the skeleton and the resulting
 // Bison output files to be licensed under the GNU General Public
 // License without this special exception.
 
 // This special exception was added by the Free Software Foundation in
 // version 2.2 of Bison.
 
-// Undocumented macros, especially those whose name start with YY_,
-// are private implementation details.  Do not rely on them.
+// DO NOT RELY ON FEATURES THAT ARE NOT DOCUMENTED in the manual,
+// especially those whose name start with YY_ or yy_.  They are
+// private implementation details that can be changed or removed.
 
-// //                    "%code top" blocks.
-#line 16 "RSParserImpl.y" // lalr1.cc:423
+// "%code top" blocks.
+#line 24 "RSParserImpl.y"
 
 #ifdef _MSC_VER
   #pragma warning( push )
-  #pragma warning( disable : 26434 26438 26440 26446 26447 26448 26456 )
+  #pragma warning( disable : 4244 26434 26438 26440 26446 26447 26448 26456 )
   #pragma warning( disable : 26460 26477 26481 26482 26493 26494 26495 26496 )
 #endif
 
 #ifdef __clang__
   #pragma clang diagnostic push
   #pragma clang diagnostic ignored "-Wsign-conversion"
   #pragma clang diagnostic ignored "-Wunused-but-set-variable"
@@ -50,15 +51,15 @@
 
 #if defined(__GNUC__) && !defined(__clang__)
   #pragma GCC diagnostic push
   #pragma GCC diagnostic ignored "-Wuseless-cast"
 #endif
 
 
-#line 58 "RSParserImpl.cpp" // lalr1.cc:423
+#line 59 "RSParserImpl.cpp"
 
 
 
 
 #include "RSParserImpl.h"
 
 
@@ -72,28 +73,26 @@
 #  endif
 # endif
 # ifndef YY_
 #  define YY_(msgid) msgid
 # endif
 #endif
 
+
 // Whether we are compiled with exception support.
 #ifndef YY_EXCEPTIONS
 # if defined __GNUC__ && !defined __EXCEPTIONS
 #  define YY_EXCEPTIONS 0
 # else
 #  define YY_EXCEPTIONS 1
 # endif
 #endif
 
 
 
-// Suppress unused-variable warnings by "using" E.
-#define YYUSE(E) ((void) (E))
-
 // Enable debugging if requested.
 #if YYDEBUG
 
 // A pseudo ostream that takes yydebug_ into account.
 # define YYCDEBUG if (yydebug_) (*yycdebug_)
 
 # define YY_SYMBOL_PRINT(Title, Symbol)         \
@@ -111,15 +110,15 @@
     if (yydebug_)                       \
       yy_reduce_print_ (Rule);          \
   } while (false)
 
 # define YY_STACK_PRINT()               \
   do {                                  \
     if (yydebug_)                       \
-      yystack_print_ ();                \
+      yy_stack_print_ ();                \
   } while (false)
 
 #else // !YYDEBUG
 
 # define YYCDEBUG if (false) std::cerr
 # define YY_SYMBOL_PRINT(Title, Symbol)  YYUSE (Symbol)
 # define YY_REDUCE_PRINT(Rule)           static_cast<void> (0)
@@ -131,88 +130,40 @@
 #define yyclearin       (yyla.clear ())
 
 #define YYACCEPT        goto yyacceptlab
 #define YYABORT         goto yyabortlab
 #define YYERROR         goto yyerrorlab
 #define YYRECOVERING()  (!!yyerrstatus_)
 
-#line 11 "RSParserImpl.y" // lalr1.cc:510
+#line 15 "RSParserImpl.y"
 namespace ccl { namespace rslang { namespace detail {
-#line 141 "RSParserImpl.cpp" // lalr1.cc:510
-
-  /* Return YYSTR after stripping away unnecessary quotes and
-     backslashes, so that it's suitable for yyerror.  The heuristic is
-     that double-quoting is unnecessary unless the string contains an
-     apostrophe, a comma, or backslash (other than backslash-backslash).
-     YYSTR is taken from yytname.  */
-  std::string
-  RSParserImpl::yytnamerr_ (const char *yystr)
-  {
-    if (*yystr == '"')
-      {
-        std::string yyr;
-        char const *yyp = yystr;
-
-        for (;;)
-          switch (*++yyp)
-            {
-            case '\'':
-            case ',':
-              goto do_not_strip_quotes;
-
-            case '\\':
-              if (*++yyp != '\\')
-                goto do_not_strip_quotes;
-              else
-                goto append;
-
-            append:
-            default:
-              yyr += *yyp;
-              break;
-
-            case '"':
-              return yyr;
-            }
-      do_not_strip_quotes: ;
-      }
-
-    return yystr;
-  }
-
+#line 140 "RSParserImpl.cpp"
 
   /// Build a parser object.
   RSParserImpl::RSParserImpl (ParserState* state_yyarg)
-    :
 #if YYDEBUG
-      yydebug_ (false),
+    : yydebug_ (false),
       yycdebug_ (&std::cerr),
+#else
+    :
 #endif
       state (state_yyarg)
   {}
 
   RSParserImpl::~RSParserImpl ()
   {}
 
   RSParserImpl::syntax_error::~syntax_error () YY_NOEXCEPT YY_NOTHROW
   {}
 
   /*---------------.
-  | Symbol types.  |
+  | symbol kinds.  |
   `---------------*/
 
   // basic_symbol.
-#if 201103L <= YY_CPLUSPLUS
-  template <typename Base>
-  RSParserImpl::basic_symbol<Base>::basic_symbol (basic_symbol&& that)
-    : Base (std::move (that))
-    , value (std::move (that.value))
-  {}
-#endif
-
   template <typename Base>
   RSParserImpl::basic_symbol<Base>::basic_symbol (const basic_symbol& that)
     : Base (that)
     , value (that.value)
   {}
 
 
@@ -226,66 +177,79 @@
   template <typename Base>
   RSParserImpl::basic_symbol<Base>::basic_symbol (typename Base::kind_type t, YY_RVREF (semantic_type) v)
     : Base (t)
     , value (YY_MOVE (v))
   {}
 
   template <typename Base>
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::basic_symbol<Base>::type_get () const YY_NOEXCEPT
+  {
+    return this->kind ();
+  }
+
+  template <typename Base>
   bool
   RSParserImpl::basic_symbol<Base>::empty () const YY_NOEXCEPT
   {
-    return Base::type_get () == empty_symbol;
+    return this->kind () == symbol_kind::S_YYEMPTY;
   }
 
   template <typename Base>
   void
   RSParserImpl::basic_symbol<Base>::move (basic_symbol& s)
   {
     super_type::move (s);
     value = YY_MOVE (s.value);
   }
 
-  // by_type.
-  RSParserImpl::by_type::by_type ()
-    : type (empty_symbol)
+  // by_kind.
+  RSParserImpl::by_kind::by_kind ()
+    : kind_ (symbol_kind::S_YYEMPTY)
   {}
 
 #if 201103L <= YY_CPLUSPLUS
-  RSParserImpl::by_type::by_type (by_type&& that)
-    : type (that.type)
+  RSParserImpl::by_kind::by_kind (by_kind&& that)
+    : kind_ (that.kind_)
   {
     that.clear ();
   }
 #endif
 
-  RSParserImpl::by_type::by_type (const by_type& that)
-    : type (that.type)
+  RSParserImpl::by_kind::by_kind (const by_kind& that)
+    : kind_ (that.kind_)
   {}
 
-  RSParserImpl::by_type::by_type (token_type t)
-    : type (yytranslate_ (t))
+  RSParserImpl::by_kind::by_kind (token_kind_type t)
+    : kind_ (yytranslate_ (t))
   {}
 
   void
-  RSParserImpl::by_type::clear ()
+  RSParserImpl::by_kind::clear ()
   {
-    type = empty_symbol;
+    kind_ = symbol_kind::S_YYEMPTY;
   }
 
   void
-  RSParserImpl::by_type::move (by_type& that)
+  RSParserImpl::by_kind::move (by_kind& that)
   {
-    type = that.type;
+    kind_ = that.kind_;
     that.clear ();
   }
 
-  int
-  RSParserImpl::by_type::type_get () const YY_NOEXCEPT
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_kind::kind () const YY_NOEXCEPT
+  {
+    return kind_;
+  }
+
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_kind::type_get () const YY_NOEXCEPT
   {
-    return type;
+    return this->kind ();
   }
 
 
   // by_state.
   RSParserImpl::by_state::by_state () YY_NOEXCEPT
     : state (empty_state)
   {}
@@ -307,21 +271,21 @@
     that.clear ();
   }
 
   RSParserImpl::by_state::by_state (state_type s) YY_NOEXCEPT
     : state (s)
   {}
 
-  RSParserImpl::symbol_number_type
-  RSParserImpl::by_state::type_get () const YY_NOEXCEPT
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_state::kind () const YY_NOEXCEPT
   {
     if (state == empty_state)
-      return empty_symbol;
+      return symbol_kind::S_YYEMPTY;
     else
-      return yystos_[state];
+      return YY_CAST (symbol_kind_type, yystos_[+state]);
   }
 
   RSParserImpl::stack_symbol_type::stack_symbol_type ()
   {}
 
   RSParserImpl::stack_symbol_type::stack_symbol_type (YY_RVREF (stack_symbol_type) that)
     : super_type (YY_MOVE (that.state), YY_MOVE (that.value))
@@ -332,19 +296,27 @@
 #endif
   }
 
   RSParserImpl::stack_symbol_type::stack_symbol_type (state_type s, YY_MOVE_REF (symbol_type) that)
     : super_type (s, YY_MOVE (that.value))
   {
     // that is emptied.
-    that.type = empty_symbol;
+    that.kind_ = symbol_kind::S_YYEMPTY;
   }
 
 #if YY_CPLUSPLUS < 201103L
   RSParserImpl::stack_symbol_type&
+  RSParserImpl::stack_symbol_type::operator= (const stack_symbol_type& that)
+  {
+    state = that.state;
+    value = that.value;
+    return *this;
+  }
+
+  RSParserImpl::stack_symbol_type&
   RSParserImpl::stack_symbol_type::operator= (stack_symbol_type& that)
   {
     state = that.state;
     value = that.value;
     // that is emptied.
     that.state = empty_state;
     return *this;
@@ -355,36 +327,34 @@
   void
   RSParserImpl::yy_destroy_ (const char* yymsg, basic_symbol<Base>& yysym) const
   {
     if (yymsg)
       YY_SYMBOL_PRINT (yymsg, yysym);
 
     // User destructor.
-    YYUSE (yysym.type_get ());
+    YYUSE (yysym.kind ());
   }
 
 #if YYDEBUG
   template <typename Base>
   void
-  RSParserImpl::yy_print_ (std::ostream& yyo,
-                                     const basic_symbol<Base>& yysym) const
+  RSParserImpl::yy_print_ (std::ostream& yyo, const basic_symbol<Base>& yysym) const
   {
     std::ostream& yyoutput = yyo;
     YYUSE (yyoutput);
-    symbol_number_type yytype = yysym.type_get ();
-#if defined __GNUC__ && ! defined __clang__ && ! defined __ICC && __GNUC__ * 100 + __GNUC_MINOR__ <= 408
-    // Avoid a (spurious) G++ 4.8 warning about "array subscript is
-    // below array bounds".
     if (yysym.empty ())
-      std::abort ();
-#endif
-    yyo << (yytype < yyntokens_ ? "token" : "nterm")
-        << ' ' << yytname_[yytype] << " (";
-    YYUSE (yytype);
-    yyo << ')';
+      yyo << "empty symbol";
+    else
+      {
+        symbol_kind_type yykind = yysym.kind ();
+        yyo << (yykind < YYNTOKENS ? "token" : "nterm")
+            << ' ' << yysym.name () << " (";
+        YYUSE (yykind);
+        yyo << ')';
+      }
   }
 #endif
 
   void
   RSParserImpl::yypush_ (const char* m, YY_MOVE_REF (stack_symbol_type) sym)
   {
     if (m)
@@ -435,19 +405,19 @@
     yydebug_ = l;
   }
 #endif // YYDEBUG
 
   RSParserImpl::state_type
   RSParserImpl::yy_lr_goto_state_ (state_type yystate, int yysym)
   {
-    int yyr = yypgoto_[yysym - yyntokens_] + yystate;
+    int yyr = yypgoto_[yysym - YYNTOKENS] + yystate;
     if (0 <= yyr && yyr <= yylast_ && yycheck_[yyr] == yystate)
       return yytable_[yyr];
     else
-      return yydefgoto_[yysym - yyntokens_];
+      return yydefgoto_[yysym - YYNTOKENS];
   }
 
   bool
   RSParserImpl::yy_pact_value_is_default_ (int yyvalue)
   {
     return yyvalue == yypact_ninf_;
   }
@@ -463,15 +433,14 @@
   {
     return parse ();
   }
 
   int
   RSParserImpl::parse ()
   {
-    // State.
     int yyn;
     /// Length of the RHS of the rule being reduced.
     int yylen = 0;
 
     // Error handling.
     int yynerrs_ = 0;
     int yyerrstatus_ = 0;
@@ -496,58 +465,71 @@
     yystack_.clear ();
     yypush_ (YY_NULLPTR, 0, YY_MOVE (yyla));
 
   /*-----------------------------------------------.
   | yynewstate -- push a new symbol on the stack.  |
   `-----------------------------------------------*/
   yynewstate:
-    YYCDEBUG << "Entering state " << yystack_[0].state << '\n';
+    YYCDEBUG << "Entering state " << int (yystack_[0].state) << '\n';
+    YY_STACK_PRINT ();
 
     // Accept?
     if (yystack_[0].state == yyfinal_)
       YYACCEPT;
 
     goto yybackup;
 
 
   /*-----------.
   | yybackup.  |
   `-----------*/
   yybackup:
     // Try to take a decision without lookahead.
-    yyn = yypact_[yystack_[0].state];
+    yyn = yypact_[+yystack_[0].state];
     if (yy_pact_value_is_default_ (yyn))
       goto yydefault;
 
     // Read a lookahead token.
     if (yyla.empty ())
       {
-        YYCDEBUG << "Reading a token: ";
+        YYCDEBUG << "Reading a token\n";
 #if YY_EXCEPTIONS
         try
 #endif // YY_EXCEPTIONS
           {
-            yyla.type = yytranslate_ (yylex (&yyla.value, state));
+            yyla.kind_ = yytranslate_ (yylex (&yyla.value, state));
           }
 #if YY_EXCEPTIONS
         catch (const syntax_error& yyexc)
           {
             YYCDEBUG << "Caught exception: " << yyexc.what() << '\n';
             error (yyexc);
             goto yyerrlab1;
           }
 #endif // YY_EXCEPTIONS
       }
     YY_SYMBOL_PRINT ("Next token is", yyla);
 
+    if (yyla.kind () == symbol_kind::S_YYerror)
+    {
+      // The scanner already issued an error message, process directly
+      // to error recovery.  But do not keep the error token as
+      // lookahead, it is too special and may lead us to an endless
+      // loop in error recovery. */
+      yyla.kind_ = symbol_kind::S_YYUNDEF;
+      goto yyerrlab1;
+    }
+
     /* If the proper action on seeing token YYLA.TYPE is to reduce or
        to detect an error, take that action.  */
-    yyn += yyla.type_get ();
-    if (yyn < 0 || yylast_ < yyn || yycheck_[yyn] != yyla.type_get ())
-      goto yydefault;
+    yyn += yyla.kind ();
+    if (yyn < 0 || yylast_ < yyn || yycheck_[yyn] != yyla.kind ())
+      {
+        goto yydefault;
+      }
 
     // Reduce or error.
     yyn = yytable_[yyn];
     if (yyn <= 0)
       {
         if (yy_table_value_is_error_ (yyn))
           goto yyerrlab;
@@ -556,23 +538,23 @@
       }
 
     // Count tokens shifted since error; after three, turn off error status.
     if (yyerrstatus_)
       --yyerrstatus_;
 
     // Shift the lookahead token.
-    yypush_ ("Shifting", yyn, YY_MOVE (yyla));
+    yypush_ ("Shifting", state_type (yyn), YY_MOVE (yyla));
     goto yynewstate;
 
 
   /*-----------------------------------------------------------.
   | yydefault -- do the default action for the current state.  |
   `-----------------------------------------------------------*/
   yydefault:
-    yyn = yydefact_[yystack_[0].state];
+    yyn = yydefact_[+yystack_[0].state];
     if (yyn == 0)
       goto yyerrlab;
     goto yyreduce;
 
 
   /*-----------------------------.
   | yyreduce -- do a reduction.  |
@@ -598,376 +580,377 @@
       YY_REDUCE_PRINT (yyn);
 #if YY_EXCEPTIONS
       try
 #endif // YY_EXCEPTIONS
         {
           switch (yyn)
             {
-  case 3:
-#line 151 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeExpression(yystack_[0].value); }
-#line 609 "RSParserImpl.cpp" // lalr1.cc:919
+  case 3: // expression: logic_or_setexpr
+#line 263 "RSParserImpl.y"
+                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 591 "RSParserImpl.cpp"
     break;
 
-  case 4:
-#line 152 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeExpression(yystack_[0].value); }
-#line 615 "RSParserImpl.cpp" // lalr1.cc:919
+  case 4: // expression: function_decl
+#line 264 "RSParserImpl.y"
+                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 597 "RSParserImpl.cpp"
     break;
 
-  case 7:
-#line 159 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = FunctionDeclaration(yystack_[3].value, yystack_[2].value, yystack_[0].value); }
-#line 621 "RSParserImpl.cpp" // lalr1.cc:919
+  case 5: // global_declaration: GLOBAL DEFINE
+#line 268 "RSParserImpl.y"
+                                            { state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value); }
+#line 603 "RSParserImpl.cpp"
     break;
 
-  case 8:
-#line 160 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
-#line 627 "RSParserImpl.cpp" // lalr1.cc:919
+  case 6: // global_declaration: GLOBAL STRUCT setexpr
+#line 269 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 609 "RSParserImpl.cpp"
     break;
 
-  case 9:
-#line 163 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::NT_ARGUMENTS, yystack_[0].value); }
-#line 633 "RSParserImpl.cpp" // lalr1.cc:919
+  case 7: // global_declaration: GLOBAL DEFINE logic_or_setexpr
+#line 270 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 615 "RSParserImpl.cpp"
     break;
 
-  case 10:
-#line 164 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Enumeration(TokenID::NT_ARGUMENTS, yystack_[2].value, yystack_[0].value); }
-#line 639 "RSParserImpl.cpp" // lalr1.cc:919
+  case 8: // global_declaration: function_name DEFINE function_decl
+#line 271 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 621 "RSParserImpl.cpp"
     break;
 
-  case 11:
-#line 165 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 645 "RSParserImpl.cpp" // lalr1.cc:919
+  case 13: // function_decl: LS arguments RS logic_or_setexpr
+#line 284 "RSParserImpl.y"
+                                            { yylhs.value = FunctionDeclaration(yystack_[3].value, yystack_[2].value, yystack_[0].value); }
+#line 627 "RSParserImpl.cpp"
     break;
 
-  case 12:
-#line 167 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::NT_ARG_DECL, yystack_[2].value, yystack_[0].value); }
-#line 651 "RSParserImpl.cpp" // lalr1.cc:919
+  case 14: // function_decl: LS error
+#line 285 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
+#line 633 "RSParserImpl.cpp"
     break;
 
-  case 13:
-#line 168 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
-#line 657 "RSParserImpl.cpp" // lalr1.cc:919
+  case 15: // arguments: declaration
+#line 290 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_ARGUMENTS, yystack_[0].value); }
+#line 639 "RSParserImpl.cpp"
     break;
 
-  case 14:
-#line 172 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value); }
-#line 663 "RSParserImpl.cpp" // lalr1.cc:919
+  case 16: // arguments: arguments COMMA declaration
+#line 291 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::NT_ARGUMENTS, yystack_[2].value, yystack_[0].value); }
+#line 645 "RSParserImpl.cpp"
     break;
 
-  case 15:
-#line 173 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 669 "RSParserImpl.cpp" // lalr1.cc:919
+  case 17: // arguments: arguments COMMA error
+#line 292 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 651 "RSParserImpl.cpp"
     break;
 
-  case 16:
-#line 174 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 675 "RSParserImpl.cpp" // lalr1.cc:919
+  case 18: // declaration: LOCAL IN setexpr
+#line 295 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_ARG_DECL, yystack_[2].value, yystack_[0].value); }
+#line 657 "RSParserImpl.cpp"
     break;
 
-  case 17:
-#line 175 "RSParserImpl.y" // lalr1.cc:919
-    { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 681 "RSParserImpl.cpp" // lalr1.cc:919
+  case 19: // declaration: LOCAL error
+#line 296 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
+#line 663 "RSParserImpl.cpp"
     break;
 
-  case 26:
-#line 190 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 687 "RSParserImpl.cpp" // lalr1.cc:919
+  case 21: // variable: LP var_enum RPE
+#line 301 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE_DECL, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 669 "RSParserImpl.cpp"
     break;
 
-  case 27:
-#line 191 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 693 "RSParserImpl.cpp" // lalr1.cc:919
+  case 22: // var_enum: var_all COMMA var_all
+#line 304 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 675 "RSParserImpl.cpp"
     break;
 
-  case 28:
-#line 193 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
-#line 699 "RSParserImpl.cpp" // lalr1.cc:919
+  case 23: // var_enum: var_all COMMA error
+#line 305 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 681 "RSParserImpl.cpp"
     break;
 
-  case 29:
-#line 195 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
-#line 705 "RSParserImpl.cpp" // lalr1.cc:919
+  case 31: // logic_par: LP logic_binary RPE
+#line 323 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 687 "RSParserImpl.cpp"
     break;
 
-  case 30:
-#line 196 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
-#line 711 "RSParserImpl.cpp" // lalr1.cc:919
+  case 32: // logic_par: LP logic_predicates RPE
+#line 324 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 693 "RSParserImpl.cpp"
     break;
 
-  case 31:
-#line 197 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 717 "RSParserImpl.cpp" // lalr1.cc:919
+  case 33: // logic_predicates: setexpr binary_predicate setexpr
+#line 328 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 699 "RSParserImpl.cpp"
     break;
 
-  case 32:
-#line 199 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 723 "RSParserImpl.cpp" // lalr1.cc:919
+  case 45: // logic_unary: NOT logic_no_binary
+#line 345 "RSParserImpl.y"
+                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
+#line 705 "RSParserImpl.cpp"
     break;
 
-  case 33:
-#line 201 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 729 "RSParserImpl.cpp" // lalr1.cc:919
+  case 46: // logic_unary: quantifier quant_var IN setexpr logic_no_binary
+#line 346 "RSParserImpl.y"
+                                                      { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
+#line 711 "RSParserImpl.cpp"
     break;
 
-  case 34:
-#line 202 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 735 "RSParserImpl.cpp" // lalr1.cc:919
+  case 47: // logic_unary: quantifier error
+#line 347 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
+#line 717 "RSParserImpl.cpp"
     break;
 
-  case 35:
-#line 203 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 741 "RSParserImpl.cpp" // lalr1.cc:919
+  case 48: // logic_unary: PREDICATE LS setexpr_enum RS
+#line 348 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 723 "RSParserImpl.cpp"
     break;
 
-  case 36:
-#line 204 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 747 "RSParserImpl.cpp" // lalr1.cc:919
+  case 56: // quant_var: LP error
+#line 362 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
+#line 729 "RSParserImpl.cpp"
     break;
 
-  case 39:
-#line 209 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
-#line 753 "RSParserImpl.cpp" // lalr1.cc:919
+  case 57: // quant_var_enum: quant_var COMMA quant_var
+#line 365 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
+#line 735 "RSParserImpl.cpp"
     break;
 
-  case 40:
-#line 211 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
-#line 759 "RSParserImpl.cpp" // lalr1.cc:919
+  case 58: // quant_var_enum: quant_var COMMA error
+#line 366 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 741 "RSParserImpl.cpp"
     break;
 
-  case 41:
-#line 212 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 765 "RSParserImpl.cpp" // lalr1.cc:919
+  case 59: // logic_binary: logic_all EQUIVALENT logic_all
+#line 370 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 747 "RSParserImpl.cpp"
     break;
 
-  case 46:
-#line 220 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 771 "RSParserImpl.cpp" // lalr1.cc:919
+  case 60: // logic_binary: logic_all IMPLICATION logic_all
+#line 371 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 753 "RSParserImpl.cpp"
     break;
 
-  case 47:
-#line 221 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 777 "RSParserImpl.cpp" // lalr1.cc:919
+  case 61: // logic_binary: logic_all OR logic_all
+#line 372 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 759 "RSParserImpl.cpp"
     break;
 
-  case 48:
-#line 224 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 783 "RSParserImpl.cpp" // lalr1.cc:919
+  case 62: // logic_binary: logic_all AND logic_all
+#line 373 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 765 "RSParserImpl.cpp"
     break;
 
-  case 49:
-#line 225 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 789 "RSParserImpl.cpp" // lalr1.cc:919
+  case 67: // setexpr: FUNCTION LS setexpr_enum RS
+#line 383 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 771 "RSParserImpl.cpp"
     break;
 
-  case 50:
-#line 226 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 795 "RSParserImpl.cpp" // lalr1.cc:919
+  case 68: // setexpr: operation_name LP setexpr RPE
+#line 384 "RSParserImpl.y"
+                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 777 "RSParserImpl.cpp"
     break;
 
-  case 51:
-#line 227 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 801 "RSParserImpl.cpp" // lalr1.cc:919
+  case 75: // setexpr_enum: setexpr
+#line 395 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
+#line 783 "RSParserImpl.cpp"
     break;
 
-  case 52:
-#line 228 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 807 "RSParserImpl.cpp" // lalr1.cc:919
+  case 77: // setexpr_enum_min2: setexpr_enum COMMA setexpr
+#line 399 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 789 "RSParserImpl.cpp"
     break;
 
-  case 53:
-#line 229 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 813 "RSParserImpl.cpp" // lalr1.cc:919
+  case 85: // setexpr_binary: setexpr PLUS setexpr
+#line 416 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 795 "RSParserImpl.cpp"
     break;
 
-  case 54:
-#line 230 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 819 "RSParserImpl.cpp" // lalr1.cc:919
+  case 86: // setexpr_binary: setexpr MINUS setexpr
+#line 417 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 801 "RSParserImpl.cpp"
     break;
 
-  case 55:
-#line 231 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Decartian(yystack_[2].value, yystack_[1].value, yystack_[0].value);}
-#line 825 "RSParserImpl.cpp" // lalr1.cc:919
+  case 87: // setexpr_binary: setexpr MULTIPLY setexpr
+#line 418 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 807 "RSParserImpl.cpp"
     break;
 
-  case 56:
-#line 232 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 831 "RSParserImpl.cpp" // lalr1.cc:919
+  case 88: // setexpr_binary: setexpr UNION setexpr
+#line 419 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 813 "RSParserImpl.cpp"
     break;
 
-  case 60:
-#line 238 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = FilterCall(yystack_[6].value, yystack_[4].value, yystack_[1].value, yystack_[0].value); }
-#line 837 "RSParserImpl.cpp" // lalr1.cc:919
+  case 89: // setexpr_binary: setexpr SET_MINUS setexpr
+#line 420 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 819 "RSParserImpl.cpp"
     break;
 
-  case 64:
-#line 243 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = ReplaceBrackets(TokenID::NT_ENUMERATION, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 843 "RSParserImpl.cpp" // lalr1.cc:919
+  case 90: // setexpr_binary: setexpr SYMMINUS setexpr
+#line 421 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 825 "RSParserImpl.cpp"
     break;
 
-  case 65:
-#line 245 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 849 "RSParserImpl.cpp" // lalr1.cc:919
+  case 91: // setexpr_binary: setexpr INTERSECTION setexpr
+#line 422 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 831 "RSParserImpl.cpp"
     break;
 
-  case 66:
-#line 247 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 855 "RSParserImpl.cpp" // lalr1.cc:919
+  case 92: // setexpr_binary: setexpr DECART setexpr
+#line 423 "RSParserImpl.y"
+                                            { yylhs.value = Decartian(yystack_[2].value, yystack_[1].value, yystack_[0].value);}
+#line 837 "RSParserImpl.cpp"
     break;
 
-  case 67:
-#line 248 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value); }
-#line 861 "RSParserImpl.cpp" // lalr1.cc:919
+  case 93: // setexpr_binary: LP setexpr_binary RPE
+#line 424 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 843 "RSParserImpl.cpp"
     break;
 
-  case 68:
-#line 250 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
-#line 867 "RSParserImpl.cpp" // lalr1.cc:919
+  case 101: // enumeration: LC setexpr_enum RC
+#line 437 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_ENUMERATION, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 849 "RSParserImpl.cpp"
     break;
 
-  case 70:
-#line 253 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 873 "RSParserImpl.cpp" // lalr1.cc:919
+  case 102: // tuple: LP setexpr_enum_min2 RPE
+#line 440 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 855 "RSParserImpl.cpp"
     break;
 
-  case 71:
-#line 255 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = TermDeclaration(yystack_[6].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 879 "RSParserImpl.cpp" // lalr1.cc:919
+  case 103: // boolean: BOOLEAN LP setexpr RPE
+#line 443 "RSParserImpl.y"
+                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 861 "RSParserImpl.cpp"
     break;
 
-  case 72:
-#line 257 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = TermDeclaration(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 885 "RSParserImpl.cpp" // lalr1.cc:919
+  case 104: // boolean: BOOLEAN boolean
+#line 444 "RSParserImpl.y"
+                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value); }
+#line 867 "RSParserImpl.cpp"
     break;
 
-  case 73:
-#line 260 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = FullRecursion(yystack_[9].value, yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 891 "RSParserImpl.cpp" // lalr1.cc:919
+  case 105: // filter_expression: FILTER LS setexpr_enum RS LP setexpr RPE
+#line 447 "RSParserImpl.y"
+                                               { yylhs.value = FilterCall(yystack_[6].value, yystack_[4].value, yystack_[1].value, yystack_[0].value); }
+#line 873 "RSParserImpl.cpp"
     break;
 
-  case 74:
-#line 262 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = ShortRecursion(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 897 "RSParserImpl.cpp" // lalr1.cc:919
+  case 106: // declarative: LC LOCAL IN setexpr BAR logic RCE
+#line 451 "RSParserImpl.y"
+                                            { yylhs.value = TermDeclaration(yystack_[6].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 879 "RSParserImpl.cpp"
     break;
 
-  case 75:
-#line 264 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Imperative(yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 903 "RSParserImpl.cpp" // lalr1.cc:919
+  case 107: // declarative: DECLARATIVE LC variable IN setexpr BAR logic RCE
+#line 452 "RSParserImpl.y"
+                                                       { yylhs.value = TermDeclaration(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 885 "RSParserImpl.cpp"
     break;
 
-  case 76:
-#line 266 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
-#line 909 "RSParserImpl.cpp" // lalr1.cc:919
+  case 108: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR logic BAR setexpr RCE
+#line 455 "RSParserImpl.y"
+                                                                     { yylhs.value = FullRecursion(yystack_[9].value, yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 891 "RSParserImpl.cpp"
     break;
 
-  case 77:
-#line 267 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 915 "RSParserImpl.cpp" // lalr1.cc:919
+  case 109: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR setexpr RCE
+#line 456 "RSParserImpl.y"
+                                                           { yylhs.value = ShortRecursion(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 897 "RSParserImpl.cpp"
     break;
 
-  case 78:
-#line 269 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::NT_IMP_DECLARE, yystack_[2].value, yystack_[0].value); }
-#line 921 "RSParserImpl.cpp" // lalr1.cc:919
+  case 110: // imperative: IMPERATIVE LC setexpr BAR imp_blocks RCE
+#line 459 "RSParserImpl.y"
+                                               { yylhs.value = Imperative(yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 903 "RSParserImpl.cpp"
     break;
 
-  case 79:
-#line 270 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::NT_IMP_ASSIGN, yystack_[2].value, yystack_[0].value); }
-#line 927 "RSParserImpl.cpp" // lalr1.cc:919
+  case 111: // imp_blocks: imp_block
+#line 462 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
+#line 909 "RSParserImpl.cpp"
     break;
 
-  case 80:
-#line 271 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = AddNode(TokenID::NT_IMP_LOGIC, yystack_[0].value); }
-#line 933 "RSParserImpl.cpp" // lalr1.cc:919
+  case 112: // imp_blocks: imp_blocks SEMICOLON imp_blocks
+#line 463 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 915 "RSParserImpl.cpp"
     break;
 
-  case 82:
-#line 274 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE_DECL, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 939 "RSParserImpl.cpp" // lalr1.cc:919
+  case 113: // imp_block: LOCAL ITERATE setexpr
+#line 466 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_DECLARE, yystack_[2].value, yystack_[0].value); }
+#line 921 "RSParserImpl.cpp"
     break;
 
-  case 83:
-#line 276 "RSParserImpl.y" // lalr1.cc:919
-    { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 945 "RSParserImpl.cpp" // lalr1.cc:919
+  case 114: // imp_block: LOCAL ASSIGN setexpr
+#line 467 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_ASSIGN, yystack_[2].value, yystack_[0].value); }
+#line 927 "RSParserImpl.cpp"
     break;
 
-  case 84:
-#line 277 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 951 "RSParserImpl.cpp" // lalr1.cc:919
+  case 115: // imp_block: logic
+#line 468 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_LOGIC, yystack_[0].value); }
+#line 933 "RSParserImpl.cpp"
     break;
 
-  case 117:
-#line 325 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::missingParanthesis); YYABORT; }
-#line 957 "RSParserImpl.cpp" // lalr1.cc:919
+  case 117: // RPE: error
+#line 475 "RSParserImpl.y"
+            { state->OnError(ParseEID::missingParenthesis); YYABORT; }
+#line 939 "RSParserImpl.cpp"
     break;
 
-  case 119:
-#line 328 "RSParserImpl.y" // lalr1.cc:919
-    { state->OnError(ParseEID::missingCurlyBrace); YYABORT; }
-#line 963 "RSParserImpl.cpp" // lalr1.cc:919
+  case 119: // RCE: error
+#line 479 "RSParserImpl.y"
+            { state->OnError(ParseEID::missingCurlyBrace); YYABORT; }
+#line 945 "RSParserImpl.cpp"
     break;
 
 
-#line 967 "RSParserImpl.cpp" // lalr1.cc:919
+#line 949 "RSParserImpl.cpp"
+
             default:
               break;
             }
         }
 #if YY_EXCEPTIONS
       catch (const syntax_error& yyexc)
         {
@@ -975,15 +958,14 @@
           error (yyexc);
           YYERROR;
         }
 #endif // YY_EXCEPTIONS
       YY_SYMBOL_PRINT ("-> $$ =", yylhs);
       yypop_ (yylen);
       yylen = 0;
-      YY_STACK_PRINT ();
 
       // Shift the result of the reduction.
       yypush_ (YY_NULLPTR, YY_MOVE (yylhs));
     }
     goto yynewstate;
 
 
@@ -991,25 +973,27 @@
   | yyerrlab -- here on detecting error.  |
   `--------------------------------------*/
   yyerrlab:
     // If not already recovering from an error, report this error.
     if (!yyerrstatus_)
       {
         ++yynerrs_;
-        error (yysyntax_error_ (yystack_[0].state, yyla));
+        context yyctx (*this, yyla);
+        std::string msg = yysyntax_error_ (yyctx);
+        error (YY_MOVE (msg));
       }
 
 
     if (yyerrstatus_ == 3)
       {
         /* If just tried and failed to reuse lookahead token after an
            error, discard it.  */
 
         // Return failure if at end of input.
-        if (yyla.type_get () == yyeof_)
+        if (yyla.kind () == symbol_kind::S_YYEOF)
           YYABORT;
         else if (!yyla.empty ())
           {
             yy_destroy_ ("Error: discarding", yyla);
             yyla.clear ();
           }
       }
@@ -1027,50 +1011,53 @@
     if (false)
       YYERROR;
 
     /* Do not reclaim the symbols of the rule whose action triggered
        this YYERROR.  */
     yypop_ (yylen);
     yylen = 0;
+    YY_STACK_PRINT ();
     goto yyerrlab1;
 
 
   /*-------------------------------------------------------------.
   | yyerrlab1 -- common code for both syntax error and YYERROR.  |
   `-------------------------------------------------------------*/
   yyerrlab1:
     yyerrstatus_ = 3;   // Each real token shifted decrements this.
+    // Pop stack until we find a state that shifts the error token.
+    for (;;)
+      {
+        yyn = yypact_[+yystack_[0].state];
+        if (!yy_pact_value_is_default_ (yyn))
+          {
+            yyn += symbol_kind::S_YYerror;
+            if (0 <= yyn && yyn <= yylast_
+                && yycheck_[yyn] == symbol_kind::S_YYerror)
+              {
+                yyn = yytable_[yyn];
+                if (0 < yyn)
+                  break;
+              }
+          }
+
+        // Pop the current state because it cannot handle the error token.
+        if (yystack_.size () == 1)
+          YYABORT;
+
+        yy_destroy_ ("Error: popping", yystack_[0]);
+        yypop_ ();
+        YY_STACK_PRINT ();
+      }
     {
       stack_symbol_type error_token;
-      for (;;)
-        {
-          yyn = yypact_[yystack_[0].state];
-          if (!yy_pact_value_is_default_ (yyn))
-            {
-              yyn += yyterror_;
-              if (0 <= yyn && yyn <= yylast_ && yycheck_[yyn] == yyterror_)
-                {
-                  yyn = yytable_[yyn];
-                  if (0 < yyn)
-                    break;
-                }
-            }
-
-          // Pop the current state because it cannot handle the error token.
-          if (yystack_.size () == 1)
-            YYABORT;
-
-          yy_destroy_ ("Error: popping", yystack_[0]);
-          yypop_ ();
-          YY_STACK_PRINT ();
-        }
 
 
       // Shift the error token.
-      error_token.state = yyn;
+      error_token.state = state_type (yyn);
       yypush_ ("Shifting", YY_MOVE (error_token));
     }
     goto yynewstate;
 
 
   /*-------------------------------------.
   | yyacceptlab -- YYACCEPT comes here.  |
@@ -1094,14 +1081,15 @@
   yyreturn:
     if (!yyla.empty ())
       yy_destroy_ ("Cleanup: discarding lookahead", yyla);
 
     /* Do not reclaim the symbols of the rule whose action triggered
        this YYABORT or YYACCEPT.  */
     yypop_ (yylen);
+    YY_STACK_PRINT ();
     while (1 < yystack_.size ())
       {
         yy_destroy_ ("Cleanup: popping", yystack_[0]);
         yypop_ ();
       }
 
     return yyresult;
@@ -1127,26 +1115,108 @@
 
   void
   RSParserImpl::error (const syntax_error& yyexc)
   {
     error (yyexc.what ());
   }
 
-  // Generate an error message.
+  /* Return YYSTR after stripping away unnecessary quotes and
+     backslashes, so that it's suitable for yyerror.  The heuristic is
+     that double-quoting is unnecessary unless the string contains an
+     apostrophe, a comma, or backslash (other than backslash-backslash).
+     YYSTR is taken from yytname.  */
   std::string
-  RSParserImpl::yysyntax_error_ (state_type yystate, const symbol_type& yyla) const
+  RSParserImpl::yytnamerr_ (const char *yystr)
   {
-    // Number of reported tokens (one for the "unexpected", one per
-    // "expected").
-    size_t yycount = 0;
-    // Its maximum.
-    enum { YYERROR_VERBOSE_ARGS_MAXIMUM = 5 };
-    // Arguments of yyformat.
-    char const *yyarg[YYERROR_VERBOSE_ARGS_MAXIMUM];
+    if (*yystr == '"')
+      {
+        std::string yyr;
+        char const *yyp = yystr;
 
+        for (;;)
+          switch (*++yyp)
+            {
+            case '\'':
+            case ',':
+              goto do_not_strip_quotes;
+
+            case '\\':
+              if (*++yyp != '\\')
+                goto do_not_strip_quotes;
+              else
+                goto append;
+
+            append:
+            default:
+              yyr += *yyp;
+              break;
+
+            case '"':
+              return yyr;
+            }
+      do_not_strip_quotes: ;
+      }
+
+    return yystr;
+  }
+
+  std::string
+  RSParserImpl::symbol_name (symbol_kind_type yysymbol)
+  {
+    return yytnamerr_ (yytname_[yysymbol]);
+  }
+
+
+
+  // RSParserImpl::context.
+  RSParserImpl::context::context (const RSParserImpl& yyparser, const symbol_type& yyla)
+    : yyparser_ (yyparser)
+    , yyla_ (yyla)
+  {}
+
+  int
+  RSParserImpl::context::expected_tokens (symbol_kind_type yyarg[], int yyargn) const
+  {
+    // Actual number of expected tokens
+    int yycount = 0;
+
+    int yyn = yypact_[+yyparser_.yystack_[0].state];
+    if (!yy_pact_value_is_default_ (yyn))
+      {
+        /* Start YYX at -YYN if negative to avoid negative indexes in
+           YYCHECK.  In other words, skip the first -YYN actions for
+           this state because they are default actions.  */
+        int yyxbegin = yyn < 0 ? -yyn : 0;
+        // Stay within bounds of both yycheck and yytname.
+        int yychecklim = yylast_ - yyn + 1;
+        int yyxend = yychecklim < YYNTOKENS ? yychecklim : YYNTOKENS;
+        for (int yyx = yyxbegin; yyx < yyxend; ++yyx)
+          if (yycheck_[yyx + yyn] == yyx && yyx != symbol_kind::S_YYerror
+              && !yy_table_value_is_error_ (yytable_[yyx + yyn]))
+            {
+              if (!yyarg)
+                ++yycount;
+              else if (yycount == yyargn)
+                return 0;
+              else
+                yyarg[yycount++] = YY_CAST (symbol_kind_type, yyx);
+            }
+      }
+
+    if (yyarg && yycount == 0 && 0 < yyargn)
+      yyarg[0] = symbol_kind::S_YYEMPTY;
+    return yycount;
+  }
+
+
+
+  int
+  RSParserImpl::yy_syntax_error_arguments_ (const context& yyctx,
+                                                 symbol_kind_type yyarg[], int yyargn) const
+  {
     /* There are many possibilities here to consider:
        - If this state is a consistent state with a default action, then
          the only way this function was invoked is if the default action
          is an error action.  In that case, don't check for expected
          tokens because there are none.
        - The only way there can be no lookahead present (in yyla) is
          if this state is a consistent state with a default action.
@@ -1157,49 +1227,40 @@
          a consistent state with a default action.  There might have
          been a previous inconsistent state, consistent state with a
          non-default action, or user semantic action that manipulated
          yyla.  (However, yyla is currently not documented for users.)
        - Of course, the expected token list depends on states to have
          correct lookahead information, and it depends on the parser not
          to perform extra reductions after fetching a lookahead from the
-         scanner and before detecting a syntax error.  Thus, state
-         merging (from LALR or IELR) and default reductions corrupt the
-         expected token list.  However, the list is correct for
-         canonical LR with one exception: it will still contain any
-         token that will not be accepted due to an error action in a
-         later state.
+         scanner and before detecting a syntax error.  Thus, state merging
+         (from LALR or IELR) and default reductions corrupt the expected
+         token list.  However, the list is correct for canonical LR with
+         one exception: it will still contain any token that will not be
+         accepted due to an error action in a later state.
     */
-    if (!yyla.empty ())
+
+    if (!yyctx.lookahead ().empty ())
       {
-        int yytoken = yyla.type_get ();
-        yyarg[yycount++] = yytname_[yytoken];
-        int yyn = yypact_[yystate];
-        if (!yy_pact_value_is_default_ (yyn))
-          {
-            /* Start YYX at -YYN if negative to avoid negative indexes in
-               YYCHECK.  In other words, skip the first -YYN actions for
-               this state because they are default actions.  */
-            int yyxbegin = yyn < 0 ? -yyn : 0;
-            // Stay within bounds of both yycheck and yytname.
-            int yychecklim = yylast_ - yyn + 1;
-            int yyxend = yychecklim < yyntokens_ ? yychecklim : yyntokens_;
-            for (int yyx = yyxbegin; yyx < yyxend; ++yyx)
-              if (yycheck_[yyx + yyn] == yyx && yyx != yyterror_
-                  && !yy_table_value_is_error_ (yytable_[yyx + yyn]))
-                {
-                  if (yycount == YYERROR_VERBOSE_ARGS_MAXIMUM)
-                    {
-                      yycount = 1;
-                      break;
-                    }
-                  else
-                    yyarg[yycount++] = yytname_[yyx];
-                }
-          }
+        if (yyarg)
+          yyarg[0] = yyctx.token ();
+        int yyn = yyctx.expected_tokens (yyarg ? yyarg + 1 : yyarg, yyargn - 1);
+        return yyn + 1;
       }
+    return 0;
+  }
+
+  // Generate an error message.
+  std::string
+  RSParserImpl::yysyntax_error_ (const context& yyctx) const
+  {
+    // Its maximum.
+    enum { YYARGS_MAX = 5 };
+    // Arguments of yyformat.
+    symbol_kind_type yyarg[YYARGS_MAX];
+    int yycount = yy_syntax_error_arguments_ (yyctx, yyarg, YYARGS_MAX);
 
     char const* yyformat = YY_NULLPTR;
     switch (yycount)
       {
 #define YYCASE_(N, S)                         \
         case N:                               \
           yyformat = S;                       \
@@ -1212,141 +1273,141 @@
         YYCASE_ (4, YY_("syntax error, unexpected %s, expecting %s or %s or %s"));
         YYCASE_ (5, YY_("syntax error, unexpected %s, expecting %s or %s or %s or %s"));
 #undef YYCASE_
       }
 
     std::string yyres;
     // Argument number.
-    size_t yyi = 0;
+    std::ptrdiff_t yyi = 0;
     for (char const* yyp = yyformat; *yyp; ++yyp)
       if (yyp[0] == '%' && yyp[1] == 's' && yyi < yycount)
         {
-          yyres += yytnamerr_ (yyarg[yyi++]);
+          yyres += symbol_name (yyarg[yyi++]);
           ++yyp;
         }
       else
         yyres += *yyp;
     return yyres;
   }
 
 
-  const signed char RSParserImpl::yypact_ninf_ = -65;
+  const signed char RSParserImpl::yypact_ninf_ = -58;
 
-  const signed char RSParserImpl::yytable_ninf_ = -87;
+  const signed char RSParserImpl::yytable_ninf_ = -116;
 
   const short
   RSParserImpl::yypact_[] =
   {
-     236,   -65,    92,   -43,   -40,   -65,   -65,   -65,   -65,   -65,
-     -65,   342,    37,   -65,   -65,   -37,   -65,   -65,   -65,   -65,
-     -16,    21,    26,   342,   414,   143,    56,   -65,   -65,   -65,
-     110,    90,   -65,   -65,   -65,   -65,   553,   -65,   -65,   -65,
-     -65,   -65,   -65,   -65,   -65,    83,   -65,   -65,   -65,    84,
-      85,   342,   466,   466,   466,   -65,   -65,   -65,   -65,   -65,
-     553,   -65,   466,   -65,   466,    93,    93,   466,   -65,    58,
-     101,   553,   202,   102,    19,   146,   -65,   466,   215,     2,
-     -65,   -65,    59,   103,   -65,   -65,   342,   342,   342,   342,
-     466,   466,   466,   -65,   -65,   -65,   -65,   -65,   -65,   -65,
-     -65,   -65,   -65,   -65,   466,   466,   466,   466,   466,   466,
-     114,   -65,   -65,   100,    12,   -65,   -65,   466,   -65,   215,
-     123,   195,   152,   203,    93,   163,   144,   489,   -65,   -65,
-     -65,   -65,   -65,   466,   -65,   466,   -65,   -65,   466,   342,
-     199,   125,   238,   185,   -65,   142,   142,   174,   -65,   -65,
-     -65,   -65,   -65,   215,   -65,   -65,   -65,    20,   194,   466,
-     127,   152,   -65,   -65,   -65,   207,   466,   466,   394,   215,
-     503,   215,   -65,   -65,   -65,   -65,   131,   290,   -65,   -65,
-     -65,   466,   516,   521,   106,     8,    10,   -65,   342,   -65,
-     -65,   -65,   -65,   152,   342,   342,   466,   466,   -65,   -65,
-     394,   -65,    11,   -65,    11,   208,    14,   215,   215,   -65,
-     -65,   -65,   466,   -65,    87,   -65
+     236,   -58,   111,   -34,   -17,   -58,   -58,   -58,   -58,   -58,
+     -58,   342,    82,   -58,   -58,    25,   -58,   -58,   -58,   -58,
+      46,    56,    75,   342,   414,     9,    60,   -58,    85,   -58,
+     -58,   137,   224,   -58,   -58,   -58,    79,   -58,   553,   118,
+     -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,
+     -58,   342,   466,   466,   466,   -58,   -58,   -58,   -58,   -58,
+     -58,   553,   466,   -58,   466,    35,    35,   466,   -58,    70,
+     101,   553,   121,    17,   202,   157,   -58,   466,   175,    24,
+     -58,   -58,    10,    63,   -58,   -58,    97,   342,   342,   342,
+     342,   -58,   -58,   100,   -58,   -19,   -58,   466,   466,   466,
+     -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,
+     -58,   466,   466,   466,   466,   466,   466,   466,   -58,   175,
+     126,   203,   129,   206,    35,   163,   144,   489,   -58,   -58,
+     -58,   -58,   466,   -58,   -58,   466,   -58,   -58,   466,   342,
+      89,   -58,   120,   241,   176,   -58,   -58,   -58,    19,   146,
+     466,   148,   143,   143,   190,   -58,   -58,   -58,   -58,   -58,
+     175,   129,   -58,   -58,   -58,   207,   466,   466,   394,   175,
+     503,   175,   -58,   -58,   -58,   -58,   154,   290,   -58,   -58,
+     -58,   466,   516,   521,   123,     6,     8,   -58,   342,   -58,
+     -58,   -58,   -58,   129,   342,   342,   466,   466,   -58,   -58,
+     394,   -58,    33,   -58,    33,   169,    14,   175,   175,   -58,
+     -58,   -58,   466,   -58,    73,   -58
   };
 
-  const unsigned char
+  const signed char
   RSParserImpl::yydefact_[] =
   {
-       0,    93,    89,    87,    88,    91,    94,    96,    95,    97,
-      98,     0,     0,   102,   103,     0,   104,    99,   100,   101,
-       0,     0,     0,     0,     0,     0,     0,     3,     4,     2,
-      21,     0,    22,    19,    18,    20,     6,    44,    45,    57,
-      58,    59,    61,    63,    62,    90,    92,    43,    42,     0,
-       0,    14,     0,     0,     0,    89,    28,    25,    24,    23,
-       0,    90,     0,    67,     0,     0,     0,     0,    21,     0,
-       0,    68,     0,     0,     0,    93,    88,     0,    68,     0,
-      69,     8,     0,     0,     9,     1,     0,     0,     0,     0,
-       0,     0,     0,   112,   113,   114,   115,   111,   110,   105,
-     106,   107,   108,   109,     0,     0,     0,     0,     0,     0,
-       0,    30,    81,     0,     0,    38,    37,     0,    16,    15,
+       0,    84,    81,     9,    10,    83,    78,    80,    79,    52,
+      53,     0,     0,    72,    73,     0,    74,    69,    70,    71,
+       0,     0,     0,     0,     0,     0,     0,     2,    82,     3,
+       4,    29,     0,    30,    26,    27,     0,    28,    12,     0,
+      63,    64,    65,    66,    94,    95,    96,    97,    98,   100,
+      99,     5,     0,     0,     0,    81,    82,    51,    49,    50,
+      45,     0,     0,   104,     0,     0,     0,     0,    29,     0,
+       0,    75,     0,     0,     0,    84,    10,     0,    75,     0,
+      76,    14,     0,     0,    15,     1,     0,     0,     0,     0,
+       0,    47,    20,     0,    54,     0,    55,     0,     0,     0,
+      41,    42,    43,    44,    40,    39,    34,    35,    36,    37,
+      38,     0,     0,     0,     0,     0,     0,     0,     7,     6,
        0,     0,     0,     0,     0,     0,     0,     0,   117,   116,
-      27,    26,    56,     0,    65,     0,    64,    13,     0,     0,
-       0,    33,    34,    35,    36,    48,    49,    50,    55,    51,
-      54,    52,    53,    32,    17,    39,    85,     0,     0,     0,
-       0,     0,    46,    31,    66,     0,     0,     0,     0,    70,
-       0,    12,     7,    11,    10,    82,     0,     0,    41,    40,
-      47,     0,     0,     0,    93,    21,     0,    76,     0,    84,
-      86,    83,    29,     0,     0,     0,     0,     0,   119,   118,
-       0,    75,     0,    60,     0,    21,     0,    79,    78,    77,
-      71,    72,     0,    74,     0,    73
+      32,    31,     0,   102,    93,     0,   101,    19,     0,     0,
+       0,     8,    59,    60,    61,    62,    56,    24,     0,     0,
+       0,     0,    85,    86,    87,    92,    88,    91,    89,    90,
+      33,     0,    67,    48,   103,     0,     0,     0,     0,    77,
+       0,    18,    13,    17,    16,    21,     0,     0,    58,    57,
+      68,     0,     0,     0,    84,    29,     0,   111,     0,    23,
+      25,    22,    46,     0,     0,     0,     0,     0,   119,   118,
+       0,   110,     0,   105,     0,    29,     0,   114,   113,   112,
+     106,   107,     0,   109,     0,   108
   };
 
   const short
   RSParserImpl::yypgoto_[] =
   {
-     -65,   -65,   -44,   155,   -65,   128,   -65,     4,   136,    95,
-      -8,    -6,    -9,   244,   109,   -65,     0,    -1,   -65,   -65,
-     -65,   258,    94,    17,   -65,   -65,   -65,    71,   -65,   -48,
-     108,   111,   285,   -65,   -65,   -65,   -65,   -65,   -65,   -64,
+     -58,   -58,   -58,   228,   -50,   178,   -58,   128,   -30,    93,
+      95,     4,   164,    -8,    -9,   -58,    -6,   107,   -58,   119,
+     -58,   249,     0,   -58,    94,    -4,   -58,   -58,    -2,   -58,
+     -58,   -58,   273,   -58,   -58,   -58,   -58,    86,   -58,   -57,
      -13
   };
 
   const short
   RSParserImpl::yydefgoto_[] =
   {
-      -1,    26,    27,    28,    83,    84,    29,    68,    31,    56,
-      32,    33,    34,    35,   114,   115,    60,    37,    38,    39,
-      40,    41,    73,    80,    42,    43,    44,   186,   187,   156,
-     157,   158,    61,    46,    47,    48,    49,    50,   109,   130,
+      -1,    26,    27,    56,    29,    30,    83,    84,   147,   148,
+     149,    68,    32,    33,    34,   116,    35,    60,    36,    95,
+      96,    37,    61,    39,    72,    80,    40,    41,    42,    43,
+      44,    45,    46,    47,    48,    49,    50,   186,   187,   130,
      201
   };
 
   const short
   RSParserImpl::yytable_[] =
   {
-      36,   116,    59,    57,    30,    58,   131,   118,   132,   -80,
-     134,   198,   198,    53,    69,   198,    54,   125,   126,    64,
-     128,   128,    72,    71,    78,    90,    91,    92,    93,    94,
-      95,    96,    97,    98,   -21,   -21,   -21,   -21,    65,   159,
-      74,    99,   100,   101,   102,   103,   104,   105,   106,   107,
-     108,    36,   119,    78,    78,    30,    85,   136,   164,   128,
-     137,   133,   122,   -80,    78,   199,   199,   127,   -80,   199,
-     200,   160,   129,   129,    12,    66,    72,    78,   -69,   -86,
-      67,   -18,   -18,   -18,   -18,   111,   138,   112,   198,    62,
-     145,   146,   147,   175,    74,   172,   112,   180,    90,    91,
-      92,   155,   128,   112,   148,   149,   150,   151,   152,   153,
-      -5,   129,   116,    86,    87,    88,    89,   161,    79,   104,
-     105,   106,   107,   108,   -20,   -20,   -20,   -20,   178,   203,
-     112,   110,   189,   169,   112,   170,   113,   117,   171,    36,
-      51,    52,   199,    30,    81,   124,    82,   120,   121,    87,
-      88,    89,   124,   128,   129,    92,   196,   197,   123,   177,
-     139,   133,   140,    90,    91,    92,   182,   183,    59,    57,
-      25,    58,   185,   135,   104,   105,   106,   107,   108,   113,
-     162,   193,   133,   124,   104,   105,   106,   107,   108,   210,
+      38,   118,    58,    57,    31,    59,    94,  -115,   150,   198,
+      81,   137,    82,   131,    69,   198,   133,   134,   128,    73,
+     128,    74,    53,    71,    78,    97,    98,    99,   100,   101,
+     102,   103,   104,   105,   198,   125,   126,   138,    92,    54,
+     151,   106,   107,   108,   109,   110,   111,   112,   113,   114,
+     115,    38,   119,    78,    78,    31,   -29,   -29,   -29,   -29,
+      85,  -115,   122,   199,    78,   164,  -115,   127,   200,   199,
+     129,   128,   129,    73,   198,    74,   -76,    78,   -25,   136,
+      91,    64,    92,   132,    97,    98,    99,   124,   199,   172,
+     173,   175,    82,   -26,   -26,   -26,   -26,   152,   153,   154,
+      65,   146,   128,    92,   180,   111,   112,   113,   114,   115,
+      66,   155,   156,   157,   158,   159,   160,   161,    79,    12,
+     139,    94,   140,   129,   -28,   -28,   -28,   -28,   199,    67,
+     128,    93,   169,    86,    62,   170,   203,   -11,   171,    38,
+      97,    98,    99,    31,    88,    89,    90,   120,   121,   178,
+     177,    92,   124,    25,   129,   189,    99,    92,   123,    51,
+      52,   111,   112,   113,   114,   115,   182,   183,    58,    57,
+     117,    59,   185,   196,   197,   111,   112,   113,   114,   115,
+     132,   193,   129,   162,   135,   132,    97,    98,    99,   210,
      166,   211,   202,   213,   167,   206,   207,   208,   204,   205,
-     173,   215,    82,   128,   185,   129,   104,   105,   106,   107,
-     108,    89,   214,   -44,   -44,   -44,   -44,   -44,   -44,   -44,
-     -44,   -44,   141,   142,   143,   144,    90,    91,    92,   -44,
-     -44,   -44,   -44,   -44,   -44,   -44,   -44,   -44,   -44,     1,
-       2,     3,     4,     5,     6,     7,     8,   104,   105,   106,
-     107,   108,   163,   176,   133,   129,     9,    10,    11,   181,
-     165,   -44,   133,    88,    89,   154,   212,    70,   174,   179,
-      63,   209,   192,    12,    13,    14,    15,    16,    17,    18,
-      19,    20,    21,    22,   190,    45,     0,   191,    23,     0,
+      93,   215,    90,   128,   185,   176,   124,   111,   112,   113,
+     114,   115,   214,   -65,   -65,   -65,   -65,   -65,   -65,   -65,
+     -65,   -65,   111,   112,   113,   114,   115,   212,    28,   -65,
+     -65,   -65,   -65,   -65,   -65,   -65,   -65,   -65,   -65,     1,
+       2,     3,     4,     5,     6,     7,     8,    87,    88,    89,
+      90,   142,   143,   144,   145,   129,     9,    10,    11,   181,
+     163,   -65,   132,   165,   141,   132,    89,    90,   174,   190,
+     179,   191,    70,    12,    13,    14,    15,    16,    17,    18,
+      19,    20,    21,    22,   192,    63,   209,     0,    23,     0,
       24,     0,    25,     1,    55,     3,     4,     5,     6,     7,
-       8,    90,    91,    92,     0,     0,     0,     0,     0,     0,
+       8,    97,    98,    99,     0,     0,     0,     0,     0,     0,
        9,    10,    11,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,   104,   105,   106,   107,   108,    12,    13,    14,
+       0,     0,   111,   112,   113,   114,   115,    12,    13,    14,
       15,    16,    17,    18,    19,    20,    21,    22,     0,     0,
        0,     0,    23,     0,    24,     1,    55,     3,     4,     5,
        6,     7,     8,     0,     0,     0,     0,     0,     0,     0,
        0,     0,     9,    10,    11,     0,     0,     0,     0,     0,
        0,     0,     0,     0,     0,     0,     0,     0,     0,    12,
       13,    14,    15,    16,    17,    18,    19,    20,    21,    22,
        0,     0,     0,     0,    23,     0,    24,   184,    55,     3,
@@ -1356,57 +1417,57 @@
        0,    12,    13,    14,    15,    16,    17,    18,    19,    20,
       21,    22,     0,     0,     0,     0,    23,     0,    24,     0,
        0,    12,    13,    14,    15,    16,    17,    18,    19,    20,
       21,    22,     0,     0,     0,     0,    77,     0,    24,     1,
       55,     3,    76,     5,     6,     7,     8,     0,     0,     0,
        0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
        0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
-      90,    91,    92,    12,    13,    14,    15,    16,    17,    18,
-      19,    20,    21,    22,    90,    91,    92,     0,    77,     0,
-      24,   104,   105,   106,   107,   108,     0,    90,    91,    92,
-       0,     0,    90,    91,    92,   104,   105,   106,   107,   108,
-       0,     0,     0,     0,     0,     0,     0,   168,   104,   105,
-     106,   107,   108,   104,   105,   106,   107,   108,     0,     0,
-       0,   188,     0,     0,    90,    91,    92,    93,    94,    95,
-      96,    97,    98,     0,   194,     0,     0,     0,     0,   195,
-      99,   100,   101,   102,   103,   104,   105,   106,   107,   108
+      97,    98,    99,    12,    13,    14,    15,    16,    17,    18,
+      19,    20,    21,    22,    97,    98,    99,     0,    77,     0,
+      24,   111,   112,   113,   114,   115,     0,    97,    98,    99,
+       0,     0,    97,    98,    99,   111,   112,   113,   114,   115,
+       0,     0,     0,     0,     0,     0,     0,   168,   111,   112,
+     113,   114,   115,   111,   112,   113,   114,   115,     0,     0,
+       0,   188,     0,     0,    97,    98,    99,   100,   101,   102,
+     103,   104,   105,     0,   194,     0,     0,     0,     0,   195,
+     106,   107,   108,   109,   110,   111,   112,   113,   114,   115
   };
 
   const short
   RSParserImpl::yycheck_[] =
   {
-       0,    49,    11,    11,     0,    11,    70,    51,    72,     1,
-      74,     1,     1,    56,    23,     1,    56,    65,    66,    56,
-       1,     1,    23,    23,    24,    11,    12,    13,    14,    15,
-      16,    17,    18,    19,    23,    24,    25,    26,    54,    27,
-      23,    27,    28,    29,    30,    31,    32,    33,    34,    35,
-      36,    51,    52,    53,    54,    51,     0,    55,   122,     1,
-       1,    59,    62,    55,    64,    55,    55,    67,    60,    55,
-      60,    59,    53,    53,    37,    54,    77,    77,    59,    59,
-      54,    23,    24,    25,    26,     1,    27,     3,     1,    52,
-      90,    91,    92,   157,    77,   139,     3,   161,    11,    12,
-      13,     1,     1,     3,   104,   105,   106,   107,   108,   109,
-       0,    53,   160,    23,    24,    25,    26,   117,    24,    32,
-      33,    34,    35,    36,    23,    24,    25,    26,     1,   193,
-       3,    48,     1,   133,     3,   135,    52,    52,   138,   139,
-      48,    49,    55,   139,     1,    52,     3,    53,    54,    24,
-      25,    26,    52,     1,    53,    13,    50,    51,    64,   159,
-      57,    59,    59,    11,    12,    13,   166,   167,   177,   177,
-      56,   177,   168,    27,    32,    33,    34,    35,    36,    52,
-      57,   181,    59,    52,    32,    33,    34,    35,    36,   202,
+       0,    51,    11,    11,     0,    11,    36,     1,    27,     1,
+       1,     1,     3,    70,    23,     1,    73,    74,     1,    23,
+       1,    23,    56,    23,    24,    11,    12,    13,    14,    15,
+      16,    17,    18,    19,     1,    65,    66,    27,     3,    56,
+      59,    27,    28,    29,    30,    31,    32,    33,    34,    35,
+      36,    51,    52,    53,    54,    51,    23,    24,    25,    26,
+       0,    55,    62,    55,    64,   122,    60,    67,    60,    55,
+      53,     1,    53,    77,     1,    77,    59,    77,    59,    55,
+       1,    56,     3,    59,    11,    12,    13,    52,    55,   139,
+       1,   148,     3,    23,    24,    25,    26,    97,    98,    99,
+      54,     1,     1,     3,   161,    32,    33,    34,    35,    36,
+      54,   111,   112,   113,   114,   115,   116,   117,    24,    37,
+      57,   151,    59,    53,    23,    24,    25,    26,    55,    54,
+       1,    52,   132,    48,    52,   135,   193,     0,   138,   139,
+      11,    12,    13,   139,    24,    25,    26,    53,    54,     1,
+     150,     3,    52,    56,    53,     1,    13,     3,    64,    48,
+      49,    32,    33,    34,    35,    36,   166,   167,   177,   177,
+      52,   177,   168,    50,    51,    32,    33,    34,    35,    36,
+      59,   181,    53,    57,    27,    59,    11,    12,    13,   202,
       27,   204,   188,   206,    50,   195,   196,   197,   194,   195,
-       1,   214,     3,     1,   200,    53,    32,    33,    34,    35,
-      36,    26,   212,    11,    12,    13,    14,    15,    16,    17,
-      18,    19,    86,    87,    88,    89,    11,    12,    13,    27,
+      52,   214,    26,     1,   200,    59,    52,    32,    33,    34,
+      35,    36,   212,    11,    12,    13,    14,    15,    16,    17,
+      18,    19,    32,    33,    34,    35,    36,    58,     0,    27,
       28,    29,    30,    31,    32,    33,    34,    35,    36,     3,
-       4,     5,     6,     7,     8,     9,    10,    32,    33,    34,
-      35,    36,    57,    59,    59,    53,    20,    21,    22,    52,
-      57,    59,    59,    25,    26,   110,    58,    23,   140,   160,
-      12,   200,   177,    37,    38,    39,    40,    41,    42,    43,
-      44,    45,    46,    47,   176,     0,    -1,   176,    52,    -1,
+       4,     5,     6,     7,     8,     9,    10,    23,    24,    25,
+      26,    87,    88,    89,    90,    53,    20,    21,    22,    52,
+      57,    59,    59,    57,    86,    59,    25,    26,   140,   176,
+     151,   176,    23,    37,    38,    39,    40,    41,    42,    43,
+      44,    45,    46,    47,   177,    12,   200,    -1,    52,    -1,
       54,    -1,    56,     3,     4,     5,     6,     7,     8,     9,
       10,    11,    12,    13,    -1,    -1,    -1,    -1,    -1,    -1,
       20,    21,    22,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
       -1,    -1,    32,    33,    34,    35,    36,    37,    38,    39,
       40,    41,    42,    43,    44,    45,    46,    47,    -1,    -1,
       -1,    -1,    52,    -1,    54,     3,     4,     5,     6,     7,
        8,     9,    10,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
@@ -1431,156 +1492,157 @@
       -1,    -1,    -1,    -1,    -1,    -1,    -1,    58,    32,    33,
       34,    35,    36,    32,    33,    34,    35,    36,    -1,    -1,
       -1,    58,    -1,    -1,    11,    12,    13,    14,    15,    16,
       17,    18,    19,    -1,    58,    -1,    -1,    -1,    -1,    58,
       27,    28,    29,    30,    31,    32,    33,    34,    35,    36
   };
 
-  const unsigned char
+  const signed char
   RSParserImpl::yystos_[] =
   {
        0,     3,     4,     5,     6,     7,     8,     9,    10,    20,
       21,    22,    37,    38,    39,    40,    41,    42,    43,    44,
-      45,    46,    47,    52,    54,    56,    62,    63,    64,    67,
-      68,    69,    71,    72,    73,    74,    77,    78,    79,    80,
-      81,    82,    85,    86,    87,    93,    94,    95,    96,    97,
-      98,    48,    49,    56,    56,     4,    70,    71,    72,    73,
-      77,    93,    52,    82,    56,    54,    54,    54,    68,    73,
-      74,    77,    78,    83,    84,     3,     6,    52,    77,    83,
-      84,     1,     3,    65,    66,     0,    23,    24,    25,    26,
-      11,    12,    13,    14,    15,    16,    17,    18,    19,    27,
-      28,    29,    30,    31,    32,    33,    34,    35,    36,    99,
-      48,     1,     3,    52,    75,    76,    90,    52,    63,    77,
-      83,    83,    77,    83,    52,    90,    90,    77,     1,    53,
-     100,   100,   100,    59,   100,    27,    55,     1,    27,    57,
-      59,    69,    69,    69,    69,    77,    77,    77,    77,    77,
-      77,    77,    77,    77,    64,     1,    90,    91,    92,    27,
-      59,    77,    57,    57,   100,    57,    27,    50,    58,    77,
-      77,    77,    63,     1,    66,   100,    59,    77,     1,    75,
-     100,    52,    77,    77,     3,    68,    88,    89,    58,     1,
-      91,    92,    70,    77,    58,    58,    50,    51,     1,    55,
-      60,   101,    68,   100,    68,    68,    77,    77,    77,    88,
-     101,   101,    58,   101,    77,   101
+      45,    46,    47,    52,    54,    56,    62,    63,    64,    65,
+      66,    72,    73,    74,    75,    77,    79,    82,    83,    84,
+      87,    88,    89,    90,    91,    92,    93,    94,    95,    96,
+      97,    48,    49,    56,    56,     4,    64,    74,    75,    77,
+      78,    83,    52,    93,    56,    54,    54,    54,    72,    75,
+      82,    83,    85,    86,    89,     3,     6,    52,    83,    85,
+      86,     1,     3,    67,    68,     0,    48,    23,    24,    25,
+      26,     1,     3,    52,    69,    80,    81,    11,    12,    13,
+      14,    15,    16,    17,    18,    19,    27,    28,    29,    30,
+      31,    32,    33,    34,    35,    36,    76,    52,    65,    83,
+      85,    85,    83,    85,    52,    69,    69,    83,     1,    53,
+     100,   100,    59,   100,   100,    27,    55,     1,    27,    57,
+      59,    66,    73,    73,    73,    73,     1,    69,    70,    71,
+      27,    59,    83,    83,    83,    83,    83,    83,    83,    83,
+      83,    83,    57,    57,   100,    57,    27,    50,    58,    83,
+      83,    83,    65,     1,    68,   100,    59,    83,     1,    80,
+     100,    52,    83,    83,     3,    72,    98,    99,    58,     1,
+      70,    71,    78,    83,    58,    58,    50,    51,     1,    55,
+      60,   101,    72,   100,    72,    72,    83,    83,    83,    98,
+     101,   101,    58,   101,    83,   101
   };
 
-  const unsigned char
+  const signed char
   RSParserImpl::yyr1_[] =
   {
-       0,    61,    62,    62,    62,    63,    63,    64,    64,    65,
-      65,    65,    66,    66,    67,    67,    67,    67,    68,    68,
-      68,    69,    69,    70,    70,    70,    71,    71,    72,    72,
-      72,    72,    73,    74,    74,    74,    74,    75,    75,    75,
-      76,    76,    77,    77,    77,    77,    77,    77,    78,    78,
-      78,    78,    78,    78,    78,    78,    78,    79,    79,    79,
-      79,    79,    79,    79,    80,    81,    82,    82,    83,    83,
-      84,    85,    85,    86,    86,    87,    88,    88,    89,    89,
-      89,    90,    90,    91,    91,    92,    92,    93,    93,    94,
-      94,    94,    95,    95,    96,    96,    96,    97,    97,    98,
-      98,    98,    98,    98,    98,    99,    99,    99,    99,    99,
-      99,    99,    99,    99,    99,    99,   100,   100,   101,   101
+       0,    61,    62,    62,    62,    63,    63,    63,    63,    64,
+      64,    65,    65,    66,    66,    67,    67,    67,    68,    68,
+      69,    69,    70,    70,    71,    71,    72,    72,    72,    73,
+      73,    74,    74,    75,    76,    76,    76,    76,    76,    76,
+      76,    76,    76,    76,    76,    77,    77,    77,    77,    78,
+      78,    78,    79,    79,    80,    80,    80,    81,    81,    82,
+      82,    82,    82,    83,    83,    83,    83,    83,    83,    84,
+      84,    84,    84,    84,    84,    85,    85,    86,    87,    87,
+      87,    88,    88,    88,    88,    89,    89,    89,    89,    89,
+      89,    89,    89,    89,    90,    90,    90,    90,    90,    90,
+      90,    91,    92,    93,    93,    94,    95,    95,    96,    96,
+      97,    98,    98,    99,    99,    99,   100,   100,   101,   101
   };
 
-  const unsigned char
+  const signed char
   RSParserImpl::yyr2_[] =
   {
-       0,     2,     1,     1,     1,     1,     1,     4,     2,     1,
-       3,     3,     3,     2,     2,     3,     3,     3,     1,     1,
-       1,     1,     1,     1,     1,     1,     3,     3,     2,     5,
-       2,     4,     3,     3,     3,     3,     3,     1,     1,     2,
-       3,     3,     1,     1,     1,     1,     4,     4,     3,     3,
-       3,     3,     3,     3,     3,     3,     3,     1,     1,     1,
-       7,     1,     1,     1,     3,     3,     4,     2,     1,     1,
-       3,     7,     8,    10,     8,     6,     1,     3,     3,     3,
-       1,     1,     3,     3,     3,     1,     1,     1,     1,     1,
-       1,     1,     1,     1,     1,     1,     1,     1,     1,     1,
-       1,     1,     1,     1,     1,     1,     1,     1,     1,     1,
-       1,     1,     1,     1,     1,     1,     1,     1,     1,     1
+       0,     2,     1,     1,     1,     2,     3,     3,     3,     1,
+       1,     1,     1,     4,     2,     1,     3,     3,     3,     2,
+       1,     3,     3,     3,     1,     1,     1,     1,     1,     1,
+       1,     3,     3,     3,     1,     1,     1,     1,     1,     1,
+       1,     1,     1,     1,     1,     2,     5,     2,     4,     1,
+       1,     1,     1,     1,     1,     1,     2,     3,     3,     3,
+       3,     3,     3,     1,     1,     1,     1,     4,     4,     1,
+       1,     1,     1,     1,     1,     1,     1,     3,     1,     1,
+       1,     1,     1,     1,     1,     3,     3,     3,     3,     3,
+       3,     3,     3,     3,     1,     1,     1,     1,     1,     1,
+       1,     3,     3,     4,     2,     7,     7,     8,    10,     8,
+       6,     1,     3,     3,     3,     1,     1,     1,     1,     1
   };
 
 
-
+#if YYDEBUG || 1
   // YYTNAME[SYMBOL-NUM] -- String name of the symbol SYMBOL-NUM.
-  // First, the terminals, then, starting at \a yyntokens_, nonterminals.
+  // First, the terminals, then, starting at \a YYNTOKENS, nonterminals.
   const char*
   const RSParserImpl::yytname_[] =
   {
-  "$end", "error", "$undefined", "LOCAL", "GLOBAL", "FUNCTION",
-  "PREDICATE", "RADICAL", "INTEGER", "INFINITY", "EMPTYSET", "PLUS",
-  "MINUS", "MULTIPLY", "GREATER", "LESSER", "GREATER_OR_EQ",
+  "\"end of file\"", "error", "\"invalid token\"", "LOCAL", "GLOBAL",
+  "FUNCTION", "PREDICATE", "RADICAL", "INTEGER", "INTSET", "EMPTYSET",
+  "PLUS", "MINUS", "MULTIPLY", "GREATER", "LESSER", "GREATER_OR_EQ",
   "LESSER_OR_EQ", "EQUAL", "NOTEQUAL", "FORALL", "EXISTS", "NOT",
   "EQUIVALENT", "IMPLICATION", "OR", "AND", "IN", "NOTIN", "SUBSET",
-  "SUBOR_EQ", "NOTSUBSET", "DECART", "UNION", "INTERSECTION", "SET_MINUS",
-  "SYMMINUS", "BOOLEAN", "BIGPR", "SMALLPR", "FILTER", "CARD", "BOOL",
-  "DEBOOL", "RED", "DECLARATIVE", "RECURSIVE", "IMPERATIVE", "DEFINE",
-  "STRUCT", "ASSIGN", "ITERATE", "LP", "RP", "LC", "RC", "LS", "RS", "BAR",
-  "COMMA", "SEMICOLON", "$accept", "expression", "term_or_logic",
-  "function_decl", "arg_declaration", "declaration", "global_declaration",
-  "logic", "logic_all", "logic_no_binary", "logic_par", "logic_unary",
-  "logic_predicates", "logic_binary", "quant_var", "quant_var_enum",
-  "term", "binary_operation", "typed_constructors", "enumeration", "tuple",
-  "boolean", "term_enum", "term_enum_min2", "declarative", "recursion",
-  "imperative", "imp_blocks", "imp_block", "variable", "var_enum",
-  "var_all", "function_name", "global_id", "identifier", "literal",
-  "quantifier", "operation_name", "binary_predicate", "RPE", "RCE", YY_NULLPTR
+  "SUBSET_OR_EQ", "NOTSUBSET", "DECART", "UNION", "INTERSECTION",
+  "SET_MINUS", "SYMMINUS", "BOOLEAN", "BIGPR", "SMALLPR", "FILTER", "CARD",
+  "BOOL", "DEBOOL", "RED", "DECLARATIVE", "RECURSIVE", "IMPERATIVE",
+  "DEFINE", "STRUCT", "ASSIGN", "ITERATE", "LP", "RP", "LC", "RC", "LS",
+  "RS", "BAR", "COMMA", "SEMICOLON", "$accept", "expression",
+  "global_declaration", "function_name", "logic_or_setexpr",
+  "function_decl", "arguments", "declaration", "variable", "var_enum",
+  "var_all", "logic", "logic_all", "logic_par", "logic_predicates",
+  "binary_predicate", "logic_unary", "logic_no_binary", "quantifier",
+  "quant_var", "quant_var_enum", "logic_binary", "setexpr",
+  "operation_name", "setexpr_enum", "setexpr_enum_min2", "literal",
+  "identifier", "setexpr_binary", "setexpr_generators", "enumeration",
+  "tuple", "boolean", "filter_expression", "declarative", "recursion",
+  "imperative", "imp_blocks", "imp_block", "RPE", "RCE", YY_NULLPTR
   };
+#endif
+
 
 #if YYDEBUG
-  const unsigned short
+  const short
   RSParserImpl::yyrline_[] =
   {
-       0,   150,   150,   151,   152,   155,   156,   159,   160,   163,
-     164,   165,   167,   168,   172,   173,   174,   175,   179,   180,
-     181,   183,   184,   186,   187,   188,   190,   191,   193,   194,
-     196,   197,   199,   201,   202,   203,   204,   207,   208,   209,
-     211,   212,   216,   217,   218,   219,   220,   221,   224,   225,
-     226,   227,   228,   229,   230,   231,   232,   235,   236,   237,
-     238,   239,   240,   241,   243,   245,   247,   248,   250,   251,
-     253,   255,   256,   259,   261,   264,   266,   267,   269,   270,
-     271,   273,   274,   276,   277,   279,   280,   284,   285,   287,
-     288,   289,   291,   292,   294,   295,   296,   299,   300,   303,
-     304,   305,   306,   307,   308,   311,   312,   313,   314,   315,
-     316,   317,   318,   319,   320,   321,   324,   325,   327,   328
+       0,   262,   262,   263,   264,   268,   269,   270,   271,   274,
+     275,   279,   280,   284,   285,   290,   291,   292,   295,   296,
+     300,   301,   304,   305,   308,   309,   314,   315,   316,   319,
+     320,   323,   324,   328,   331,   332,   333,   334,   335,   336,
+     337,   338,   339,   340,   341,   345,   346,   347,   348,   351,
+     352,   353,   356,   357,   360,   361,   362,   365,   366,   370,
+     371,   372,   373,   379,   380,   381,   382,   383,   384,   387,
+     388,   389,   390,   391,   392,   395,   396,   399,   403,   404,
+     405,   409,   410,   411,   412,   416,   417,   418,   419,   420,
+     421,   422,   423,   424,   428,   429,   430,   431,   432,   433,
+     434,   437,   440,   443,   444,   447,   451,   452,   455,   456,
+     459,   462,   463,   466,   467,   468,   474,   475,   478,   479
   };
 
-  // Print the state stack on the debug stream.
   void
-  RSParserImpl::yystack_print_ ()
+  RSParserImpl::yy_stack_print_ () const
   {
     *yycdebug_ << "Stack now";
     for (stack_type::const_iterator
            i = yystack_.begin (),
            i_end = yystack_.end ();
          i != i_end; ++i)
-      *yycdebug_ << ' ' << i->state;
+      *yycdebug_ << ' ' << int (i->state);
     *yycdebug_ << '\n';
   }
 
-  // Report on the debug stream that the rule \a yyrule is going to be reduced.
   void
-  RSParserImpl::yy_reduce_print_ (int yyrule)
+  RSParserImpl::yy_reduce_print_ (int yyrule) const
   {
-    unsigned yylno = yyrline_[yyrule];
+    int yylno = yyrline_[yyrule];
     int yynrhs = yyr2_[yyrule];
     // Print the symbols being reduced, and their result.
     *yycdebug_ << "Reducing stack by rule " << yyrule - 1
                << " (line " << yylno << "):\n";
     // The symbols being reduced.
     for (int yyi = 0; yyi < yynrhs; yyi++)
       YY_SYMBOL_PRINT ("   $" << yyi + 1 << " =",
                        yystack_[(yynrhs) - (yyi + 1)]);
   }
 #endif // YYDEBUG
 
-  RSParserImpl::token_number_type
+  RSParserImpl::symbol_kind_type
   RSParserImpl::yytranslate_ (int t)
   {
     // YYTRANSLATE[TOKEN-NUM] -- Symbol number corresponding to
     // TOKEN-NUM as returned by yylex.
     static
-    const token_number_type
+    const signed char
     translate_table[] =
     {
        0,     2,     2,     2,     2,     2,     2,     2,     2,     2,
        2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
        2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
        2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
        2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
@@ -1608,29 +1670,30 @@
        5,     6,     7,     8,     9,    10,    11,    12,    13,    14,
       15,    16,    17,    18,    19,    20,    21,    22,    23,    24,
       25,    26,    27,    28,    29,    30,    31,    32,    33,    34,
       35,    36,    37,    38,    39,    40,    41,    42,    43,    44,
       45,    46,    47,    48,    49,    50,    51,    52,    53,    54,
       55,    56,    57,    58,    59,    60
     };
-    const unsigned user_token_number_max_ = 315;
-    const token_number_type undef_token_ = 2;
+    // Last valid token kind.
+    const int code_max = 315;
 
-    if (static_cast<int> (t) <= yyeof_)
-      return yyeof_;
-    else if (static_cast<unsigned> (t) <= user_token_number_max_)
-      return translate_table[t];
+    if (t <= 0)
+      return symbol_kind::S_YYEOF;
+    else if (t <= code_max)
+      return YY_CAST (symbol_kind_type, translate_table[t]);
     else
-      return undef_token_;
+      return symbol_kind::S_YYUNDEF;
   }
 
-#line 11 "RSParserImpl.y" // lalr1.cc:1242
+#line 15 "RSParserImpl.y"
 } } } // ccl::rslang::detail
-#line 1629 "RSParserImpl.cpp" // lalr1.cc:1242
-#line 331 "RSParserImpl.y" // lalr1.cc:1243
+#line 1691 "RSParserImpl.cpp"
+
+#line 486 "RSParserImpl.y"
 
 
 #ifdef _MSC_VER
   #pragma warning( pop )
 #endif
 
 #ifdef __clang__
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/RSToken.cpp` & `pyconcept-0.1.3/ccl/rslang/src/RSToken.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/SDImplementation.cpp` & `pyconcept-0.1.3/ccl/rslang/src/SDImplementation.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,16 @@
   return SDIterator{ Iterator(*this, true) };
 }
 
 bool SDPowerSet::Contains(StructuredData element) const {
   return element.B().IsSubsetOrEq(base.B());
 }
 
-SDDecartian::Iterator::Iterator(const SDDecartian& decart, const bool completed)
-  : decartian{ &decart }, isCompleted{ completed || decartian->Cardinality() == 0 } {
+SDDecartian::Iterator::Iterator(const SDDecartian& base, const bool completed)
+  : decartian{ &base }, isCompleted{ completed || base.Cardinality() == 0 } {
   if (!isCompleted) {
     componentIters.reserve(size(decartian->factors));
     for (const auto& factor : decartian->factors) {
       componentIters.emplace_back(std::begin(factor.B()));
     }
   }
 }
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/SDataCompact.cpp` & `pyconcept-0.1.3/ccl/rslang/src/SDataCompact.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #include "ccl/rslang/SDataCompact.h"
 
 #include "ccl/rslang/RSToken.h"
+#include "ccl/rslang/Typification.h"
+#include "ccl/rslang/StructuredData.h"
+
+#include <optional>
 
 namespace ccl::object {
 
 namespace {
 
 using rslang::Typification;
 
@@ -55,15 +59,15 @@
   Header result{};
   const auto visitor = [&](const Typification& host) {
     switch (host.Structure()) {
     case rslang::StructureType::basic:
       result.push_back(host.E().baseID); break;
 
     case rslang::StructureType::collection:
-      result.push_back("B"); break;
+      result.emplace_back("B"); break;
 
     case rslang::StructureType::tuple:
       break;
     }
   };
   type.ConstVisit(visitor);
   return result;
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/StructuredData.cpp` & `pyconcept-0.1.3/ccl/rslang/src/StructuredData.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/src/SyntaxTree.cpp` & `pyconcept-0.1.3/ccl/rslang/src/SyntaxTree.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -219,16 +219,16 @@
   if (!root->pos.Contains(range)) {
     return std::nullopt;
   } else if (root.ChildrenCount() == 0) {
     return root;
   } else {
     root.MoveToChild(0);
     do {
-      if (const auto result = FindMinimalNode(root, range); 
-          result.has_value()) {
+      const auto result = FindMinimalNode(root, range);
+      if (result.has_value()) {
         return result;
       }
     } while (root.MoveToNextSibling());
     root.MoveToParent();
     return root;
   }
 }
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/TypeAuditor.cpp` & `pyconcept-0.1.3/ccl/rslang/src/TypeAuditor.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 [[nodiscard]] std::string ToString(const ExpressionType& type) noexcept(false);
 [[nodiscard]] constexpr bool IsSubset(TokenID token) noexcept;
 [[nodiscard]] bool IsEchelon(SyntaxTree::Cursor iter);
 [[nodiscard]] bool IsEchelon(SyntaxTree::Cursor iter, Index index);
 void MangleRadicals(const std::string& funcName, Typification& type);
 
 std::string ToString(const ExpressionType& type) noexcept(false) {
-  return std::visit(meta::Overloads{
-    [](const Typification& t) { return t.ToString();  },
-    [](const LogicT& /*t*/) { return std::string{"LOGIC"}; },
-                    }, type);
+  return std::visit(
+    meta::Overloads{
+      [](const Typification& t) { return t.ToString();  },
+      [](const LogicT& /*t*/) { return std::string{"LOGIC"}; },
+    }
+    , type);
 }
 
 constexpr bool IsSubset(const TokenID token) noexcept {
   return token == TokenID::SUBSET
     || token == TokenID::SUBSET_OR_EQ
     || token == TokenID::NOTSUBSET;
 }
@@ -113,21 +115,33 @@
     return AreCompatible(std::get<Typification>(type1), std::get<Typification>(type2));
   }
 }
 
 bool TypeEnv::AreCompatible(const Typification& type1, const Typification& type2) const {
   if (type1 == type2) {
     return true;
-  } else if (type1.Structure() != type2.Structure()) {
+  } 
+  
+  const auto struct1 = type1.Structure();
+  const auto struct2 = type2.Structure();
+  
+  if (struct1 == rslang::StructureType::basic && type1.E().baseID == Typification::anyTypificationName) {
+    return true;
+  }
+  if (struct2 == rslang::StructureType::basic && type2.E().baseID == Typification::anyTypificationName) {
+    return true;
+  }
+  if (struct1 != struct2) {
     return false;
   }
-  switch (type1.Structure()) {
+
+  switch (struct1) {
   default:
   case rslang::StructureType::basic: return CommonType(type1, type2) != nullptr;
-  case rslang::StructureType::collection:  return AreCompatible(type1.B().Base(), type2.B().Base());
+  case rslang::StructureType::collection: return AreCompatible(type1.B().Base(), type2.B().Base());
   case rslang::StructureType::tuple: {
     if (type1.T().Arity() != type2.T().Arity()) {
       return false;
     } else {
       for (auto index = Typification::PR_START; index < type1.T().Arity() + Typification::PR_START; ++index) {
         if (!AreCompatible(type1.T().Component(index), type2.T().Component(index))) {
           return false;
@@ -138,105 +152,124 @@
   }
   }
 }
 
 std::optional<Typification> TypeEnv::Merge(const Typification& type1, const Typification& type2) const {
   if (type1 == type2) {
     return type1;
-  } else if (type1.Structure() != type2.Structure()) {
+  }
+  if (type1.Structure() != type2.Structure()) {
     return std::nullopt;
   }
-  switch (type1.Structure()) {
+
+  const auto struct1 = type1.Structure();
+  const auto struct2 = type2.Structure();
+
+  if (struct1 == rslang::StructureType::basic && type1.E().baseID == Typification::anyTypificationName) {
+    return type2;
+  }
+  if (struct2 == rslang::StructureType::basic && type2.E().baseID == Typification::anyTypificationName) {
+    return type1;
+  }
+
+  switch (struct1) {
   default:
-  case rslang::StructureType::basic: {
-    if (const auto* type = CommonType(type1, type2); type == nullptr) {
-      return std::nullopt;
-    } else {
+    case rslang::StructureType::basic: {
+      const auto* type = CommonType(type1, type2);
+      if (type == nullptr) {
+        return std::nullopt;
+      }
       return *type;
     }
-  }
-  case rslang::StructureType::collection: {
-    if (auto base = Merge(type1.B().Base(), type2.B().Base()); !base.has_value()) {
-      return std::nullopt;
-    } else {
+    case rslang::StructureType::collection: {
+      auto base = Merge(type1.B().Base(), type2.B().Base());
+      if (!base.has_value()) {
+        return std::nullopt;
+      }
       return base.value().ApplyBool();
     }
-  }
-  case rslang::StructureType::tuple: {
-    if (type1.T().Arity() != type2.T().Arity()) {
-      return std::nullopt;
-    } else {
+    case rslang::StructureType::tuple: {
+      if (type1.T().Arity() != type2.T().Arity()) {
+        return std::nullopt;
+      }
       std::vector<Typification> components{};
-      for (auto index = Typification::PR_START; index < type1.T().Arity() + Typification::PR_START; ++index) {
-        if (auto component = Merge(type1.T().Component(index), type2.T().Component(index));
-            !component.has_value()) {
+      const auto maxIndex = Typification::PR_START + type1.T().Arity();
+      for (auto index = Typification::PR_START; index < maxIndex; ++index) {
+        auto component = Merge(type1.T().Component(index), type2.T().Component(index));
+        if (!component.has_value()) {
           return std::nullopt;
-        } else {
-          components.emplace_back(std::move(component.value()));
         }
+        components.emplace_back(std::move(component.value()));
       }
       return Typification::Tuple(components);
     }
   }
-  }
 }
 
 bool TypeEnv::CompareTemplated(
   Typification::Substitutes& substitutes,
   const Typification& arg,
   const Typification& value
 ) {
   if (arg == value) {
     return true;
   }
   if (arg.IsElement() && IsRadical(arg.E().baseID)) {
-    if (const auto& base = arg.E().baseID; !substitutes.contains(base)) {
+    const auto& base = arg.E().baseID;
+    if (!substitutes.contains(base)) {
       substitutes.insert({ base, value });
       return true;
-    } else if (auto mergeType = Merge(substitutes.at(base), value);
-               !mergeType.has_value()) {
+    }
+
+    auto mergeType = Merge(substitutes.at(base), value);
+    if (!mergeType.has_value()) {
       return false;
-    } else {
-      substitutes.at(base) = std::move(mergeType.value());
-      return true;
     }
+    substitutes.at(base) = std::move(mergeType.value());
+    return true;
   } else if (arg.Structure() != value.Structure()) {
     return false;
   } else {
     switch (arg.Structure()) {
-    default:
-    case rslang::StructureType::basic: return CommonType(arg, value) != nullptr;
-    case rslang::StructureType::collection:  return CompareTemplated(substitutes, arg.B().Base(), value.B().Base());
-    case rslang::StructureType::tuple: {
-      if (arg.T().Arity() != value.T().Arity()) {
-        return false;
-      } else {
-        for (auto index = Typification::PR_START; index < arg.T().Arity() + Typification::PR_START; ++index) {
+      default:
+      case rslang::StructureType::basic:
+        return CommonType(arg, value) != nullptr;
+      case rslang::StructureType::collection:
+        return CompareTemplated(substitutes, arg.B().Base(), value.B().Base());
+      case rslang::StructureType::tuple: {
+        if (arg.T().Arity() != value.T().Arity()) {
+          return false;
+        }
+        const auto maxIndex = Typification::PR_START + arg.T().Arity();
+        for (auto index = Typification::PR_START; index < maxIndex; ++index) {
           if (!CompareTemplated(substitutes, arg.T().Component(index), value.T().Component(index))) {
             return false;
           }
         }
         return true;
       }
     }
-    }
   }
 }
 
 } // namespace details
 
 bool TypeAuditor::CheckType(const rslang::SyntaxTree& tree) {
   Clear();
   return tree.Root().DispatchVisit(*this);
 }
 
 const ExpressionType& TypeAuditor::GetType() const noexcept {
   return currentType;
 }
 
+void TypeAuditor::SetExepectTypification(const bool value) noexcept {
+  isTypification = value;
+}
+
 void TypeAuditor::OnError(const SemanticEID eid, const StrPos position) {
   if (reporter.has_value()) {
     reporter.value()(Error{ static_cast<uint32_t>(eid), position });
   }
 }
 
 void TypeAuditor::OnError(const SemanticEID eid, const StrPos position, std::string param) {
@@ -266,52 +299,67 @@
 
 bool TypeAuditor::ViGlobalDefinition(Cursor iter) {
   const auto childrenCount = iter.ChildrenCount();
   if (iter->id == TokenID::PUNC_STRUCT) {
     if (childrenCount != 2 || !IsEchelon(iter, 1)) {
       OnError(SemanticEID::globalStructure, iter(0).pos.finish);
       return false;
-    } else if (const auto maybeType = ChildType(iter, 1); !maybeType.has_value()) {
+    }
+    const auto maybeType = ChildType(iter, 1);
+    if (!maybeType.has_value()) {
       return false;
-    } else if (const auto& type = std::get<Typification>(maybeType.value()); !type.IsCollection()) {
+    } 
+    
+    const auto& type = std::get<Typification>(maybeType.value());
+    if (!type.IsCollection()) {
       return false;
-    } else {
-      return VisitAndReturn(type.B().Base());
     }
+    return VisitAndReturn(type.B().Base());
   } else {
     assert(iter->id == TokenID::PUNC_DEFINE);
     if (childrenCount == 1) {
       return VisitAndReturn(Typification{ iter(0).data.ToText() }.ApplyBool());
-    } else if (const auto type = ChildType(iter, 1); !type.has_value()) {
+    } 
+    
+    const auto type = ChildType(iter, 1);
+    if (!type.has_value()) {
         return false;
-    } else {
-      return VisitAndReturn(type.value());
     }
+    return VisitAndReturn(type.value());
   }
 }
 
 bool TypeAuditor::ViFunctionDefinition(Cursor iter) {
-  if (const auto guard = isFuncDeclaration.CreateGuard(); !VisitChild(iter, 0)) {
-    return false;
+  {
+    const auto guard = isFuncDeclaration.CreateGuard();
+    if (!VisitChild(iter, 0)) {
+      return false;
+    }
   }
+
   for (auto n : functionArgsID) {
     functionArgs.emplace_back(localVars.at(n).arg);
   }
-  if (const auto type = ChildType(iter, 1); !type.has_value()) {
+
+  const auto type = ChildType(iter, 1);
+  if (!type.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(type.value());
   }
+  return VisitAndReturn(type.value());
 }
 
 bool TypeAuditor::ViFunctionCall(Cursor iter) {
   const auto& funcName = iter(0).data.ToText();
   const auto* funcType = env.context.TypeFor(funcName);
   if (funcType == nullptr) {
-    OnError(SemanticEID::globalNotTyped, iter->pos.start, funcName);
+    OnError(
+      SemanticEID::globalNotTyped,
+      iter->pos.start,
+      funcName
+    );
     return false;
   }
   const auto substitutes = CheckFuncArguments(iter, funcName);
   if (!substitutes.has_value()) {
     return false;
   }
   if (!std::holds_alternative<Typification>(*funcType)) {
@@ -325,21 +373,26 @@
     return VisitAndReturn(fixedType);
   }
 }
 
 std::optional<Typification::Substitutes> TypeAuditor::CheckFuncArguments(Cursor iter, const std::string& funcName) {
   const auto* args = env.context.FunctionArgsFor(funcName);
   if (args == nullptr) {
-    OnError(SemanticEID::globalFuncMissing, iter(0).pos.start, iter(0).data.ToText());
+    OnError(
+      SemanticEID::globalFuncMissing,
+      iter(0).pos.start,
+      iter(0).data.ToText()
+    );
     return std::nullopt;
   }
   const auto expectedArguments = iter.ChildrenCount() - 1;
-  if (const auto argCount = static_cast<Index>(ssize(*args)); argCount != expectedArguments) {
+  const auto argCount = static_cast<Index>(ssize(*args));
+  if (argCount != expectedArguments) {
     OnError(
-      SemanticEID::invalidArgsArtity,
+      SemanticEID::invalidArgsArity,
       iter(1).pos.start,
       { std::to_string(expectedArguments), std::to_string(argCount) }
     );
     return std::nullopt;
   }
 
   Typification::Substitutes substitutes{};
@@ -347,65 +400,81 @@
     const auto childType = ChildType(iter, child);
     if (!childType.has_value() || !std::holds_alternative<Typification>(childType.value())) {
       return std::nullopt;
     }
     Typification argType = args->at(static_cast<size_t>(child) - 1).type;
     MangleRadicals(funcName, argType);
     if (!env.CompareTemplated(substitutes, argType, std::get<Typification>(childType.value()))) {
-      OnError(SemanticEID::invalidArgumentType, iter(child).pos.start, argType, childType.value());
+      OnError(
+        SemanticEID::invalidArgumentType,
+        iter(child).pos.start, argType,
+        childType.value()
+      );
       return std::nullopt;
     }
   }
   return substitutes;
 }
 
 bool TypeAuditor::ViGlobal(Cursor iter) {
   const auto& globalName = iter->data.ToText();
   if (iter->id == TokenID::ID_RADICAL) {
-    if (isFuncDeclaration) {
-      return VisitAndReturn(Typification(globalName).ApplyBool());
-    } else {
-      OnError(SemanticEID::radicalUsage, iter->pos.start, globalName);
+    if (!isFuncDeclaration && !isTypification) {
+      OnError(
+        SemanticEID::radicalUsage,
+        iter->pos.start,
+        globalName
+      );
+      return false;
+    }
+    return VisitAndReturn(Typification(globalName).ApplyBool());
+  } else {
+    if (env.context.FunctionArgsFor(globalName) != nullptr) {
+      OnError(
+        SemanticEID::globalFuncWithoutArgs,
+        iter->pos.start,
+        globalName
+      );
+      return false;
+    }
+    const auto* type = env.context.TypeFor(globalName); 
+    if (type == nullptr) {
+      OnError(
+        SemanticEID::globalNotTyped,
+        iter->pos.start,
+        globalName
+      );
       return false;
     }
-  } else if (env.context.FunctionArgsFor(globalName) != nullptr) {
-    OnError(SemanticEID::globalFuncWithoutArgs, iter->pos.start, globalName);
-    return false;
-  } else if (const auto* type = env.context.TypeFor(globalName); type == nullptr) {
-    OnError(SemanticEID::globalNotTyped, iter->pos.start, globalName);
-    return false;
-  } else {
     return VisitAndReturn(*type);
   }
 }
 
 bool TypeAuditor::ViLocal(Cursor iter) {
   const auto& localName = iter->data.ToText();
   if (isLocalDeclaration || isArgDeclaration) {
     return AddLocalVar(localName, std::get<Typification>(currentType), iter->pos.start);
   } else {
     const auto* local = GetLocalTypification(localName, iter->pos.start);
-    if (local != nullptr) {
-      return VisitAndReturn(*local);
-    } else {
+    if (local == nullptr) {
       return false;
     }
+    return VisitAndReturn(*local);
   }
 }
 
-bool TypeAuditor::ViEmptySet(Cursor iter) {
-  OnError(SemanticEID::emptySetUsage, iter->pos.start);
-  return false;
+bool TypeAuditor::ViEmptySet(Cursor /*iter*/) {
+  return VisitAndReturn(Typification::EmptySet());
 }
 
 bool TypeAuditor::ViLocalBind(Cursor iter) {
   assert(isLocalDeclaration || isFuncDeclaration);
   const Typification type = std::get<Typification>(currentType);
   if (!type.IsTuple() || type.T().Arity() != iter.ChildrenCount()) {
-    OnError(SemanticEID::ivalidBinding, iter(0).pos.start);
+    OnError(SemanticEID::invalidBinding, iter(0).pos.start);
     return false;
   }
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     currentType = type.T().Component(static_cast<Index>(child + Typification::PR_START));
     if (!VisitChild(iter, child)) {
       return false;
     }
@@ -413,106 +482,151 @@
   return VisitAndReturn(type);
 }
 
 bool TypeAuditor::ViArgument(Cursor iter) {
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!domain.has_value()) {
     return false;
-  } else {
-    const auto guard{ isArgDeclaration.CreateGuard() };
-    currentType = domain.value();
-    return VisitChild(iter, 0) && VisitAndReturn(LogicT{});
   }
+  const auto guard{ isArgDeclaration.CreateGuard() };
+  currentType = domain.value();
+  return VisitChild(iter, 0) && VisitAndReturn(LogicT{});
 }
 
 bool TypeAuditor::ViCard(Cursor iter) {
   return ChildTypeDebool(iter, 0, SemanticEID::invalidCard).has_value()
     && VisitAndReturn(Typification::Integer());
 }
 
 bool TypeAuditor::ViArithmetic(Cursor iter) {
-  if (const auto test1 = ChildType(iter, 0); !test1.has_value()) {
+  const auto test1 = ChildType(iter, 0);
+  if (!test1.has_value()) {
     return false;
-  } else if (const auto& type1 = std::get<Typification>(test1.value()); 
-             !env.IsArithmetic(type1)) {
-    OnError(SemanticEID::arithmeticNotSupported, iter(0).pos.start, type1.ToString());
+  } 
+  
+  const auto& type1 = std::get<Typification>(test1.value());
+  if (!env.IsArithmetic(type1)) {
+    OnError(
+      SemanticEID::arithmeticNotSupported,
+      iter(0).pos.start,
+      type1.ToString()
+    );
     return false;
-  } else if (const auto test2 = ChildType(iter, 1); !test2.has_value()) {
+  } 
+  
+  const auto test2 = ChildType(iter, 1);
+  if (!test2.has_value()) {
     return false;
-  } else if (const auto& type2 = std::get<Typification>(test2.value()); 
-             !env.IsArithmetic(type2)) {
-    OnError(SemanticEID::arithmeticNotSupported, iter(1).pos.start, type2.ToString());
+  } 
+  
+  const auto& type2 = std::get<Typification>(test2.value());
+  if (!env.IsArithmetic(type2)) {
+    OnError(
+      SemanticEID::arithmeticNotSupported,
+      iter(1).pos.start,
+      type2.ToString()
+    );
     return false;
-  } else if (const auto result = env.Merge(type1, type2); !result.has_value()) {
-    OnError(SemanticEID::typesNotCompatible, iter(1).pos.start, type1, type2);
+  } 
+  
+  const auto result = env.Merge(type1, type2);
+  if (!result.has_value()) {
+    OnError(
+      SemanticEID::typesNotCompatible,
+      iter(1).pos.start,
+      type1,
+      type2
+    );
     return false;
-  } else {
-    return VisitAndReturn(result.value());
   }
+  return VisitAndReturn(result.value());
 }
 
 bool TypeAuditor::ViOrdering(Cursor iter) {
-  if(const auto test1 = ChildType(iter, 0); !test1.has_value()) {
+  const auto test1 = ChildType(iter, 0);
+  if(!test1.has_value()) {
     return false;
-  } else if (const auto& type1 = std::get<Typification>(test1.value());
-             !env.IsOrdered(type1)) {
-    OnError(SemanticEID::orderingNotSupported, iter(0).pos.start, type1.ToString());
+  } 
+  
+  const auto& type1 = std::get<Typification>(test1.value());
+  if (!env.IsOrdered(type1)) {
+    OnError(
+      SemanticEID::orderingNotSupported,
+      iter(0).pos.start,
+      type1.ToString()
+    );
     return false;
-  } else if (const auto test2 = ChildType(iter, 1); !test2.has_value()) {
+  } 
+  
+  const auto test2 = ChildType(iter, 1);
+  if (!test2.has_value()) {
     return false;
-  } else if (const auto& type2 = std::get<Typification>(test2.value());
-             !env.IsOrdered(type2)) {
-    OnError(SemanticEID::orderingNotSupported, iter(1).pos.start, type2.ToString());
+  } 
+  
+  const auto& type2 = std::get<Typification>(test2.value());
+  if (!env.IsOrdered(type2)) {
+    OnError(
+      SemanticEID::orderingNotSupported,
+      iter(1).pos.start,
+      type2.ToString()
+    );
     return false;
-  } else if (!env.AreCompatible(type1, type2)) {
-    OnError(SemanticEID::typesNotCompatible, iter(1).pos.start, type1, type2);
+  } 
+  
+  if (!env.AreCompatible(type1, type2)) {
+    OnError(
+      SemanticEID::typesNotCompatible,
+      iter(1).pos.start,
+      type1,
+      type2
+    );
     return false;
-  } else {
-    return VisitAndReturn(LogicT{});
   }
+  return VisitAndReturn(LogicT{});
 }
 
 bool TypeAuditor::ViQuantifier(Cursor iter) {
   StartScope();
-  if (const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation); !domain.has_value()) {
+
+  const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
+  if (!domain.has_value()) {
     return false;
   } else if (!VisitChildDeclaration(iter, 0, domain.value())) {
     return false;
   } else if (!VisitChild(iter, 2)) {
     return false;
-  } else {
-    EndScope(iter->pos.start);
-    return VisitAndReturn(LogicT{});
   }
+
+  EndScope(iter->pos.start);
+  return VisitAndReturn(LogicT{});
 }
 
 bool TypeAuditor::ViEquals(Cursor iter) {
-  if (iter(1).id == TokenID::LIT_EMPTYSET) {
-    const auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidEqualsEmpty);
-    return type.has_value() && VisitAndReturn(LogicT{});
-  } else {
-    const auto test1 = ChildType(iter, 0);
-    if (!test1.has_value()) {
-      return false;
-    }
-    const auto& type1 = std::get<Typification>(test1.value());
-
-    const auto test2 = ChildType(iter, 1);
-    if (!test2.has_value()) {
-      return false;
-    }
-    const auto& type2 = std::get<Typification>(test2.value());
+  const auto test1 = ChildType(iter, 0);
+  if (!test1.has_value()) {
+    return false;
+  }
+  const auto& type1 = std::get<Typification>(test1.value());
 
-    if (!env.AreCompatible(type1, type2)) {
-      OnError(SemanticEID::typesNotCompatible, iter(1).pos.start, type1, type2);
-      return false;
-    } else {
-      return VisitAndReturn(LogicT{});
-    }
+  const auto test2 = ChildType(iter, 1);
+  if (!test2.has_value()) {
+    return false;
   }
+  const auto& type2 = std::get<Typification>(test2.value());
+
+  if (!env.AreCompatible(type1, type2)) {
+    OnError(
+      SemanticEID::typesNotCompatible,
+      iter(1).pos.start,
+      type1,
+      type2
+    );
+    return false;
+  } 
+  return VisitAndReturn(LogicT{});
 }
 
 bool TypeAuditor::ViTypedPredicate(Cursor iter) {
   auto type2 = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!type2.has_value()) {
     return false;
   }
@@ -523,52 +637,64 @@
   const auto type1 = ChildType(iter, 0);
   if (!type1.has_value()) {
     return false;
   }
 
   if (!env.AreCompatible(type1.value(), type2.value())) {
     if (isSubset) {
-      OnError(SemanticEID::typesNotEqual, iter(1).pos.start, type1.value(), type2.value());
+      OnError(
+        SemanticEID::typesNotEqual,
+        iter(1).pos.start,
+        type1.value(),
+        type2.value()
+      );
     } else {
-      OnError(SemanticEID::invalidElementPredicat, iter(1).pos.start,
-              { ToString(type1.value()), iter->ToString(), type2->Bool().ToString() });
+      OnError(
+        SemanticEID::invalidElementPredicate,
+        iter(1).pos.start,
+        { ToString(type1.value()), iter->ToString(), type2->Bool().ToString() }
+      );
     }
     return false;
-  } else {
-    return VisitAndReturn(LogicT{});
   }
+  return VisitAndReturn(LogicT{});
 }
 
 bool TypeAuditor::ViDeclarative(Cursor iter) {
   StartScope();
-  if (auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation); !domain.has_value()) {
+
+  auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
+  if (!domain.has_value()) {
     return false;
   } else if (!VisitChildDeclaration(iter, 0, domain.value())) {
     return false;
   } else if (!VisitChild(iter, 2)) {
     return false;
-  } else {
-    EndScope(iter->pos.start);
-    return VisitAndReturn(domain->ApplyBool());
   }
+  
+  EndScope(iter->pos.start);
+  return VisitAndReturn(domain->ApplyBool());
 }
 
 bool TypeAuditor::ViImperative(Cursor iter) {
   StartScope();
+
   for (Index child = 1; child < iter.ChildrenCount(); ++child) {
     if (!VisitChild(iter, child)) {
       return false;
     }
   }
-  if (auto type = ChildType(iter, 0); !type.has_value()) {
+
+  auto type = ChildType(iter, 0); 
+  if (!type.has_value()) {
     return false;
-  } else {
-    EndScope(iter->pos.start);
-    return VisitAndReturn(std::get<Typification>(type.value()).Bool());
   }
+
+  EndScope(iter->pos.start);
+  return VisitAndReturn(std::get<Typification>(type.value()).Bool());
 }
 
 bool TypeAuditor::ViImpDeclare(Cursor iter) {
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   return domain.has_value() 
     && VisitChildDeclaration(iter, 0, domain.value());
 }
@@ -577,14 +703,15 @@
   const auto domain = ChildType(iter, 1);
   return domain.has_value()
     && VisitChildDeclaration(iter, 0, std::get<Typification>(domain.value()));
 }
 
 bool TypeAuditor::ViRecursion(Cursor iter) {
   StartScope();
+
   auto initType = ChildType(iter, 1);
   if (!initType.has_value()) {
     return false;
   } else if (!VisitChildDeclaration(iter, 0, std::get<Typification>(initType.value()))) {
     return false;
   }
 
@@ -596,18 +723,23 @@
     }
   }
 
   const auto iterationType = ChildType(iter, iterationIndex);
   if (!iterationType.has_value()) {
     return false;
   } else if (!env.AreCompatible(iterationType.value(), initType.value())) {
-    OnError(SemanticEID::typesNotEqual, iter(iterationIndex).pos.start, 
-            iterationType.value(), initType.value());
+    OnError(
+      SemanticEID::typesNotEqual,
+      iter(iterationIndex).pos.start, 
+      iterationType.value(),
+      initType.value()
+    );
     return false;
   }
+
   EndScope(iter->pos.start);
   return VisitAndReturn(iterationType.value());
 }
 
 bool TypeAuditor::ViDecart(Cursor iter) {
   std::vector<Typification> factors{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
@@ -618,95 +750,117 @@
       factors.emplace_back(type.value());
     }
   }
   return VisitAndReturn(Typification::Tuple(factors).ApplyBool());
 }
 
 bool TypeAuditor::ViBoolean(Cursor iter) {
-  if (auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidBoolean); !type.has_value()) {
+  auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidBoolean);
+  if (!type.has_value()) {
     return false;
-  } else {
-    return VisitAndReturn(type->ApplyBool().ApplyBool());
   }
+  return VisitAndReturn(type->ApplyBool().ApplyBool());
 }
 
 bool TypeAuditor::ViTuple(Cursor iter) {
   std::vector<Typification> components{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
-    if (const auto type = ChildType(iter, child); !type.has_value()) {
+    const auto type = ChildType(iter, child);
+    if (!type.has_value()) {
       return false;
-    } else {
-      components.emplace_back(std::get<Typification>(type.value()));
     }
+    components.emplace_back(std::get<Typification>(type.value()));
   }
   return VisitAndReturn(Typification::Tuple(components));
 }
 
 bool TypeAuditor::ViSetEnum(Cursor iter) {
   auto test = ChildType(iter, 0);
   if (!test.has_value()) {
     return false;
   }
   auto& type = std::get<Typification>(test.value());
   for (Index child = 1; child < iter.ChildrenCount(); ++child) {
-    if (auto childType = ChildType(iter, child); !childType.has_value()) {
+    auto childType = ChildType(iter, child);
+    if (!childType.has_value()) {
       return false;
-    } else if (auto merge = env.Merge(type, std::get<Typification>(childType.value())); 
-               !merge.has_value()) {
-      OnError(SemanticEID::invalidEnumeration, iter(child).pos.start, type, childType.value());
+    } 
+    
+    auto merge = env.Merge(type, std::get<Typification>(childType.value())); 
+    if (!merge.has_value()) {
+      OnError(
+        SemanticEID::invalidEnumeration,
+        iter(child).pos.start,
+        type,
+        childType.value()
+      );
       return false;
-    } else {
-      type = std::move(merge.value());
     }
+    type = std::move(merge.value());
   }
   return VisitAndReturn(type.Bool());
 }
 
 bool TypeAuditor::ViDebool(Cursor iter) {
-  if (auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidDebool); type.has_value()) {
-    return VisitAndReturn(type.value());
-  } else {
+  auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidDebool); 
+  if (!type.has_value()) {
     return false;
   }
+  return VisitAndReturn(type.value());
 }
 
 bool TypeAuditor::ViTypedBinary(Cursor iter) {
   auto type1 = ChildTypeDebool(iter, 0, SemanticEID::invalidTypeOperation);
   if (!type1.has_value()) {
     return false;
   }
+
   auto type2 = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!type2.has_value()) {
     return false;
   }
-  if (const auto result = env.Merge(type1.value(), type2.value()); !result.has_value()) {
-    OnError(SemanticEID::typesNotEqual, iter(1).pos.start, type1->Bool(), type2->Bool());
+
+  const auto result = env.Merge(type1.value(), type2.value());
+  if (!result.has_value()) {
+    OnError(
+      SemanticEID::typesNotEqual,
+      iter(1).pos.start,
+      type1->Bool(),
+      type2->Bool()
+    );
     return false;
-  } else {
-    return VisitAndReturn(result.value().Bool());
   }
+  return VisitAndReturn(result.value().Bool());
 }
 
 bool TypeAuditor::ViProjectSet(Cursor iter) {
   // T(Pri(a)) = B(Pi(D(T(a))))
   const auto baseType = ChildTypeDebool(iter, 0, SemanticEID::invalidProjectionSet);
   if (!baseType.has_value()) {
     return false;
   }
   if (!baseType->IsTuple()) {
-    OnError(SemanticEID::invalidProjectionSet, iter(0).pos.start, { iter->ToString(), baseType->ToString() });
+    OnError(
+      SemanticEID::invalidProjectionSet,
+      iter(0).pos.start,
+      { iter->ToString(), baseType->ToString() }
+    );
     return false;
   }
 
   const auto& indicies = iter->data.ToTuple();
   std::vector<Typification> components{};
   components.reserve(size(indicies));
   for (const auto index : indicies) {
     if (!baseType->T().TestIndex(index)) {
-      OnError(SemanticEID::invalidProjectionSet, iter(0).pos.start, { iter->ToString(), baseType->ToString() });
+      OnError(
+        SemanticEID::invalidProjectionSet,
+        iter(0).pos.start,
+        { iter->ToString(), baseType->ToString() }
+      );
       return false;
     } else {
       components.emplace_back(baseType->T().Component(index));
     }
   }
   currentType = Typification::Tuple(components).ApplyBool();
   return true;
@@ -783,19 +937,22 @@
   // T(red(a)) = B(DD(T(a)))
   const auto baseType = ChildType(iter, 0);
   if (!baseType.has_value()) {
     return false;
   }
   const auto& base = std::get<Typification>(baseType.value());
   if (!base.IsCollection() || !base.B().Base().IsCollection()) {
-    OnError(SemanticEID::invalidReduce, iter(0).pos.start + 1, base.ToString());
+    OnError(
+      SemanticEID::invalidReduce,
+      iter(0).pos.start + 1,
+      base.ToString()
+    );
     return false;
-  } else {
-    return VisitAndReturn(base.B().Base());
   }
+  return VisitAndReturn(base.B().Base());
 }
 
 bool TypeAuditor::VisitAndReturn(ExpressionType type) noexcept {
   currentType = std::move(type);
   return true;
 }
 
@@ -828,24 +985,30 @@
 
 std::optional<Typification> TypeAuditor::ChildTypeDebool(Cursor iter, const Index index, const SemanticEID eid) {
   const auto result = ChildType(iter, index);
   if (!result.has_value() || !std::holds_alternative<Typification>(result.value())) {
     return std::nullopt;
   }
   if (!std::get<Typification>(result.value()).IsCollection()) {
-    OnError(eid, iter(index).pos.start, ToString(result.value()));
+    OnError(
+      eid,
+      iter(index).pos.start,
+      ToString(result.value())
+    );
     return std::nullopt;
-  } else {
-    return std::get<Typification>(result.value()).B().Base();
   }
+  return std::get<Typification>(result.value()).B().Base();
 }
 
 const Typification* TypeAuditor::GetLocalTypification(const std::string& name, const StrPos pos) {
-  const auto varIter = std::find_if(begin(localVars), end(localVars),
-                                    [&](const auto& data) noexcept { return data.arg.name == name; });
+  const auto varIter = std::find_if(
+    begin(localVars),
+    end(localVars),
+    [&](const auto& data) noexcept { return data.arg.name == name; }
+  );
   if (varIter == end(localVars)) {
     if (!isArgDeclaration) {
       OnError(SemanticEID::localUndeclared, pos, name);
     }
     return nullptr;
   } else if (!varIter->enabled) {
     OnError(SemanticEID::localOutOfScope, pos, name);
@@ -864,29 +1027,41 @@
 
 void TypeAuditor::EndScope(const StrPos pos) {
   for (auto& var : localVars) {
     --var.level;
     if (var.level < 0 && var.enabled) {
       var.enabled = false;
       if (var.useCount == 0) {
-        OnError(SemanticEID::localNotUsed, pos, var.arg.name);
+        OnError(
+          SemanticEID::localNotUsed,
+          pos,
+          var.arg.name
+        );
       }
     }
   }
 }
 
 bool TypeAuditor::AddLocalVar(const std::string& name, const Typification& type, const StrPos pos) {
   auto varIter = std::find_if(begin(localVars), end(localVars),
                               [&](const auto& data) noexcept { return data.arg.name == name; });
   if (varIter != end(localVars)) {
     if (varIter->enabled) {
-      OnError(SemanticEID::localShadowing, pos, name);
+      OnError(
+        SemanticEID::localShadowing,
+        pos,
+        name
+      );
       return false;
     } else {
-      OnError(SemanticEID::localDoubleDeclare, pos, name);
+      OnError(
+        SemanticEID::localDoubleDeclare,
+        pos,
+        name
+      );
       varIter->arg.type = type;
       varIter->enabled = true;
       varIter->level = 0;
       varIter->useCount = 0;
       return true;
     }
   } else {
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/Typification.cpp` & `pyconcept-0.1.3/ccl/rslang/src/Typification.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 }
 
 const Typification& Typification::Integer() {
   static const Typification integers{ std::string{integerTypeName} };
   return integers;
 }
 
+const Typification& Typification::EmptySet() {
+  static const auto empty = Typification{ std::string{anyTypificationName} }.Bool();
+  return empty;
+}
+
 std::string Typification::ToString() const noexcept(false) {
   std::string result{};
   std::visit(meta::Overloads{ [&](const auto& val) { result = val.ToString(); }},
              state);
   return result;
 }
```

### Comparing `pyconcept-0.1.2/ccl/rslang/src/ValueAuditor.cpp` & `pyconcept-0.1.3/ccl/rslang/src/ValueAuditor.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,19 @@
     current = funcType;
     return true;
   } else {
     return RunCheckOnFunc(iter, globalName, args);
   }
 }
 
-bool ValueAuditor::RunCheckOnFunc(Cursor iter, 
-                                  const std::string& funcName, 
-                                  const std::vector<ValueClass>& argumentVals) {
+bool ValueAuditor::RunCheckOnFunc(
+  Cursor iter, 
+  const std::string& funcName, 
+  const std::vector<ValueClass>& argumentVals
+) {
   const auto* ast = globalAST(funcName);
   if (ast == nullptr) {
     OnError(SemanticEID::globalMissingAST, iter->pos.start, funcName);
     return false;
   }
 
   ValueAuditor funcAuditor{ globalClass, globalAST };
@@ -119,33 +121,31 @@
       funcAuditor.localProps.emplace_back(args.Child(child)(0).data.ToText());
     }
   }
 
   if (!ast->Root().Child(1).Child(1).DispatchVisit(funcAuditor)) {
     OnError(SemanticEID::globalFuncNoInterpretation, iter->pos.start);
     return false;
-  } else {
-    current = funcAuditor.VType();
-    return true;
   }
+  current = funcAuditor.VType();
+  return true;
 }
 
 bool ValueAuditor::ViGlobal(Cursor iter) {
   const auto& globalName = iter->data.ToText();
   if (iter->id == TokenID::ID_RADICAL) {
     return VisitAndReturn(ValueClass::value);
   } else {
     const auto type = globalClass(globalName);
     if (type == ValueClass::invalid) {
       OnError(SemanticEID::globalNoValue, iter->pos.start, globalName);
       return false;
-    } else {
-      current = type;
-      return true;
     }
+    current = type;
+    return true;
   }
 }
 
 bool ValueAuditor::ViLocal(Cursor iter) {
   const auto& localName = iter->data.ToText();
   if (std::find(begin(localProps), end(localProps), localName) == end(localProps)) {
     return VisitAndReturn(ValueClass::value);
```

### Comparing `pyconcept-0.1.2/ccl/rslang/unity/reflex_unity1.cpp` & `pyconcept-0.1.3/ccl/rslang/unity/reflex_unity1.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/ccl/rslang/unity/reflex_unity2.cpp` & `pyconcept-0.1.3/ccl/rslang/unity/reflex_unity2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/cmake/CXXTargets.cmake` & `pyconcept-0.1.3/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/include/pyconcept.h` & `pyconcept-0.1.3/include/pyconcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/pyconcept.egg-info/PKG-INFO` & `pyconcept-0.1.3/pyconcept.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.2
+Version: 0.1.3
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.2/pyconcept.egg-info/SOURCES.txt` & `pyconcept-0.1.3/pyconcept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/setup.cfg` & `pyconcept-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/setup.py` & `pyconcept-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/src/pyconcept.cpp` & `pyconcept-0.1.3/src/pyconcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/tests/__pycache__/testBinding.cpython-312.pyc` & `pyconcept-0.1.3/tests/__pycache__/testBinding.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/tests/data/Schema1.trs` & `pyconcept-0.1.3/tests/data/Schema1.trs`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.2/tests/testBinding.py` & `pyconcept-0.1.3/tests/testBinding.py`

 * *Files identical despite different names*

