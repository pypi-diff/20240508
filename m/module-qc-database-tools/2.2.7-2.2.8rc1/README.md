# Comparing `tmp/module_qc_database_tools-2.2.7.tar.gz` & `tmp/module_qc_database_tools-2.2.8rc1.tar.gz`

## Comparing `module_qc_database_tools-2.2.7.tar` & `module_qc_database_tools-2.2.8rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.env.template
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.gitlab-ci.yml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/ci/pre-commit-update.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/docs/.gitkeep
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    25500 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/LICENSE
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/README.md
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.env.template
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/docs/.gitkeep
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    26057 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/LICENSE
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/README.md
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/PKG-INFO
```

### Comparing `module_qc_database_tools-2.2.7/.gitlab-ci.yml` & `module_qc_database_tools-2.2.8rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/.pre-commit-config.yaml` & `module_qc_database_tools-2.2.8rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/tbump.toml` & `module_qc_database_tools-2.2.8rc1/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e32 2e37 220a 0a23 2045  t = "2.2.7"..# E
-00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
-00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
-00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
-00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
-00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
-00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
-00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
-00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
-000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
-000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
-000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
-000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
-000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
-000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
-00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
-00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
-00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
-00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 322e  mp version: 2.2.
-00000150: 3720 e286 9220 7b6e 6577 5f76 6572 7369  7 ... {new_versi
-00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
-00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
-00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
-00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
-000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
-000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
-000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
-000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
-00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
-00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
-00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
-00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
-00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
-00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
-00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
-00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
-00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
-00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
-000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
-000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
-000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
-000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
-000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
-000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
-00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
-00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
-00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
-00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
-00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
-00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
-00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
+00000010: 7420 3d20 2232 2e32 2e38 7263 3122 0a0a  t = "2.2.8rc1"..
+00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
+00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
+00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
+00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
+00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
+00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
+00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
+00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
+000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
+000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
+000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
+000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
+000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
+000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
+00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
+00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
+00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
+00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
+00000140: 2242 756d 7020 7665 7273 696f 6e3a 2032  "Bump version: 2
+00000150: 2e32 2e38 7263 3120 e286 9220 7b6e 6577  .2.8rc1 ... {new
+00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
+00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
+00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
+00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
+000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
+000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
+000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
+000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
+000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
+00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
+00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
+00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
+00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
+00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
+00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
+00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
+00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
+00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
+00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
+000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
+000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
+000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
+000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
+000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
+000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
+00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
+00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
+00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
+00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
+00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
+00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
+00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
+00000380: 2222 0a                                  "".
```

### Comparing `module_qc_database_tools-2.2.7/ci/pre-commit-update.sh` & `module_qc_database_tools-2.2.8rc1/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/__init__.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/chip_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/core.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 import sys
 from pathlib import Path
 
 import pandas as pd
 from bson.objectid import ObjectId
 
 from module_qc_database_tools.chip_config_api import ChipConfigAPI
-from module_qc_database_tools.utils import chip_serial_number_to_uid
+from module_qc_database_tools.utils import (
+    chip_serial_number_to_uid,
+    get_chip_type_from_serial_number,
+)
 
 log = logging.getLogger(__name__)
 
 
 class Module:
     """
     Module class.
     """
 
     def __init__(self, client, serial_number, no_eos_token=False, name=None):
         self.client = client
         self.serial_number = serial_number
         self.name = name if name else self.serial_number
+        self.chip_type = get_chip_type_from_serial_number(self.serial_number)
         self.module = client.get("getComponent", json={"component": serial_number})
         self.bare_modules = []
         self.chips = []
         self.sensors = []
         self.orientation = True
         self.sensor_vendor = None
         for _property in self.module["properties"]:
@@ -103,28 +107,29 @@
             layer_config,
             version,
             speed,
         )
         if self.module_type == "triplet" and reverse:
             log.info("Orientation is reverse!")
 
-        configs = {"module": {"chipType": "RD53B", "chips": []}, "chips": []}
+        configs = {"module": {"chipType": self.chip_type, "chips": []}, "chips": []}
 
         for chip_index, chip in enumerate(self.chips):
             if self.module_type == "triplet":
                 rx = [2, 1, 0][chip_index] if reverse else [0, 1, 2][chip_index]
             else:
                 rx = [2, 1, 0, 3][chip_index]
 
             try:
                 configs["chips"].append(
                     chip.generate_config(
                         copy.deepcopy(
                             chip_template
                         ),  # NB: make sure we copy as Chip::generate_config modifies this in-place
+                        self.chip_type,
                         chip_index,
                         layer_config,
                         self.module_type,
                         suffix=suffix,
                         speed=speed,
                         version=version,
                         sensor_vendor=self.sensor_vendor,
@@ -159,14 +164,15 @@
     Chip class.
     """
 
     def __init__(self, client, serial_number, no_eos_token=False, module_name=None):
         self.client = client
         self.serial_number = serial_number
         self.uid = chip_serial_number_to_uid(serial_number)
+        self.chip_type = get_chip_type_from_serial_number(self.serial_number)
         self.module_name = module_name or self.serial_number
         self.chip = client.get(
             "getComponent",
             json={"component": serial_number, "noEosToken": no_eos_token},
         )
         self.attachments = list(self.chip["attachments"])
         self.test_run = None
@@ -188,15 +194,15 @@
                 "uu-app-binarystore/getBinaryData", json={"code": item["code"]}
             )
 
         with Path(infile.filename).open(mode="r", encoding="UTF-8") as confjson:
             tmp_conf = json.loads(confjson.read())
             try:
                 log.info("Generating chip config for readout at %i MHz.", speed)
-                tmp_conf["RD53B"]["GlobalConfig"]["CdrClkSel"] = {
+                tmp_conf[self.chip_type]["GlobalConfig"]["CdrClkSel"] = {
                     1280: 0,
                     640: 1,
                     320: 2,
                     160: 3,
                 }[speed]
             except KeyError as err:
                 log.error(
@@ -223,25 +229,28 @@
             msg = f"There are no wafer probing data in production DB for chip {self.serial_number}!"
             raise RuntimeError(msg)
         self.test_run = TestRun(self.client, test_id)
 
     def generate_config(
         self,
         chip_template,
+        chip_type,
         chip_index,
         layer_config,
         module_type,
         suffix="",
         version="latest",
         speed=1280,
         sensor_vendor=None,
     ):
         """
         Generate chip config.
         """
+        if "chip_type" in chip_template:
+            chip_template = {chip_type: chip_template.get("chip_type")}
         if version == "latest" and len(self.attachments) >= 3:
             checklist = [".json", layer_config, suffix]
             for item in self.attachments:
                 if all(check in item["title"] for check in checklist):
                     log.info(
                         "Latest chip configs found for chip %s %s %s!",
                         self.uid,
@@ -276,228 +285,228 @@
                 "Generating chip config for chip %s with %s from wafer probing.",
                 self.uid,
                 layer_config,
             )
             power_config = "LP" if suffix == "LP" else layer_config
             try:
                 log.info("Generating chip config for readout at %i MHz.", speed)
-                chip_template["RD53B"]["GlobalConfig"]["CdrClkSel"] = {
+                chip_template[chip_type]["GlobalConfig"]["CdrClkSel"] = {
                     1280: 0,
                     640: 1,
                     320: 2,
                     160: 4,
                 }[speed]
             except KeyError as err:
                 log.error(
                     "Readout speed not valid. Possible choices: [1280, 640, 320, 160] MHz. %s",
                     err,
                 )
                 sys.exit()
 
             if sensor_vendor == 3:  ## HPK
-                chip_template["RD53B"]["GlobalConfig"]["DiffLcc"] = 200
-                chip_template["RD53B"]["GlobalConfig"]["DiffLccEn"] = 1
+                chip_template[chip_type]["GlobalConfig"]["DiffLcc"] = 200
+                chip_template[chip_type]["GlobalConfig"]["DiffLccEn"] = 1
 
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreComp"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreComp"] = {
                 "R0": 350,
                 "R0.5": 350,
                 "L0": 350,
                 "L1": 350,
                 "L2": 350,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampL"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampL"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampM"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampM"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampR"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampR"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampT"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampT"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampTL"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampTL"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffPreampTR"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffPreampTR"] = {
                 "R0": 900,
                 "R0.5": 900,
                 "L0": 900,
                 "L1": 730,
                 "L2": 550,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["DiffVff"] = {
+            chip_template[chip_type]["GlobalConfig"]["DiffVff"] = {
                 "R0": 150,
                 "R0.5": 150,
                 "L0": 150,
                 "L1": 150,
                 "L2": 60,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol0"] = {
+            chip_template[chip_type]["GlobalConfig"]["EnCoreCol0"] = {
                 "R0": 65535,
                 "R0.5": 65535,
                 "L0": 65535,
                 "L1": 65535,
                 "L2": 65535,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol1"] = {
+            chip_template[chip_type]["GlobalConfig"]["EnCoreCol1"] = {
                 "R0": 65535,
                 "R0.5": 65535,
                 "L0": 65535,
                 "L1": 65535,
                 "L2": 65535,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol2"] = {
+            chip_template[chip_type]["GlobalConfig"]["EnCoreCol2"] = {
                 "R0": 65535,
                 "R0.5": 65535,
                 "L0": 65535,
                 "L1": 65535,
                 "L2": 65535,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["GlobalConfig"]["EnCoreCol3"] = {
+            chip_template[chip_type]["GlobalConfig"]["EnCoreCol3"] = {
                 "R0": 63,
                 "R0.5": 63,
                 "L0": 63,
                 "L1": 63,
                 "L2": 63,
                 "LP": 0,
             }[power_config]
-            chip_template["RD53B"]["Parameter"]["Name"] = self.uid
+            chip_template[chip_type]["Parameter"]["Name"] = self.uid
 
             if module_type == "triplet":
-                chip_template["RD53B"]["Parameter"]["ChipId"] = chip_index + 1
-                chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = {
+                chip_template[chip_type]["Parameter"]["ChipId"] = chip_index + 1
+                chip_template[chip_type]["GlobalConfig"]["AuroraActiveLanes"] = {
                     "R0": 7,
                     "R0.5": 3,
                     "L0": 15,
                 }[layer_config]  ## TODO: add source for R0 and R0.5
-                # chip_template["RD53B"]["GlobalConfig"]["MonitorEnable"] = 0
-                # chip_template["RD53B"]["GlobalConfig"]["MonitorV"] = 63
+                # chip_template[chip_type]["GlobalConfig"]["MonitorEnable"] = 0
+                # chip_template[chip_type]["GlobalConfig"]["MonitorV"] = 63
                 for index in range(4):
-                    chip_template["RD53B"]["GlobalConfig"][
+                    chip_template[chip_type]["GlobalConfig"][
                         f"DataMergeOutMux{index}"
                     ] = (0 + index) % 4
-                chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = {
+                chip_template[chip_type]["GlobalConfig"]["SerEnLane"] = {
                     "R0": 7,
                     "R0.5": 3,
                     "L0": 15,
                 }[layer_config]
             else:
-                chip_template["RD53B"]["Parameter"]["ChipId"] = 12 + chip_index
-                chip_template["RD53B"]["GlobalConfig"]["AuroraActiveLanes"] = 1
+                chip_template[chip_type]["Parameter"]["ChipId"] = 12 + chip_index
+                chip_template[chip_type]["GlobalConfig"]["AuroraActiveLanes"] = 1
                 for index in range(4):
-                    chip_template["RD53B"]["GlobalConfig"][
+                    chip_template[chip_type]["GlobalConfig"][
                         f"DataMergeOutMux{index}"
                     ] = ([2, 0, 1, 0][chip_index] + index) % 4
-                chip_template["RD53B"]["GlobalConfig"]["SerEnLane"] = [4, 1, 8, 1][
+                chip_template[chip_type]["GlobalConfig"]["SerEnLane"] = [4, 1, 8, 1][
                     chip_index
                 ]
 
             if not self.test_run:
                 try:
                     self.load_wafer_probing_data()
                 except RuntimeError as err:
                     log.warning("[red]%s Will generate default config.[/]", err)
                     return chip_template
             if self.test_run:
-                chip_template["RD53B"]["GlobalConfig"][
+                chip_template[chip_type]["GlobalConfig"][
                     "SldoTrimA"
                 ] = self.test_run.get_result("VDDA_TRIM")
-                chip_template["RD53B"]["GlobalConfig"][
+                chip_template[chip_type]["GlobalConfig"][
                     "SldoTrimD"
                 ] = self.test_run.get_result("VDDD_TRIM")
-                chip_template["RD53B"]["Parameter"]["ADCcalPar"][0] = (
+                chip_template[chip_type]["Parameter"]["ADCcalPar"][0] = (
                     self.test_run.get_result("ADC_OFFSET") * 1000
                 )
-                chip_template["RD53B"]["Parameter"]["ADCcalPar"][1] = (
+                chip_template[chip_type]["Parameter"]["ADCcalPar"][1] = (
                     self.test_run.get_result("ADC_SLOPE") * 1000
                 )
-                chip_template["RD53B"]["Parameter"]["InjCap"] = (
+                chip_template[chip_type]["Parameter"]["InjCap"] = (
                     self.test_run.get_result("InjectionCapacitance") * (10**15)
                 )
 
                 # For transistor sensors calibration, the ideality factor is calculated following the presentation:
                 # https://indico.cern.ch/event/1011941/contributions/4278988/attachments/2210633/3741190/RD53B_calibatrion_sensor_temperature.pdf
                 e_charge = 1.602e-19
                 kB = 1.38064852e-23
                 PC_NTC = self.test_run.get_result("PC_NTC") + 273
                 DeltaT = 2  # 2 degree difference between PC NTC and transistor sensors
-                chip_template["RD53B"]["Parameter"]["NfDSLDO"] = (
+                chip_template[chip_type]["Parameter"]["NfDSLDO"] = (
                     self.test_run.get_result("TEMPERATURE_D")
                     * e_charge
                     / (kB * math.log(15) * (PC_NTC + DeltaT))
                 )
-                chip_template["RD53B"]["Parameter"]["NfASLDO"] = (
+                chip_template[chip_type]["Parameter"]["NfASLDO"] = (
                     self.test_run.get_result("TEMPERATURE_A")
                     * e_charge
                     / (kB * math.log(15) * (PC_NTC + DeltaT))
                 )
-                chip_template["RD53B"]["Parameter"]["NfACB"] = (
+                chip_template[chip_type]["Parameter"]["NfACB"] = (
                     self.test_run.get_result("TEMPERATURE_C")
                     * e_charge
                     / (kB * math.log(15) * (PC_NTC + DeltaT))
                 )
 
-                chip_template["RD53B"]["Parameter"]["VcalPar"] = [
+                chip_template[chip_type]["Parameter"]["VcalPar"] = [
                     abs(
                         self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_OFFSET") * 1000
                     ),
                     self.test_run.get_result("VCAL_HIGH_LARGE_RANGE_SLOPE") * 1000,
                 ]
-                chip_template["RD53B"]["Parameter"][
+                chip_template[chip_type]["Parameter"][
                     "IrefTrim"
                 ] = self.test_run.get_result("IREF_TRIM")
-                chip_template["RD53B"]["Parameter"][
+                chip_template[chip_type]["Parameter"][
                     "KSenseInA"
                 ] = self.test_run.get_result("CURR_MULT_FAC_A")
-                chip_template["RD53B"]["Parameter"][
+                chip_template[chip_type]["Parameter"][
                     "KSenseInD"
                 ] = self.test_run.get_result("CURR_MULT_FAC_D")
-                chip_template["RD53B"]["Parameter"]["KSenseShuntA"] = (
+                chip_template[chip_type]["Parameter"]["KSenseShuntA"] = (
                     self.test_run.get_result("CURR_MULT_FAC_A") * 26000.0 / 21000.0
                 )
-                chip_template["RD53B"]["Parameter"]["KSenseShuntD"] = (
+                chip_template[chip_type]["Parameter"]["KSenseShuntD"] = (
                     self.test_run.get_result("CURR_MULT_FAC_D") * 26000.0 / 21000.0
                 )
-                chip_template["RD53B"]["Parameter"][
+                chip_template[chip_type]["Parameter"][
                     "KShuntA"
                 ] = self.test_run.get_result("VINA_SHUNT_KFACTOR")
-                chip_template["RD53B"]["Parameter"][
+                chip_template[chip_type]["Parameter"][
                     "KShuntD"
                 ] = self.test_run.get_result("VIND_SHUNT_KFACTOR")
 
             return chip_template
         else:
             msg = f"Not able to generate config for chip {self.uid}. Chip configs might not be complete."
             raise RuntimeError(msg)
@@ -584,15 +593,15 @@
     """
 
     def __init__(self, client, serial_number, name=None):
         self.client = client
         self.localdb = client.localdb
         self.serial_number = serial_number
         self.name = name if name else self.serial_number
-
+        self.chip_type = get_chip_type_from_serial_number(self.serial_number)
         self.module = client.localdb.component.find_one({"serialNumber": serial_number})
 
         self.chips = self.get_chips()
 
         if len(self.chips) == 3:
             self.module_type = "triplet"
             log.info("triplet %s initiated.", self.serial_number)
@@ -663,15 +672,15 @@
             reverse,
         )
 
         config_api = ChipConfigAPI(self.client)
 
         current_stage = self.get_current_stage()
 
-        configs = {"module": {"chipType": "RD53B", "chips": []}, "chips": []}
+        configs = {"module": {"chipType": self.chip_type, "chips": []}, "chips": []}
 
         for chip_index, chip in enumerate(self.chips):
             if self.module_type == "triplet":
                 rx = [2, 1, 0][chip_index]
             else:
                 rx = [2, 1, 0, 3][chip_index]
```

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,26 +22,47 @@
 
     if "PIM1" in serial_number or "PIRB" in serial_number:
         return "L1"
 
     if "PG" in serial_number:
         return "L2"
 
-    log.exception("Error: invalid module SN.")
+    log.exception("Invalid module SN: %s", serial_number)
     raise ValueError()
 
 
 def chip_serial_number_to_uid(serial_number):
     """
     Convert chip serial number to hexadecimal UID.
     """
     assert serial_number.startswith(
         "20UPGFC"
-    ), "Serial number must be for a valid RD53B"
+    ), "Serial number must be for a valid RD53 chip"
     return hex(int(serial_number[-7:]))
 
 
 def chip_uid_to_serial_number(uid):
     """
     Convert chip hexadecimal UID to serial number.
     """
     return f"20UPGFC{int(uid, 16):07}"
+
+
+def get_chip_type_from_serial_number(serial_number):
+    """
+    Convert module SN or chip SN to chip type
+    """
+    if "FC" in serial_number.upper():
+        serial_number = str(chip_serial_number_to_uid(serial_number))
+        if int(serial_number[-5]) == 1:
+            return "RD53B"
+        if int(serial_number[-5]) >= 2:
+            return "ITKPIXV2"
+        log.exception("Invalid serial number: %s", serial_number)
+        raise ValueError()
+
+    if serial_number[7] in ["1", "2"]:
+        return "RD53B"
+    if serial_number[7] == "3":
+        return "ITKPIXV2"
+    log.exception("Invalid serial number: %s", serial_number)
+    raise ValueError()
```

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,18 @@
         typer.echo(f"chip config file saved to {output_path}")
 
 
 def save_configs_mongo(configs, chip_config_client, mode):
     """
     Save the configs generated to mongo.
     """
+    chip_type = configs["chipType"]
     for chip_spec in configs["chips"]:
         chip_serial_number = chip_uid_to_serial_number(
-            chip_spec["RD53B"]["Parameter"]["Name"]
+            chip_spec[chip_type]["Parameter"]["Name"]
         )
         base_commit_id = chip_config_client.create_config(
             chip_serial_number, "MODULE/INITIAL_WARM", branch=mode
         )
         new_commit_id = chip_config_client.commit(
             base_commit_id,
             chip_spec,
```

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/tests/test_cli.py` & `module_qc_database_tools-2.2.8rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/tests/test_config_api.py` & `module_qc_database_tools-2.2.8rc1/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/.gitignore` & `module_qc_database_tools-2.2.8rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/LICENSE` & `module_qc_database_tools-2.2.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/README.md` & `module_qc_database_tools-2.2.8rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v2.2.7
+# Module QC Database Tools v2.2.8rc1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-2.2.7/pyproject.toml` & `module_qc_database_tools-2.2.8rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.7/PKG-INFO` & `module_qc_database_tools-2.2.8rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: module-qc-database-tools
-Version: 2.2.7
+Version: 2.2.8rc1
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 License: Copyright (c) 2022 ATLAS ITk Pixel Modules
@@ -50,15 +50,15 @@
 Requires-Dist: pyarrow
 Requires-Dist: pymongo
 Requires-Dist: rich
 Requires-Dist: typer
 Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v2.2.7
+# Module QC Database Tools v2.2.8rc1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

