# Comparing `tmp/shareyourcloning_linkml-0.1.3a0.tar.gz` & `tmp/shareyourcloning_linkml-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareyourcloning_linkml-0.1.3a0.tar", max compression
+gzip compressed data, was "shareyourcloning_linkml-0.1.4a0.tar", max compression
```

## Comparing `shareyourcloning_linkml-0.1.3a0.tar` & `shareyourcloning_linkml-0.1.4a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1087 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/LICENSE
--rw-r--r--   0        0        0      923 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/README.md
--rw-r--r--   0        0        0    17108 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/excel/shareyourcloning_linkml.xlsx
--rw-r--r--   0        0        0     4114 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/graphql/shareyourcloning_linkml.graphql
--rw-r--r--   0        0        0     6825 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.context.jsonld
--rw-r--r--   0        0        0    81533 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.jsonld
--rw-r--r--   0        0        0    41625 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/jsonschema/shareyourcloning_linkml.schema.json
--rw-r--r--   0        0        0    54043 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/owl/shareyourcloning_linkml.owl.ttl
--rw-r--r--   0        0        0      400 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/prefixmap/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     5967 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/protobuf/shareyourcloning_linkml.proto
--rw-r--r--   0        0        0    63629 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/python/shareyourcloning_linkml.py
--rw-r--r--   0        0        0    43592 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/shacl/shareyourcloning_linkml.shacl.ttl
--rw-r--r--   0        0        0     9441 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/shex/shareyourcloning_linkml.shex
--rw-r--r--   0        0        0    30615 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/sqlschema/shareyourcloning_linkml.sql
--rw-r--r--   0        0        0     1499 2024-05-08 09:21:56.632731 shareyourcloning_linkml-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0      186 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/_version.py
--rw-r--r--   0        0        0       41 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/__init__.py
--rw-r--r--   0        0        0    25796 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/_models.py
--rw-r--r--   0        0        0       42 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/models.py
--rw-r--r--   0        0        0    15500 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-08 11:34:24.551916 shareyourcloning_linkml-0.1.4a0/LICENSE
+-rw-r--r--   0        0        0      923 2024-05-08 11:34:24.551916 shareyourcloning_linkml-0.1.4a0/README.md
+-rw-r--r--   0        0        0    17584 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/excel/shareyourcloning_linkml.xlsx
+-rw-r--r--   0        0        0     4170 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/graphql/shareyourcloning_linkml.graphql
+-rw-r--r--   0        0        0     6881 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.context.jsonld
+-rw-r--r--   0        0        0    82573 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.jsonld
+-rw-r--r--   0        0        0    42013 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonschema/shareyourcloning_linkml.schema.json
+-rw-r--r--   0        0        0    54517 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/owl/shareyourcloning_linkml.owl.ttl
+-rw-r--r--   0        0        0      400 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/prefixmap/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     6097 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/protobuf/shareyourcloning_linkml.proto
+-rw-r--r--   0        0        0    64703 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/python/shareyourcloning_linkml.py
+-rw-r--r--   0        0        0    44003 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/shacl/shareyourcloning_linkml.shacl.ttl
+-rw-r--r--   0        0        0     9599 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/shex/shareyourcloning_linkml.shex
+-rw-r--r--   0        0        0    30549 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/sqlschema/shareyourcloning_linkml.sql
+-rw-r--r--   0        0        0     1499 2024-05-08 11:34:34.396056 shareyourcloning_linkml-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0      186 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/_version.py
+-rw-r--r--   0        0        0       41 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/__init__.py
+-rw-r--r--   0        0        0    25925 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/_models.py
+-rw-r--r--   0        0        0       42 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/models.py
+-rw-r--r--   0        0        0    15604 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.4a0/PKG-INFO
```

### Comparing `shareyourcloning_linkml-0.1.3a0/LICENSE` & `shareyourcloning_linkml-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.3a0/README.md` & `shareyourcloning_linkml-0.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.3a0/project/excel/shareyourcloning_linkml.xlsx` & `shareyourcloning_linkml-0.1.4a0/project/excel/shareyourcloning_linkml.xlsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 504b 0304 1400 0000 0800 d050 a858 465a  PK.........P.XFZ
+00000000: 504b 0304 1400 0000 0800 d263 a858 465a  PK.........c.XFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 d050 a858 150f  PK.........P.X..
-000000c0: 74b6 ee00 0000 cb01 0000 1100 0000 646f  t.............do
+000000b0: 504b 0304 1400 0000 0800 d263 a858 9d88  PK.........c.X..
+000000c0: 5136 ee00 0000 cb01 0000 1100 0000 646f  Q6............do
 000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
-000000e0: 914d 4fc3 300c 86ff ca94 7beb b41d 1344  .MO.0.....{....D
-000000f0: 5d2f a09d 4042 6212 885b 9478 5b44 f3a1  ]/..@Bb..[.x[D..
-00000100: c4a8 ddbf a72d 5b37 0417 8ef1 fbf8 b1ad  .....-[7........
-00000110: d42a 08e5 233e 471f 3092 c1b4 e86d eb92  .*..#>G.0....m..
-00000120: 5061 cd0e 4441 0024 7540 2b53 3e10 6e08  Pa..DA.$u@+S>.n.
-00000130: 773e 5a49 c333 ee21 48f5 21f7 0825 e72b  w>ZI.3.!H.!..%.+
-00000140: b048 524b 9230 0ab3 301b d949 a9d5 ac0c  .HRK.0..0..I....
-00000150: 9fb1 9d04 5a01 b668 d151 8222 2fe0 c212  ....Z..h.Q."/...
-00000160: 469b fe6c 9892 99ec 9399 a9ae ebf2 ae9a  F..l............
-00000170: b861 a302 de9e 1e5f a6e5 33e3 1249 a790  .a....._..3..I..
-00000180: 35b5 5642 4594 e463 335e 148e 7d5b c355  5.VBE..c3^..}[.U
-00000190: b13e cdfe 2ea0 5e0c 1304 1d03 aed9 3979  .>....^.......9y
-000001a0: adee 1fb6 1bd6 94bc 5c66 fc26 e3b7 5b7e  ........\f.&..[~
-000001b0: 27f8 4a54 c5fb e8fa d17f 115a afcd cefc  '.JT.......Z....
-000001c0: d358 5d19 cf82 a686 5fff d67c 0150 4b03  .X]....._..|.PK.
-000001d0: 0414 0000 0008 00d0 50a8 5899 5c9c 2310  ........P.X.\.#.
+000000e0: 91c1 4ec3 300c 865f 65ea bd75 d26e 80a2  ..N.0.._e..u.n..
+000000f0: ac17 d04e 2021 3109 c42d 4abc 2da2 69a3  ...N !1..-J.-.i.
+00000100: c4a8 dddb 9396 ad1b 820b c7f8 fffc d956  ...............V
+00000110: a4f6 4277 019f 43e7 3190 c5b8 185c d346  ..Bw..C.1....\.F
+00000120: a1fd 3a3b 1079 0110 f501 9d8a 4522 da14  ..:;.y......E"..
+00000130: eeba e014 a567 d883 57fa 43ed 114a c66e  .....g..W.C..J.n
+00000140: c021 29a3 48c1 28cc fd6c cc4e 4aa3 67a5  .!).H.(..l.NJ.g.
+00000150: ff0c cd24 301a b041 872d 45e0 0587 0b4b  ...$0..A.-E....K
+00000160: 185c fcb3 614a 6672 8876 a6fa be2f fa6a  .\..aJfr.v.../.j
+00000170: e2d2 461c de9e 1e5f a6e5 73db 4652 adc6  ..F...._..s.FR..
+00000180: ac96 460b 1d50 5117 eaf1 227f 1c1a 0957  ..F..PQ..."....W
+00000190: 4579 9afd 5d40 b348 1304 1d3d aeb3 73f2  Ey..]@.H...=..s.
+000001a0: 5add 3f6c 3759 5db2 7299 b355 ceee b69c  Z.?l7Y].r..U....
+000001b0: 8b8a 896a f53e ba7e f45f 84ae 3376 67ff  ...j.>.~._..3vg.
+000001c0: 69bc bd32 9e05 b584 5fff 567f 0150 4b03  i..2...._.V..PK.
+000001d0: 0414 0000 0008 00d2 63a8 5899 5c9c 2310  ........c.X.\.#.
 000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
 000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
 00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
 00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
 00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
 00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
 00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
@@ -123,15 +123,15 @@
 000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
 000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
 000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
 000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
 000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
 000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
 00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 d050 a858 bbe8 8b38  .........P.X...8
+00000810: 0304 1400 0000 0800 d263 a858 bbe8 8b38  .........c.X...8
 00000820: 3801 0000 1102 0000 1800 0000 786c 2f77  8...........xl/w
 00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
 00000840: 2e78 6d6c 4d52 db6e 8330 0cfd 9528 1fd0  .xmlMR.n.0...(..
 00000850: d049 bba8 02a4 b6d3 b43d 4caa 5a6d 7b4e  .I.......=L.Zm{N
 00000860: c140 d424 6689 3bb6 bf9f 03bd 3d44 f838  .@.$f.;.....=D.8
 00000870: 3ee7 d826 f980 e110 3b00 12bf cefa 58c8  >..&....;.....X.
 00000880: 8ea8 5f28 15ab 0e9c 8e33 ecc1 f34d 83c1  .._(.....3...M..
@@ -146,15 +146,15 @@
 00000910: 618d f6cb d4d4 15f2 498a 1a1a 7db4 b4c5  a.......I...}...
 00000920: e115 4e33 dd5f 5b7c d6a4 cb3c e020 421a  ..N3._[|...<. B.
 00000930: b6cc ab14 244b 2e34 3e2d 6947 81f3 869d  ....$K.4>-iG....
 00000940: a834 75ae 88fd 1352 151f 669e db99 a4d2  .4u....R..f.....
 00000950: aade 7568 8d8f c242 c32a d9ec 910d c3e4  ..uh...B.*......
 00000960: 3d01 c27e 5ced 1e89 d08d 61c7 bf0c 422a  =..~\.....a...B*
 00000970: e0fb 0691 2e20 cd7e 7905 e53f 504b 0304  ..... .~y..?PK..
-00000980: 1400 0000 0800 d050 a858 0712 deaa ee01  .......P.X......
+00000980: 1400 0000 0800 d263 a858 0712 deaa ee01  .......c.X......
 00000990: 0000 2104 0000 1800 0000 786c 2f77 6f72  ..!.......xl/wor
 000009a0: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
 000009b0: 6d6c 8554 db6e db30 0cfd 1543 cf45 95f4  ml.T.n.0...C.E..
 000009c0: 8ec0 36d0 240d d687 0245 8b75 8f81 62d3  ..6.$....E.u..b.
 000009d0: b610 5974 25ba 5eff 7e94 9db8 e996 602f  ..Yt%.^.~.....`/
 000009e0: 1649 9187 8717 39ee d06d 7d05 40d1 efda  .I....9..m}.@...
 000009f0: 589f 888a a899 49e9 b30a 6ae5 cfb1 01cb  X.....I...j.....
@@ -180,15 +180,15 @@
 00000b30: a4de f068 9b96 9ec0 7b5e d8d1 f8e0 1cba  ...h....{^......
 00000b40: 43a3 32bc ec73 a3ec b65f f0c0 3511 467b  C.2..s..._..5.F{
 00000b50: e2cc 61a6 ad51 d354 14ca 933a 2bc1 6ed8  ..a..Q.T...:+.n.
 00000b60: f1cc 5bd5 b00c 2296 a34b 2cbf f3fc c7e0  ..[..."..K,.....
 00000b70: 87a7 f3a4 5ca9 b940 0305 d737 39bf e505  ....\..@...79...
 00000b80: 74c3 2e0e 0a61 d333 d920 11d6 bd58 f113  t....a.3. ...X..
 00000b90: 0617 1cf8 be40 a451 096f 61fc 2ba4 7f00  .....@.Q.oa.+...
-00000ba0: 504b 0304 1400 0000 0800 d050 a858 a497  PK.........P.X..
+00000ba0: 504b 0304 1400 0000 0800 d263 a858 a497  PK.........c.X..
 00000bb0: 6e89 5601 0000 a502 0000 1800 0000 786c  n.V...........xl
 00000bc0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00000bd0: 7433 2e78 6d6c 7552 db6e c230 0cfd 952a  t3.xmluR.n.0...*
 00000be0: 1f40 60d2 2e42 6da5 019a b687 4908 b4ed  .@`..Bm.....I...
 00000bf0: 39b4 2e8d 48e2 92b8 ebf8 fb39 2d97 6982  9...H......9-.i.
 00000c00: a7d8 ce39 c73e 4ed2 0efd 2ed4 0094 fc58  ...9.>N........X
 00000c10: e342 266a a266 2a65 286a b02a 8cb0 01c7  .B&j.f*e(j.*....
@@ -205,15 +205,15 @@
 00000cc0: 6397 f868 364f 8b18 c496 0cd4 2e2e 694d  c..h6O........iM
 00000cd0: 9eeb 9a3b 51ee 9485 5412 4f10 7359 1cf1  ...;Q...T.O.sY..
 00000ce0: b35b f800 fb16 5c71 8d33 bfc5 d1e5 15f4  .[....\q.3......
 00000cf0: e216 9a0e cd3f 75c9 6e4e 2b1a ecc5 e77b  .....?u.nN+....{
 00000d00: 577e ab5d 480c 54ac 331e 3df2 12fc b08f  W~.]H.T.3.=.....
 00000d10: 2121 6cfa e7de 2011 da3e acf9 1b81 8f00  !!l... ..>......
 00000d20: beaf 10e9 9cc4 f738 ffcc fc17 504b 0304  .......8....PK..
-00000d30: 1400 0000 0800 d050 a858 32c0 66ed 4c01  .......P.X2.f.L.
+00000d30: 1400 0000 0800 d263 a858 32c0 66ed 4c01  .......c.X2.f.L.
 00000d40: 0000 4d02 0000 1800 0000 786c 2f77 6f72  ..M.......xl/wor
 00000d50: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
 00000d60: 6d6c 7552 db4e c330 0cfd 952a 1f40 3a24  mluR.N.0...*.@:$
 00000d70: 2e9a da4a 6c08 c103 d2b4 0978 4459 ebb6  ...Jl......xDY..
 00000d80: d192 b824 ee0a 7f8f d3ee c603 4fb1 4f7c  ...$........O.O|
 00000d90: 8e8f 9d64 03fa 5d68 0128 f9b6 c685 5cb4  ...d..]h.(....\.
 00000da0: 44dd 5cca 50b6 6055 b8c2 0e1c dfd4 e8ad  D.\.P.`U........
@@ -229,15 +229,15 @@
 00000e40: 6738 cc74 73b6 f8a8 4815 99c7 21f1 71d8  g8.ts...H...!.q.
 00000e50: 222b 6310 5b72 a176 7149 1bf2 8c6b ee44  "+c.[r.vqI...k.D
 00000e60: 45d9 d3e7 c07b 4697 4962 1f11 95e5 81b5  E....{F.Ib......
 00000e70: f88f 857b f0ad 72cd 5f8e e4ae c751 261b  ...{..r._....Q&.
 00000e80: 71cd afca 37da 85c4 40cd 5ae9 d51d 9bf5  q...7...@.Z.....
 00000e90: 93ef 2921 ecc6 67d9 2211 da31 6cf9 b9c1  ..)!..g."..1l...
 00000ea0: c702 beaf 11e9 94c4 bd9d 7e50 f10b 504b  ..........~P..PK
-00000eb0: 0304 1400 0000 0800 d050 a858 0840 26f8  .........P.X.@&.
+00000eb0: 0304 1400 0000 0800 d263 a858 0840 26f8  .........c.X.@&.
 00000ec0: 5c01 0000 8b02 0000 1800 0000 786c 2f77  \...........xl/w
 00000ed0: 6f72 6b73 6865 6574 732f 7368 6565 7435  orksheets/sheet5
 00000ee0: 2e78 6d6c 7552 db4e c330 0cfd 952a 1f40  .xmluR.N.0...*.@
 00000ef0: 3624 2e42 6d25 3684 e001 6902 018f 286b  6$.Bm%6...i...(k
 00000f00: dd36 5a12 17c7 a38c afc7 e96e 20c1 537c  .6Z........n .S|
 00000f10: 3bf6 3976 f201 6915 3b00 ce3e bd0b b150  ;.9v..i.;..>...P
 00000f20: 1d73 7fa5 75ac 3af0 269e 600f 4132 0d92  .s..u.:.&.`.A2..
@@ -254,15 +254,15 @@
 00000fd0: 24b6 ccab 64a4 9152 6843 5ad2 1393 c4ad  $...d..RhCZ.....
 00000fe0: 4ce2 9220 32d9 91ee 1b84 af8d 875c b3f0  L.. 2........\..
 00000ff0: 4959 5ded d0b3 ffd0 d59a df06 b912 863f  IY]............?
 00001000: 50f3 ff50 f801 d499 d0fe c668 e1bc 5fc4  P..P.......h.._.
 00001010: 5644 3ad2 83a1 d686 9839 68a4 d7e4 e442  VD:......9h....B
 00001020: a4d2 56f5 d661 ecc7 a32e 9119 fd68 76f2  ..V..a.......hv.
 00001030: 5980 5281 e41b 443e 3869 eb87 ff57 7e03  Y.R...D>8i...W~.
-00001040: 504b 0304 1400 0000 0800 d050 a858 4ec7  PK.........P.XN.
+00001040: 504b 0304 1400 0000 0800 d263 a858 4ec7  PK.........c.XN.
 00001050: 5d80 8a01 0000 9103 0000 1800 0000 786c  ].............xl
 00001060: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00001070: 7436 2e78 6d6c 8553 6d4f dc30 0cfe 2b55  t6.xml.SmO.0..+U
 00001080: 7e00 3986 3626 d456 8263 ecf6 6112 026d  ~.9.6&.V.c..a..m
 00001090: 7c3c e55a b78d 2e8d 83e3 d2f1 efe7 f45e  |<.Z...........^
 000010a0: 00e9 2a3e c576 fc3c 7e1c 3bf9 88b4 8d1d  ..*>.v.<~.;.....
 000010b0: 0067 ff7a e763 a13a e670 a575 ac3a e84d  .g.z.c.:.p.u.:.M
@@ -282,15 +282,15 @@
 00001190: 6a4f 70f3 29c1 28d3 423f cfb0 9c63 1822  jOp.).(.B?...c."
 000011a0: d0da fa30 f009 d4ed 1caa b254 0dce d009  ...0.......T....
 000011b0: cc8f 39cc 5c91 bbd9 e606 3e8d f839 87e0  ..9.\.....>..9..
 000011c0: d770 aaf9 d5ac a4fa 63b6 96c9 1dd6 6137  .p......c.....a7
 000011d0: cab4 aabf 0db5 d6c7 cc41 232c 8bb3 4b19  .........A#,..K.
 000011e0: 38ed 66bf 7318 c3b4 da1b 64c6 7e32 3bf9  8.f.s.....d.~2;.
 000011f0: 3240 2941 ee1b 443e 3a69 f78e bfb0 fc0f  2@)A..D>:i......
-00001200: 504b 0304 1400 0000 0800 d050 a858 4409  PK.........P.XD.
+00001200: 504b 0304 1400 0000 0800 d263 a858 4409  PK.........c.XD.
 00001210: 9006 e701 0000 3704 0000 1800 0000 786c  ......7.......xl
 00001220: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00001230: 7437 2e78 6d6c 7554 4d6f a330 10fd 2bc8  t7.xmluTMo.0..+.
 00001240: e7aa 26d5 f643 1120 3549 dbed a152 d56a  ..&..C. 5I...R.j
 00001250: db63 e5c0 0056 8c4d ed61 69ff fd8e 4d42  .c...V.M.ai...MB
 00001260: 132d 5cf0 cc78 decc 1bfb 99a4 3776 e76a  .-\..x......7v.j
 00001270: 008c be1a a55d ca6a c476 c9b9 cb6b 6884  .....].j.v...kh.
@@ -316,15 +316,15 @@
 000013b0: f0e8 cfe1 099c 2319 8fc1 3b6b 8d3d 0e0a  ......#...;k.=..
 000013c0: 454f 60a5 84de 05d9 fbc9 52a6 a443 eaec  EO`.......R..C..
 000013d0: 6fba 5362 91b1 5238 1467 15e8 2d25 9e39  o.Sb..R8.g..-%.9
 000013e0: 2d5a b281 257c 4c49 f829 cfff 026e 7850  -Z..%|LI.)...nxP
 000013f0: 4fc2 5692 0654 50d2 7cf1 f935 c9d2 0e0a  O.V..TP.|..5....
 00001400: 1d1c 346d 60b2 3588 a609 664d 0f1b ac4f  ..4m`.5...fM...O
 00001410: a0fd d218 1c1d ff42 c67f 45f6 0f50 4b03  .......B..E..PK.
-00001420: 0414 0000 0008 00d0 50a8 5891 c100 8bd2  ........P.X.....
+00001420: 0414 0000 0008 00d2 63a8 5891 c100 8bd2  ........c.X.....
 00001430: 0100 00f6 0300 0018 0000 0078 6c2f 776f  ...........xl/wo
 00001440: 726b 7368 6565 7473 2f73 6865 6574 382e  rksheets/sheet8.
 00001450: 786d 6c8d 53db 6edb 300c fd15 43cf 43e5  xml.S.n.0...C.C.
 00001460: 14bd 21b0 0d34 4983 f5a1 40d1 62ed e3a0  ..!..4I...@.b...
 00001470: d8b4 2d44 165d 899e 97bf 1f65 276e ba25  ..-D.].....e'n.%
 00001480: c05e 24de 0ec5 4352 498f 6eeb 6b00 8a7e  .^$...CRI.n.k..~
 00001490: 37c6 fa54 d444 ed5c 4a9f d7d0 287f 812d  7..T.D.\J...(..-
@@ -348,16 +348,16 @@
 000015b0: 8627 5f63 bf72 d8ae b0b7 614b 06c3 63e8  .'_c.r....aK..c.
 000015c0: c313 78cf cb38 191f 9c43 776c 5486 1779  ..x..8...CwlT..y
 000015d0: 6194 dd0e cb1b 98a5 c268 4ffc 72f8 249d  a........hO.r.$.
 000015e0: 51b3 4ca8 a2a8 c0c2 373e 361c 2a12 39f9  Q.L.....7>6.*.9.
 000015f0: 12f9 b5c0 7f0c 7efc 0f4f ca55 9a99 1928  ......~..O.U...(
 00001600: 9958 7c71 cb5b e5c6 051b 15c2 7628 6183  .X|q.[......v(a.
 00001610: 44d8 0c62 cdff 125c 0860 7f89 4893 1216  D..b...\.`..H...
-00001620: 7cfa ead9 1f50 4b03 0414 0000 0008 00d0  |....PK.........
-00001630: 50a8 58d3 d762 9c0b 0200 0031 0500 0018  P.X..b.....1....
+00001620: 7cfa ead9 1f50 4b03 0414 0000 0008 00d2  |....PK.........
+00001630: 63a8 58d3 d762 9c0b 0200 0031 0500 0018  c.X..b.....1....
 00001640: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
 00001650: 2f73 6865 6574 392e 786d 6cbd 544d 6fdb  /sheet9.xml.TMo.
 00001660: 300c fd2b 86ce 5d95 04eb 0702 dbc0 92b4  0..+..].........
 00001670: 4b0f 058a 16ed 8e81 62d3 b110 5974 257a  K.......b...Yt%z
 00001680: 5eff fd28 2771 b320 1e76 dac5 1629 bea7  ^..('q. .v...)..
 00001690: 4791 54dc a2db fa12 80a2 5f95 b13e 1125  G.T......._..>.%
 000016a0: 513d 95d2 6725 54ca 5f62 0d96 770a 7495  Q=..g%T._b..w.t.
@@ -385,15 +385,15 @@
 00001800: 4266 8930 da13 9f1c 46b4 316a 9c8a fc50  Bf.0....F.1j...P
 00001810: 8c2f 4563 ccc5 be2f 3a43 c4b2 8f8b e59f  ./Ec.../:C......
 00001820: 6287 c4cf 27d3 f9ff 13bf 577b c19f 3587  b...'.....W{..5.
 00001830: fe5d f089 c3ef 9e92 47e5 369a cb62 a0e0  .]......G.6..b..
 00001840: aa8c 2e6f 7820 dd6e 3677 0661 dd49 5823  ...ox .n6w.a.IX#
 00001850: 1156 ddb2 e427 0d5c 08e0 fd02 917a 23bc  .V...'.\.....z#.
 00001860: 0dfd 2b99 fe06 504b 0304 1400 0000 0800  ..+...PK........
-00001870: d050 a858 1a82 8f86 9c01 0000 1a04 0000  .P.X............
+00001870: d263 a858 1a82 8f86 9c01 0000 1a04 0000  .c.X............
 00001880: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
 00001890: 732f 7368 6565 7431 302e 786d 6c7d 94db  s/sheet10.xml}..
 000018a0: 4ee4 300c 865f a5ca 0390 0109 58a1 b6d2  N.0.._......X...
 000018b0: 321c 1721 2110 bb97 a34c ebb6 1149 5c12  2..!!....L...I\.
 000018c0: 97ee bcfd 3a9d 0368 d570 35b6 e3ef cfef  ....:..h.p5.....
 000018d0: ca99 7c44 ff16 3a00 cafe 5ae3 4221 3aa2  ..|D..:...Z.B!:.
 000018e0: fe42 ca50 7560 5538 c21e 1c9f 34e8 ad22  .B.Pu`U8....4.."
@@ -414,15 +414,15 @@
 000019d0: ac74 3d83 5c27 5d92 f234 03dc a400 7073  .t=.\']..4....ps
 000019e0: fab7 697d af66 89bb 14a1 5d3f cc39 ba4f  ..i}.f....]?.9.O
 000019f0: 01bc def3 c4af 1441 9b1e 66fa 1f92 96fe  .......A..f.....
 00001a00: 1b40 f20a edf7 72bb 53f1 cd3c 2adf 6a17  .@....r.S..<*.j.
 00001a10: 3203 0dab 2c8e ce79 f3fc 7609 b709 613f  2...,..y..v...a?
 00001a20: bdb1 3512 a19d c28e df2e f8d8 c0e7 0d22  ..5............"
 00001a30: 1d92 f808 0e7f 07e5 3f50 4b03 0414 0000  ........?PK.....
-00001a40: 0008 00d0 50a8 5882 b2f4 9d67 0100 000f  ....P.X....g....
+00001a40: 0008 00d2 63a8 5882 b2f4 9d67 0100 000f  ....c.X....g....
 00001a50: 0300 0019 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
 00001a60: 6565 7473 2f73 6865 6574 3131 2e78 6d6c  eets/sheet11.xml
 00001a70: 7553 db4e c330 0cfd 952a 1f40 3624 2e9a  uS.N.0...*.@6$..
 00001a80: da4a 6c63 8207 a469 13f0 88b2 d66d a3e5  .Jlc...i.....m..
 00001a90: 46e2 51f6 f738 ed6e 48eb 536d c7c7 3e3e  F.Q..8.nH.Sm..>>
 00001aa0: 76d3 d6fa 6d68 0030 f9d5 ca84 8c35 886e  v...mh.0.....5.n
 00001ab0: c279 281a d022 dc58 0786 5e2a ebb5 4072  .y(..".X..^*..@r
@@ -440,15 +440,15 @@
 00001b70: e60a 2afc 82b2 8694 23d1 8841 5e1c 40d3  ..*.....#..A^.@.
 00001b80: 2190 8f6d 8750 b321 9434 6e87 5700 f321  !..m.P.!.4n.W..!
 00001b90: 00ed f43a e279 0881 7b77 8dd2 6290 52f9  ...:.y..{w..b.R.
 00001ba0: 3f9b 936e c765 f442 c643 7913 be96 2624  ?..n.e.B.Cy...&$
 00001bb0: 512b 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b  Q+Z.....{.{....k
 00001bc0: 6311 adee cc86 0e16 7c4c a0f7 ca5a 3c39  c.......|L...Z<9
 00001bd0: 71f3 a77f 20ff 0350 4b03 0414 0000 0008  q... ..PK.......
-00001be0: 00d0 50a8 5882 b2f4 9d67 0100 000f 0300  ..P.X....g......
+00001be0: 00d2 63a8 5882 b2f4 9d67 0100 000f 0300  ..c.X....g......
 00001bf0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
 00001c00: 7473 2f73 6865 6574 3132 2e78 6d6c 7553  ts/sheet12.xmluS
 00001c10: db4e c330 0cfd 952a 1f40 3624 2e9a da4a  .N.0...*.@6$...J
 00001c20: 6c63 8207 a469 13f0 88b2 d66d a3e5 46e2  lc...i.....m..F.
 00001c30: 51f6 f738 ed6e 48eb 536d c7c7 3e3e 76d3  Q..8.nH.Sm..>>v.
 00001c40: d6fa 6d68 0030 f9d5 ca84 8c35 886e c279  ..mh.0.....5.n.y
 00001c50: 281a d022 dc58 0786 5e2a ebb5 4072 7dcd  (..".X..^*..@r}.
@@ -465,16 +465,16 @@
 00001d00: 8846 6c49 89d2 4491 d6e8 292e a913 e60a  .FlI..D...).....
 00001d10: 2afc 82b2 8694 23d1 8841 5e1c 40d3 2190  *.....#..A^.@.!.
 00001d20: 8f6d 8750 b321 9434 6e87 5700 f321 00ed  .m.P.!.4n.W..!..
 00001d30: f43a e279 0881 7b77 8dd2 6290 52f9 3f9b  .:.y..{w..b.R.?.
 00001d40: 936e c765 f442 c643 7913 be96 2624 512b  .n.e.B.Cy...&$Q+
 00001d50: 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b 6311  Z.....{.{....kc.
 00001d60: adee cc86 0e16 7c4c a0f7 ca5a 3c39 71f3  ......|L...Z<9q.
-00001d70: a77f 20ff 0350 4b03 0414 0000 0008 00d0  .. ..PK.........
-00001d80: 50a8 58fb c712 8d4a 0100 0075 0200 0019  P.X....J...u....
+00001d70: a77f 20ff 0350 4b03 0414 0000 0008 00d2  .. ..PK.........
+00001d80: 63a8 58fb c712 8d4a 0100 0075 0200 0019  c.X....J...u....
 00001d90: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
 00001da0: 2f73 6865 6574 3133 2e78 6d6c 7552 d94e  /sheet13.xmluR.N
 00001db0: c330 10fc 95c8 1f50 a748 1caa 9248 3408  .0.....P.H...H4.
 00001dc0: c103 52d5 0a78 7693 4d62 d5f6 067b 4be0  ..R..xv.Mb...{K.
 00001dd0: ef59 273d 10a2 4fde 6b66 676c 6703 fa5d  .Y'=..O.kfglg..]
 00001de0: e800 28f9 b2c6 855c 7444 fd42 ca50 7560  ..(....\tD.B.Pu`
 00001df0: 5598 610f 8e3b 0d7a ab88 53df cad0 7b50  U.a..;.z..S...{P
@@ -490,581 +490,610 @@
 00001e90: 4191 2a32 8f43 e2a3 d922 ab62 1057 f2a0  A.*2.C...".b.W..
 00001ea0: 76f1 9236 e4b9 ae79 1315 8194 a74c 124b  v..6...y.....L.K
 00001eb0: 8805 591d 00cb 4b00 70f5 3fe3 e565 7eaf  ..Y...K.p.?..e~.
 00001ec0: fe22 24ab 3b5a 9ee4 c6e7 7851 bed5 2e24  ."$.;Z....xQ...$
 00001ed0: 061a 664a 67b7 6cca 4ffe a684 b01f 9f6f  ..fJg.l.O......o
 00001ee0: 8b44 68c7 b0e3 6f01 3e0e 70bf 41a4 5312  .Dh...o.>.p.A.S.
 00001ef0: eff7 f4d3 8a1f 504b 0304 1400 0000 0800  ......PK........
-00001f00: d050 a858 2751 7b71 5a01 0000 c902 0000  .P.X'Q{qZ.......
+00001f00: d263 a858 f666 8318 5c01 0000 8b02 0000  .c.X.f..\.......
 00001f10: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00001f20: 732f 7368 6565 7431 342e 786d 6c7d 52db  s/sheet14.xml}R.
-00001f30: 4ec3 300c fd95 2a1f b06c 485c 84da 4a6c  N.0...*..lH\..Jl
-00001f40: 1382 07a4 6908 7844 59eb b6d1 92ba 241e  ....i.xDY.....$.
-00001f50: 85bf c7ee ae0f 634f f1ed f8f8 d849 7b0c  ......cO.....I{.
-00001f60: ebd8 0050 f2e3 5d1b 33d5 1075 f75a c7a2  ...P..].3..u.Z..
-00001f70: 016f e208 3b68 3953 61f0 86d8 0db5 8e5d  .o..;h9Sa......]
-00001f80: 0053 0e20 eff4 d578 7ca3 bdb1 adca d321  .S. ...x|......!
-00001f90: b608 798a 1b72 b685 4548 e2c6 7b13 7ea7  ..y..r..EH..{.~.
-00001fa0: e0b0 cfd4 44ed 034b 5b37 3404 749e 76a6  ....D..K[74.t.v.
-00001fb0: 8657 a0b7 8e01 ecea 439f d27a 68a3 c536  .W......C..zh..6
-00001fc0: 0950 65ea 6172 3fdf 2286 8a77 0b7d 3cb1  .Pe.ar?."..w.}<.
-00001fd0: 1311 b342 5c8b f35c 666a 2c33 8183 82a4  ...B\..\fj,3....
-00001fe0: 85e1 e71b 66e0 9c74 e249 be76 4dd5 9154  ....f..t.I.vM..T
-00001ff0: 90a7 f6be fde3 a09f c75b 9908 3374 1fb6  .........[..3t..
-00002000: a426 5377 2a29 a132 1b47 4bec 9f60 a7e9  .&Sw*).2.GK..`..
-00002010: fa38 e2dc 90c9 d380 7d12 446c 9e16 6208  .8......}.Dl..b.
-00002020: 2517 da56 96f4 4a81 e396 9928 7750 d167  %..V..J....(wP.g
-00002030: 154c cdb2 29d5 c4a3 4842 173b e0f4 3f60  .L..)...HB.;..?`
-00002040: 10ea 4bc8 d945 4a87 8591 1d9d 01ce 2f53  ..K..EJ......./S
-00002050: 9e47 6a56 bc5f e376 0572 e217 136a dbc6  .GjV._.v.r...j..
-00002060: 4428 f938 a35b 5e54 d8ee 6ceb 1076 c397  D(.8.[^T..l..v..
-00002070: 5821 11fa c16c f8ab 4190 02ce 5788 7470  X!...l..A...W.tp
-00002080: e466 87df 9bff 0150 4b03 0414 0000 0008  .f.....PK.......
-00002090: 00d0 50a8 5844 ff81 0869 0100 000c 0300  ..P.XD...i......
-000020a0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000020b0: 7473 2f73 6865 6574 3135 2e78 6d6c 7553  ts/sheet15.xmluS
-000020c0: db6e 8330 0cfd 1594 0f68 da49 bba8 02a4  .n.0.....h.I....
-000020d0: b55d b53d 4caa 5a6d 7b0e 604a d45c 5862  .].=L.Zm{.`J.\Xb
-000020e0: c6fa f773 a0b7 49f0 84ed f81c 1f5f 885b  ...s..I......_.[
-000020f0: eb0e be02 c0e8 572b e313 5621 d673 ce7d  ......W+..V!.s.}
-00002100: 5e81 167e 626b 30f4 525a a705 92eb f6dc  ^..~bk0.RZ......
-00002110: d70e 44d1 81b4 e277 d3e9 03d7 421a 96c6  ..D....w....B...
-00002120: 5d6c e3d2 d836 a8a4 818d 8b7c a3b5 70c7  ]l...6.....|..p.
-00002130: 0528 db26 6cc6 ce81 addc 57d8 0578 1ad7  .(.&l.....W..x..
-00002140: 620f 3bc0 8f9a 00e4 f20b 4f21 3518 2fad  b.;.......O!5./.
-00002150: 891c 9409 7b9e cdd7 3da2 cbf8 94d0 fa1b  ....{...=.......
-00002160: 3b0a cd64 d61e 82f3 5624 6c1a 3481 821c  ;..d....V$l.4...
-00002170: 0385 a0cf 0f2c 41a9 c044 4abe 4fa4 ec5a  .....,A..DJ.O..Z
-00002180: 3420 6fed 33fd baeb 9fe4 65c2 c3d2 aa2f  4 o.3.....e..../
-00002190: 5960 95b0 2716 1550 8a46 e1d6 b6af 70ea  Y`..'..P.F....p.
-000021a0: e9fe 2a71 2550 a4b1 b36d e442 b369 9c07  ..*q%P...m.B.i..
-000021b0: 2394 a444 69c2 9076 e828 2ea9 12a6 b974  #..Di..v.(.....t
-000021c0: 79a3 848b 3992 8a10 e3f9 09b3 18c3 08ef  y...9...........
-000021d0: 4167 ea38 8059 8e61 a4a9 1b1c 00ac c600  Ag.8.Y.a........
-000021e0: b4d0 61c4 cb18 028f 350c e4af 4725 15ff  ..a.....5...G%..
-000021f0: b339 0ded bc89 7e8a e14a de85 db4b e323  .9....~..J...K.#
-00002200: 0525 b14c 278f 346b d78f bd77 d0d6 dd55  .%.L'.4k...w...U
-00002210: 6516 d1ea ceac e85a c185 047a 2fad c58b  e......Z...z/...
-00002220: 13d6 7ef9 01d2 3f50 4b03 0414 0000 0008  ..~...?PK.......
-00002230: 00d0 50a8 5811 26ee aa80 0100 0080 0300  ..P.X.&.........
-00002240: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00002250: 7473 2f73 6865 6574 3136 2e78 6d6c 7593  ts/sheet16.xmlu.
-00002260: 594f c330 0c80 ff4a 951f 4006 1287 505b  YO.0...J..@...P[
-00002270: 898d 633c 2021 10f0 88b2 d65d 2372 e1b8  ..c< !.....]#r..
-00002280: 94fd 7b9c ee00 a4f6 29b6 e3cf 47ec e4bd  ..{.....)...G...
-00002290: c78f d802 50f6 6d8d 8b85 6889 c2a5 94b1  ....P.m...h.....
-000022a0: 6ac1 aa78 e403 38be 693c 5a45 ace2 5ac6  j..x..8.i<ZE..Z.
-000022b0: 80a0 ea01 b246 9ecc 6667 d22a ed44 990f  .....F..fg.*.D..
-000022c0: b647 2c73 df91 d10e 1e31 8b9d b50a 3773  .G,s.....1....7s
-000022d0: 30be 2fc4 b1d8 1b9e f4ba a5c1 20cb 3ca8  0./......... .<.
-000022e0: 353c 03bd 0406 5895 8738 b5b6 e0a2 f62e  5<....X..8......
-000022f0: 4368 0a71 757c b9dc 1283 c7ab 863e fe91  Ch.qu|.......>..
-00002300: b3d4 ccca fb8f a4dc d785 98a5 9ac0 4045  ..............@E
-00002310: 2984 e2e3 0b16 604c 8ac4 957c ee82 8adf  ).....`L...|....
-00002320: a489 fc2b efc3 df0e fd73 792b 1561 e1cd  ...+.....sy+.a..
-00002330: 9bae a92d c485 c86a 6854 67e8 c9f7 4bd8  ...-...jhTg...K.
-00002340: f574 fa5b e2b5 2255 e6e8 fb0c 53b3 655e  .t.[.."U....S.e^
-00002350: 2521 a564 47ed d223 3d13 b25d 7326 2af9  %!.dG..#=..]s&*.
-00002360: 997b 85f5 7b40 6e1c 7349 5c4b ba91 d58e  .{..{@n.sI\K....
-00002370: 9c4f 9108 5f80 11a6 c9c5 1459 69ac 3aa3  .O.._......Yi.:.
-00002380: c698 eb29 46c5 0876 6536 23cc cd14 a35d  ...)F..ve6#....]
-00002390: e868 04b8 9d02 7889 c689 bb29 8236 0146  .h....x....).6.F
-000023a0: fc97 9325 d5ff bd25 0f6a 3ffd ede4 d266  ...%...%.j?....f
-000023b0: 3e28 5c6b 1733 030d 4799 1d9d f37c 713b  >(\k.3..G....|q;
-000023c0: eaad 423e 0c9b bcf2 44de 0e62 cb3f 0430  ..B>....D..b.?.0
-000023d0: 39f0 7de3 3d1d 94b4 6a87 4f57 fe00 504b  9.}.=...j.OW..PK
-000023e0: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
-000023f0: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
-00002400: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002410: 372e 786d 6c75 53db 6e83 300c fd15 940f  7.xmluS.n.0.....
-00002420: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
-00002430: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
-00002440: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
-00002450: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
-00002460: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
-00002470: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
-00002480: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
-00002490: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
-000024a0: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
-000024b0: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
-000024c0: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
-000024d0: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
-000024e0: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
-000024f0: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
-00002500: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
-00002510: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
-00002520: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
-00002530: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
-00002540: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
-00002550: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
-00002560: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
-00002570: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
-00002580: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
-00002590: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
-000025a0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-000025b0: 382e 786d 6c75 53db 6e83 300c fd15 940f  8.xmluS.n.0.....
-000025c0: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
-000025d0: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
-000025e0: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
-000025f0: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
-00002600: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
-00002610: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
-00002620: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
-00002630: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
-00002640: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
-00002650: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
-00002660: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
-00002670: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
-00002680: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
-00002690: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
-000026a0: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
-000026b0: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
-000026c0: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
-000026d0: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
-000026e0: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
-000026f0: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
-00002700: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
-00002710: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
-00002720: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
-00002730: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
-00002740: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002750: 392e 786d 6c75 53db 6e83 300c fd15 940f  9.xmluS.n.0.....
-00002760: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
-00002770: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
-00002780: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
-00002790: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
-000027a0: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
-000027b0: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
-000027c0: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
-000027d0: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
-000027e0: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
-000027f0: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
-00002800: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
-00002810: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
-00002820: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
-00002830: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
-00002840: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
-00002850: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
-00002860: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
-00002870: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
-00002880: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
-00002890: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
-000028a0: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
-000028b0: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
-000028c0: 0304 1400 0000 0800 d050 a858 19ef 2f38  .........P.X../8
-000028d0: 7b01 0000 4b03 0000 1900 0000 786c 2f77  {...K.......xl/w
-000028e0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
-000028f0: 302e 786d 6c75 93db 4ec3 300c 865f a5ca  0.xmlu..N.0.._..
-00002900: 0390 81c4 41a8 adc4 364e 1748 6808 b844  ....A...6N.Hh..D
-00002910: 59eb ae11 3914 c7a5 8ca7 c7e9 8e48 ed55  Y...9........H.U
-00002920: 6dc7 9ff3 3b76 d3ce e367 a801 28f9 b1c6  m...;v...g..(...
-00002930: 854c d444 cdb5 94a1 a8c1 aa70 e21b 707c  .L.D.......p..p|
-00002940: 5279 b48a d8c5 950c 0d82 2a7b c81a 7936  Ry........*{..y6
-00002950: 995c 48ab b413 79da c79e 314f 7d4b 463b  .\H...y...1O}KF;
-00002960: 78c6 24b4 d62a 5c4f c1f8 2e13 a762 1758  x.$..*\O.....b.X
-00002970: e855 4d7d 40e6 69a3 56f0 02f4 da30 c0ae  .UM}@.i.V....0..
-00002980: dcd7 29b5 0517 b477 0942 9589 9bd3 ebfb  ..)....w.B......
-00002990: 0dd1 67bc 69e8 c291 9dc4 6696 de7f 46e7  ..g.i.....f...F.
-000029a0: b1cc c424 6a02 0305 c512 8a3f df30 0363  ...$j......?.0.c
-000029b0: 6225 56f2 b52d 2a0e 9746 f2d8 de95 bfeb  b%V..-*..F......
-000029c0: fb67 794b 1560 e6cd bb2e a9ce c495 484a  .gyK.`........HJ
-000029d0: a854 6b68 e1bb 07d8 f674 7e90 3857 a4f2  .Tkh.....t~.8W..
-000029e0: 147d 9760 6c36 4f8b 68c4 2b39 51bb f848  .}.`l6O.h.+9Q..H
-000029f0: 2f84 1cd7 7c13 e508 8150 f772 3fc0 fdae  /...|....P.r?...
-00002a00: 2d84 5412 0b8a c7b2 d8e2 d331 bcd0 58b4  -.T........1..X.
-00002a10: 46e1 0033 1b63 5408 6097 663d c0cc c718  F..3.cT.`.f=....
-00002a20: ed9a 9606 80db 3180 f761 98b8 1b23 68dd  ......1..a...#h.
-00002a30: c040 fefd a8a4 f27f b6e4 37df 0d72 3384  .@........7..r3.
-00002a40: b864 4f0a 57da 85c4 40c5 5526 2797 3c2a  .dO.W...@.U&'.<*
-00002a50: dc4c 6de3 906f faa5 5c7a 226f 7bb3 e665  .Lm..o..\z"o{..e
-00002a60: 078c 097c 5e79 4f7b 276e cdfe ffc9 ff00  ...|^yO{'n......
-00002a70: 504b 0304 1400 0000 0800 d050 a858 caac  PK.........P.X..
-00002a80: fec0 7101 0000 3e03 0000 1900 0000 786c  ..q...>.......xl
-00002a90: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00002aa0: 7432 312e 786d 6c75 93db 6e83 300c 407f  t21.xmlu..n.0.@.
-00002ab0: 05e5 039a 76d2 2eaa 0069 6dd7 6e0f 93aa  ....v....im.n...
-00002ac0: 56db 9e53 3010 3517 9698 b1fe fd1c 7a9d  V..S0.5.......z.
-00002ad0: 044f d88e 8fef c4ad 757b 5f01 60f4 ab95  .O......u{_.`...
-00002ae0: f109 ab10 eb29 e73e ab40 0b3f b235 187a  .....).>.@.?.5.z
-00002af0: 29ac d302 4975 25f7 b503 9177 9056 fc6e  )...Iu%....w.V.n
-00002b00: 3c7e e05a 48c3 d2b8 b3ad 5d1a db06 9534  <~.ZH.....]....4
-00002b10: b076 916f b416 ee30 0365 db84 4dd8 d9b0  .v.o...0.e..M...
-00002b20: 9165 859d 81a7 712d 4ad8 027e d404 90ca  .e....q-J..~....
-00002b30: 2f71 72a9 c178 694d e4a0 48d8 f364 ba3a  /qr..xiM..H..d.:
-00002b40: 129d c7a7 84d6 dfc8 5168 6667 ed3e 286f  ........Qhfg.>(o
-00002b50: 79c2 c6a1 2650 9061 0821 e8f3 0373 502a  y...&P.a.!...sP*
-00002b60: 44a2 4abe 4f41 d935 6920 6fe5 73f8 65d7  D.J.OA.5i o.s.e.
-00002b70: 3f95 b713 1ee6 567d c91c ab84 3db1 2887  ?.....V}....=.(.
-00002b80: 4234 0a37 b67d 8553 4ff7 d712 1702 451a  B4.7.}.SO.....E.
-00002b90: 3bdb 462e 349b c659 1042 4a72 9426 0c69  ;.F.4..Y.BJr.&.i
-00002ba0: 8b8e ec92 3261 5a36 3207 1f73 a41a 8285  ....2aZ62..s....
-00002bb0: 6727 6236 4464 d265 8d12 ae87 990f 31c2  g'b6Dd.e......1.
-00002bc0: 7bd0 3b75 e861 1643 8c34 7583 3dc0 cb10  {.;u.a.C.4u.=...
-00002bd0: 4027 d04f 2c87 083c d4d0 e3bf 1a2c 29ff  @'.O,..<.....,).
-00002be0: efcd 69cc e7dd 1de7 1eee ea5d b852 1a1f  ..i........].R..
-00002bf0: 2928 28ca 78f4 48db 71c7 451d 15b4 7577  )((.x.H.q.E...uw
-00002c00: 873b 8b68 7527 5674 dfe0 8203 bd17 d6e2  .;.hu'Vt........
-00002c10: 4509 8772 f965 d23f 504b 0304 1400 0000  E..r.e.?PK......
-00002c20: 0800 d050 a858 2513 3651 8301 0000 5703  ...P.X%.6Q....W.
-00002c30: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00002c40: 6574 732f 7368 6565 7432 322e 786d 6c75  ets/sheet22.xmlu
-00002c50: 53db 6edb 300c fd15 431f 50a5 1bba 0d85  S.n.0...C.P.....
-00002c60: 6d60 4d2f dbc3 80a2 c5b6 c740 b169 5b88  m`M/.......@.i[.
-00002c70: 246a 145d af7f 3fca b9b4 03e2 2793 14cf  $j.]..?.....'...
-00002c80: e1e1 c5e5 84b4 4b03 0017 7fbd 0ba9 5203  ......K.......R.
-00002c90: 73bc d63a 3503 7893 2e30 4290 970e c91b  s..:5.x..0B.....
-00002ca0: 1697 7a9d 2281 6967 9077 fac3 6af5 497b  ..z.".ig.w..j.I{
-00002cb0: 6383 aacb 39f6 4875 8923 3b1b e091 8a34  c...9.Hu.#;....4
-00002cc0: 7a6f e8f5 061c 4e95 ba54 c7c0 93ed 079e  zo....N..T......
-00002cd0: 03ba 2ea3 e9e1 19f8 6714 80b8 fac4 d35a  ........g......Z
-00002ce0: 0f21 590c 0541 57a9 af97 d70f 7bc4 9cf1  .!Y..AW.....{...
-00002cf0: cbc2 94de d945 6e66 8bb8 cbce f7b6 52ab  .....Enf......R.
-00002d00: ac09 1c34 9c29 8c7c 5e60 0dce 6526 51f2  ...4.).|^`..e&Q.
-00002d10: e740 aade 8a66 e47b fb48 7f3f f72f f2b6  .@...f.{.H.?./..
-00002d20: 26c1 1add 6fdb f250 a92f aa68 a133 a3e3  &...o..P./.h.3..
-00002d30: 279c bec1 a1a7 ab37 89b7 864d 5d12 4e05  '......7...M].N.
-00002d40: e566 ebb2 c946 2e29 8936 e421 3d33 49dc  .f...F.).6.!=3I.
-00002d50: 4a25 aef1 0568 30a1 df34 649b dde6 6324  J%...h0..4d...c$
-00002d60: 1940 a959 24e5 04dd 1c08 6e96 0864 4f93  .@.Y$.....n..dO.
-00002d70: a176 83ce f678 06b8 5e02 1248 e904 8bc0  .v...x..^..H....
-00002d80: db25 a00d 71e4 3380 bbc5 1e47 3e8f b85f  .%..q.3....G>.._
-00002d90: 42f0 6b3c 3784 8745 49ed ffd9 5ae6 7f5c  B.k<7..EI...Z..\
-00002da0: ea7e 21f9 e07e 18ea 6d48 8583 4e58 5617  .~!..~..mH..NXV.
-00002db0: 9f65 6db4 dfe0 de61 8cf3 816e 9119 fd6c  .em....a...n...l
-00002dc0: 0e72 f840 3941 de3b 443e 39f9 824e ff52  .r.@9A.;D>9..N.R
-00002dd0: fd0f 504b 0304 1400 0000 0800 d050 a858  ..PK.........P.X
-00002de0: a50c 764f 5301 0000 a402 0000 1900 0000  ..vOS...........
-00002df0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00002e00: 6565 7432 332e 786d 6c75 52db 6ac3 300c  eet23.xmluR.j.0.
-00002e10: fd95 e00f a8d3 c12e 9424 b0b6 8ced 6150  .........$....aP
-00002e20: 5ab6 3dbb 8992 98fa 365b 59d6 bf9f 9cf4  Z.=.....6[Y.....
-00002e30: 3668 9f2c c93a 47e7 c8ce 7aeb 77a1 05c0  6h.,.:G...z.w...
-00002e40: e457 2b13 72d6 22ba 19e7 a16c 418b 30b1  .W+.r."....lA.0.
-00002e50: 0e0c ddd4 d66b 8194 fa86 07e7 4154 0348  .....k......AT.H
-00002e60: 2b7e 97a6 0f5c 0b69 5891 0db5 952f 32db  +~...\.iX..../2.
-00002e70: a192 0656 3e09 9dd6 c2ef e7a0 6c9f b329  ...V>.......l..)
-00002e80: 3b16 d6b2 6971 28f0 2273 a281 0de0 8723  ;...iq(."s.....#
-00002e90: 00a5 fcc4 5349 0d26 486b 120f 75ce 9ea7  ....SI.&Hk..u...
-00002ea0: b3e5 8818 3a3e 25f4 e122 4ea2 99ad b5bb  ....:>%.."N.....
-00002eb0: 98bc 5539 4ba3 2650 5062 a410 74fc c002  ..U9K.&PPb..t...
-00002ec0: 948a 4ca4 e4fb 40ca ce43 23f2 323e d2bf  ..L...@..C#.2>..
-00002ed0: 0cfe 49de 5604 5858 f525 2b6c 73f6 c492  ..I.V.XX.%+ls...
-00002ee0: 0a6a d129 5cdb fe15 0e9e eecf 1297 0245  .j.)\..........E
-00002ef0: 9179 db27 3e9a 2db2 3206 7124 354a 1397  .y.'>.-.2.q$5J..
-00002f00: b441 4f75 4993 b090 c675 9871 2409 b1c0  .AOuI....u.q$...
-00002f10: cb03 607e 0b40 8bbe 8e58 dc42 e0de c195  ..`~.@...X.B....
-00002f20: fee5 4d49 d5ff 6e4e 668e 1b1a ddc5 d77b  ..MI..nNf......{
-00002f30: 17be 9126 240a 6a62 4927 8fb4 033f ae63  ...&$.jbI'...?.c
-00002f40: 4cd0 bae1 b5b7 16d1 ea21 6ce9 1781 8f0d  L........!l.....
-00002f50: 745f 5b8b a724 3ec7 e963 167f 504b 0304  t_[..$>..c..PK..
-00002f60: 1400 0000 0800 d050 a858 6517 5607 5c01  .......P.Xe.V.\.
-00002f70: 0000 b502 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
-00002f80: 6b73 6865 6574 732f 7368 6565 7432 342e  ksheets/sheet24.
-00002f90: 786d 6c75 52db 4ec3 300c fd95 2a1f b06c  xmluR.N.0...*..l
-00002fa0: 485c 84da 4ab0 09c1 03d2 0402 9eb3 d65d  H\..J..........]
-00002fb0: 2392 b873 5c0a 7f8f d35d 91d8 536c 27e7  #..s\....]..Sl'.
-00002fc0: d8e7 38f9 80f4 195b 00ce bebd 0bb1 502d  ..8....[......P-
-00002fd0: 7377 ab75 ac5a f026 4eb0 8320 370d 9237  sw.u.Z.&N.. 7..7
-00002fe0: 2c29 ad75 ec08 4c3d 82bc d317 d3e9 95f6  ,).u..L=........
-00002ff0: c606 55e6 636d 4965 8e3d 3b1b 6049 59ec  ..U.cmIe.=;.`IY.
-00003000: bd37 f473 0f0e 8742 cdd4 bef0 62d7 2d8f  .7.s...B....b.-.
-00003010: 055d e69d 59c3 2bf0 5b27 0049 f581 a7b6  .]..Y.+.['.I....
-00003020: 1e42 b418 3282 a650 77b3 dbc5 1631 be78  .B..2..Pw....1.x
-00003030: b730 c493 384b 6256 889f 2979 aa0b 354d  .0..8KbV..)y..5M
-00003040: 3381 838a 1385 91e3 0be6 e05c 6292 4936  3..........\b.I6
-00003050: 3b52 756c 9a90 a7f1 9efe 61d4 2fe3 ad4c  ;Rul......a./..L
-00003060: 8439 ba0f 5b73 5ba8 1b95 d5d0 98de f10b  .9..[s[.........
-00003070: 0e8f b0d3 7479 1c71 61d8 9439 e190 5112  ....ty.qa..9..Q.
-00003080: 5be6 550a 524b 7968 4332 e995 49ea 563a  [.U.RKyhC2..I.V:
-00003090: 7119 61d3 43a8 20e6 9a65 8c54 d4d5 0e74  q.a.C. ..e.T...t
-000030a0: 7f16 843d fd0f 999f 8374 24c6 d27f 90c5  ...=.....t$.....
-000030b0: 3948 0db1 22db 2527 ffc2 b4a8 db5b b695  9H..".%'.....[..
-000030c0: 9bd6 f96c 686d 43cc 1c34 4237 9d5c 8b29  ...lhmC..4B7.\.)
-000030d0: b4f5 679b 3076 e3fa 57c8 8c7e 0c5b f956  ..g.0v..W..~.[.V
-000030e0: 40e9 81dc 3788 7c48 d27e 0e3f b5fc 0550  @...7.|H.~.?...P
-000030f0: 4b03 0414 0000 0008 00d0 50a8 58d2 05f1  K.........P.X...
-00003100: 4652 0200 0047 0a00 000d 0000 0078 6c2f  FR...G.......xl/
-00003110: 7374 796c 6573 2e78 6d6c dd56 db8a db30  styles.xml.V...0
-00003120: 10fd 15e3 0fa8 9398 9ab8 2479 a821 5068  ..........$y.!Ph
-00003130: cbc2 ee43 5fe5 584e 04ba b8b2 bc24 fdfa  ...C_.XN.....$..
-00003140: 6a24 e7b6 9be3 52fa 569b e099 393a 3367  j$....R.V...9:3g
-00003150: a431 ceaa 7727 c99f 0f9c bbe4 a8a4 eed7  .1..w'..........
-00003160: e9c1 b9ee 5396 f5bb 0357 acff 603a ae3d  ....S....W..`:.=
-00003170: d21a ab98 f3ae dd67 7d67 396b 7a22 2999  .......g}g9kz").
-00003180: 2d66 b322 534c e874 b3d2 83da 2ad7 273b  -f."SL.t....*.';
-00003190: 3368 b74e 6769 926d 56ad d1d7 d03c 8d01  3h.Ngi.mV....<..
-000031a0: bf96 299e bc32 b94e 2b26 456d 455c cc94  ..)..2.N+&EmE\..
-000031b0: 90a7 185f 84c8 ce48 6313 e7d5 70a2 53a8  ..._...Hc...p.S.
-000031c0: ff15 17cc 4797 a48e b994 d0c6 8668 16cb  ....G........h..
-000031d0: 8447 ef13 0b29 2f2a 1669 0c6c 561d 738e  .G...)/*.i.lV.s.
-000031e0: 5bbd f54e 2485 e87b 6cb4 5f4e 9d57 b1b7  [..N$..{l._N.W..
-000031f0: ec34 5f7c 4c6f 18e1 e1cb d4c6 36dc deb5  .4_|Lo......6...
-00003200: 1b43 9b95 e4ad 2386 15fb 4330 9ce9 e851  .C....#...C0...Q
-00003210: 1be7 8c22 ab11 6c6f 348b 4ace b4d1 f0b9  ..."..lo4.J.....
-00003220: 775c ca67 3aaf 1fed 5d81 639b c48d ffd2  w\.g:...].c.....
-00003230: 843d a78e cfa6 5735 9a31 cde8 5081 db74  .=....W5.1..P..t
-00003240: 31f9 bfe7 edc4 ab71 9f07 df90 0efe cfc1  1......q........
-00003250: 38fe 6479 2b8e c13f b66f 045c 6a07 2577  8.dy+..?.o.\j.%w
-00003260: e52f d184 4665 9d7e a711 9437 39ea 4148  ./..Fe.~...79.AH
-00003270: 27f4 e81d 44d3 70fd be3b 9fdf b1da 0ff9  '...D.p..;......
-00003280: 5d01 bfaa e12d 1ba4 7bb9 80eb f46a 7fe3  ]....-..{....j..
-00003290: 8d18 5479 59f5 448d 8dab aef6 573a ca79  ..TyY.D.....W:.y
-000032a0: 719d 535f 4ce8 861f 7953 8dae ddd7 c14c  q.S_L...yS.....L
-000032b0: bce1 cb8e 5760 bc85 b6e1 0210 6445 1040  ....W`......dE.@
-000032c0: 04c2 5a50 0664 451e acf5 3ff6 b5c4 7d45  ..ZP.dE...?...}E
-000032d0: 102a 5c3e 8696 98b5 c4ac c87b 0855 e186  .*\>.......{.U..
-000032e0: b500 abf4 1768 b92c f3bc 28e0 f656 d563  .....h.,..(..V.c
-000032f0: 1915 dcc3 a2a0 1f48 0815 1207 d6a2 6a7f  .......H......j.
-00003300: bbf3 1303 3031 367f 980d 78ca 9363 035b  ....016...x..c.[
-00003310: 9e18 51d8 f2c4 ce13 04f6 9038 6509 0600  ..Q........8e...
-00003320: d622 0e3c 1438 5124 02d4 a251 03ac 3ca7  .".<.8Q$...Q..<.
-00003330: 7386 0ae1 6b3e 0195 2584 6848 c1f4 1605  s...k>..%.hH....
-00003340: daa8 826e 705e f025 caf3 b204 1081 4046  ...np^.%......@F
-00003350: 9e43 885e d809 08ca 2021 10ca f3f8 217d  .C.^.... !....!}
-00003360: f33d cbce dfb9 ecfa d771 f31b 504b 0304  .=.......q..PK..
-00003370: 1400 0000 0800 d050 a858 b747 eb8a c000  .......P.X.G....
-00003380: 0000 1602 0000 0b00 0000 5f72 656c 732f  .........._rels/
-00003390: 2e72 656c 739d 924b 6e02 310c 40af 1265  .rels..Kn.1.@..e
-000033a0: 5f4c a9c4 0231 acd8 b043 880b b889 e7a3  _L...1...C......
-000033b0: 99c4 9163 c4f4 f68d d8c0 2068 114b ff9e  ...c...... h.K..
-000033c0: 9e2d af0f 34a0 761c 73db a56c c630 c45c  .-..4.v.s..l.0.\
-000033d0: d956 35ad 00b2 6b29 609e 71a2 582a 354b  .V5...k)`.q.X*5K
-000033e0: 402d a134 90d0 f5d8 102c e6f3 25c8 2dc3  @-.4.....,..%.-.
-000033f0: 6ed6 b74c 73fc 49f4 0a91 ebba 73b4 6577  n..Ls.I.....s.ew
-00003400: 0a14 f501 f8ae c39a 234a 435a d971 8033  ........#JCZ.q.3
-00003410: 4bff cddc cf0a d49a 9daf acec fca7 35f0  K.............5.
-00003420: a6cc f3f5 2090 a247 4570 2cf4 91a4 4c8b  .... ..GEp,...L.
-00003430: 7694 af3e 9edd bea4 f3a5 6362 b478 dfe8  v..>......cb.x..
-00003440: fff3 d0a8 143d f9bf 9d30 a589 d2d7 4509  .....=...0....E.
-00003450: 266f b0f9 0550 4b03 0414 0000 0008 00d0  &o...PK.........
-00003460: 50a8 58dc 9a46 7c94 0200 000f 0900 000f  P.X..F|.........
-00003470: 0000 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
-00003480: 6d6c 8d96 6f53 a330 10c6 bf4a 870f 7014  ml..oS.0...J..p.
-00003490: d4fa 67ac 334e f5b4 37de d929 3ddf 07b2  ..g.3N..7..)=...
-000034a0: a53b 2659 2e09 2afd f417 60aa 78c1 ccbd  .;&Y..*...`.x...
-000034b0: 29cd 86fd b11b 9e27 e1f2 95f4 734e f43c  )......'....sN.<
-000034c0: 7993 4299 0b3d 8f76 d656 1771 6c8a 1d48  y.B..=.v.V.ql..H
-000034d0: 66be 5105 cacd 6d49 4b66 dd50 9731 6db7  f.Q...mIKf.P.1m.
-000034e0: 58c0 0d15 b504 65e3 743a 9dc5 1a04 b348  X.....e.t:.....H
-000034f0: caec b032 514f fb1f 96a9 3430 6e76 0056  ...2QO....40nv.V
-00003500: 8a1e 2519 aae8 eaf2 50d9 4a4f e2e1 882c  ..%.....P.JO...,
-00003510: 14ed 93da 681b 7942 7835 1f37 b4c3 c90b  ....h.yBx5.7....
-00003520: 1acc 51a0 6de6 51f7 5f40 3491 a850 e21e  ..Q.m.Q._@4..P..
-00003530: f83c 9a46 13b3 a3d7 7bd2 b827 6599 c80a  .<.F....{..'e...
-00003540: 4d42 cca3 a49f 7802 6db1 f0c2 595b e686  MB....x.m...Y[..
-00003550: e5a6 8b58 96af db9e e7d1 6cea 805b d4c6  ...X......l..[..
-00003560: 7677 747c e68a 7c01 7773 3faa 2d7d 4761  vwt|..|.ws?.-}Ga
-00003570: 41df 300b 779a ea0a 55d9 615c 1bf1 a08f  A.0.w...U.a\....
-00003580: 6e29 0ed7 8962 12e6 d12f f7cb 373b 97d1  n)...b.../..7;..
-00003590: d6e1 e24b ded7 641d 6cd0 a1be 4037 a197  ...K..d.l...@7..
-000035a0: bcc7 0e11 1b78 b3ae 00c8 e04f 0daa 8001  .....x.....O....
-000035b0: 280d 8052 0fb4 d228 410f d28f 02e9 475e  (..R...(A.....G^
-000035c0: fae1 f98b da0e 18c7 01c6 b1c7 5883 b11a  ............X...
-000035d0: 3b11 8ce3 4e02 b813 0ff7 93a9 9a09 d16c  ;...N..........l
-000035e0: 9a0a 7846 b5fe b43a b300 6be6 b17e 5782  ..xF...:..k..~W.
-000035f0: 1807 de2d f5bf a8d3 00ea 74a4 cb8a 0c5a  ...-......t....Z
-00003600: d2cd d2af ea2c 803a f350 d79c df81 8211  .....,.:.P......
-00003610: ce79 8073 ee71 1c84 242c 8834 47e5 b28c  .y.s.q..$,.4G...
-00003620: c74b a621 554e 4372 f059 4185 fb12 1fc8  .K.!UNCr.YA.....
-00003630: e256 ed1b 0937 58ba 50ab 120f 1dd2 7ce2  .V...7X.P.....|.
-00003640: 8b3e 4359 7d78 e781 8a6e af1b 0243 2e48  .>CY}x...n...C.H
-00003650: 7c1b 5c1b 0332 17cd 0fc2 4f98 9011 12df  |.\..2....O.....
-00003660: 0907 8cdf 60c8 0289 ef81 d562 ed33 42d2  ....`......b.3B.
-00003670: 4f7c ed3f 60c9 c657 3b24 fcc4 57fe 3d49  O|.?`..W;$..W.=I
-00003680: 1254 526d d650 90cc 5bad 8d72 432e 487c  .TRm.P..[..rC.H|
-00003690: 1bdc 616e 487d bd66 2133 24be 1b06 7abb  ..anH}.f!3$...z.
-000036a0: 56fc cbee d390 2552 df12 8bf5 325b f96f  V.....%R....2[.o
-000036b0: 230d b921 f5dd f028 b0a4 fb26 d7c8 71ff  #..!...(...&..q.
-000036c0: 4565 c19d 7f64 eb27 e15c a599 81db 370b  Ee...d.'.\....7.
-000036d0: ca8c 3243 4648 7d23 2c04 2977 ae65 56bb  ..2CFH}#,.)w.eV.
-000036e0: 9cb2 1992 425e 487b 2fc4 87d3 92c3 1615  ....B^H{/.......
-000036f0: f0f6 a034 ed84 3bbb 0bf7 e1d0 5e7a bf1f  ...4..;.....^z..
-00003700: 9fb4 6f70 5b0b b170 b147 f5e0 b6e9 f7e3  ..op[..p.G......
-00003710: f7f0 ed70 f517 504b 0304 1400 0000 0800  ...p..PK........
-00003720: d050 a858 7296 7e91 3701 0000 390f 0000  .P.Xr.~.7...9...
-00003730: 1a00 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
-00003740: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 cdd7  kbook.xml.rels..
-00003750: 418e 8230 14c6 f1ab 901e c0f2 aaa2 4ec4  A..0..........N.
-00003760: 951b b713 2fd0 e013 8840 49db c9e8 ed87  ..../....@I.....
-00003770: c802 3f32 8bd9 9879 2bd2 121e ff45 f30b  ..?2...y+....E..
-00003780: ec3f b9b1 b176 5da8 ea3e 24f7 b6e9 42ae  .?...v]..>$...B.
-00003790: aa18 fb0f ad43 5171 6bc3 c2f5 dc0d 77ae  .....CQqk.....w.
-000037a0: ceb7 360e 4b5f eade 1637 5bb2 3669 9a69  ..6.K_...7[.6i.i
-000037b0: ff3a 431d f6af 3393 f3a3 e7bf 4c74 d76b  .:C...3.....Lt.k
-000037c0: 5df0 d115 5f2d 77f1 97c1 fadb f95b a898  ]..._-w......[..
-000037d0: a34a ced6 971c 73a5 efcd b41d f4f3 428b  .J....s.......B.
-000037e0: 61b2 4a4e 975c f9d3 8554 a2ff bbc8 4091  a.JN.\...T....@.
-000037f0: 1150 b484 a2a5 80a2 1514 ad04 14ad a168  .P.............h
-00003800: 2da0 2883 a24c 40d1 068a 3602 8ab6 50b4  -.(..L@...6...P.
-00003810: 1550 b483 a29d 8022 4a91 c854 42d3 8c6d  .P....."J..TB..m
-00003820: 096e 13c2 4d12 e426 a49b 24d8 4d88 3749  .n..M..&..$.M.7I
-00003830: d09b 906f 92e0 3721 e024 4170 42c2 4982  ...o..7!.$ApB.I.
-00003840: e184 8893 04c5 0919 2709 8e1b 74dc 4870  ........'...t.Hp
-00003850: dca0 e346 82e3 66f6 012e c171 838e 1b09  ...F..f....q....
-00003860: 8e1b 74dc bcd5 f110 1f0d 8729 685c 63c0  ..t........)h\c.
-00003870: 5bd1 8ec3 b33c bdff b91c 3767 4778 645a  [....<....7gGxdZ
-00003880: c39f f2e1 0750 4b03 0414 0000 0008 00d0  .....PK.........
-00003890: 50a8 588b 1ae4 a471 0100 0035 1000 0013  P.X....q...5....
-000038a0: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
-000038b0: 735d 2e78 6d6c cd98 cb6e c230 1045 7f25  s].xml...n.0.E.%
-000038c0: ca16 1163 b7a5 0f01 9bb6 db96 457f c04d  ...c........E..M
-000038d0: 26c4 c22f 790c 85bf af13 0a52 2bca 4354  &../y......R+.CT
-000038e0: ea6c 6225 9eb9 f7c6 231d 2919 bdad 3d60  .lb%....#.)...=`
-000038f0: b632 dae2 386f 62f4 0f8c 61d9 8091 5838  .2..8ob...a...X8
-00003900: 0f36 edd4 2e18 19d3 6d98 312f cbb9 9c01  .6......m.1/....
-00003910: 1383 c190 95ce 46b0 b11f 5b8d 7c32 7a82  ......F...[.|2z.
-00003920: 5a2e 74cc 9e57 e931 2a67 c779 008d 79f6  Z.t..W.1*g.y..y.
-00003930: b829 6cbd c6b9 f45e ab52 c6b4 cf96 b6fa  .)l....^.R......
-00003940: e1d2 ff72 2852 6757 838d f2d8 4b05 79c6  ...r(RgW....K.y.
-00003950: f65a 745b bf3a 6c1b 5f97 1082 aa20 9bca  .Zt[.:l._.... ..
-00003960: 105f a449 656c a519 c6b5 062c 0e6b ec49  ._.Iel.....,.k.I
-00003970: e9ea 5a95 50b9 7261 524b 813e 80ac b001  ..Z.P.raRK.>....
-00003980: 8846 171b d1de 11eb 980e 1936 577e 7180  .F.........6W~q.
-00003990: 4ee6 a063 2a9d 06e7 314d 2dc0 f97e dbb1  N..c*...1M-..~..
-000039a0: b4dd 7d9f 8420 4475 e425 7796 49fb e237  ..}.. Du.%w.I..7
-000039b0: 8476 e215 54a7 9aa7 13fe 7061 decd 0459  .v..T.....pa...Y
-000039c0: b75c 7ecc dfe7 bcd3 3f37 88a0 12e4 8a4a  .\~.....?7.....J
-000039d0: 906b 2a41 6ea8 0419 5209 724b 25c8 1d95  .k*An...R.rK%...
-000039e0: 20f7 5482 f001 9924 64d8 cac9 c095 93a1   .T....$d.......
-000039f0: 2b27 8357 4e86 af9c 0c60 3919 c272 3288  +'.WN....`9..r2.
-00003a00: e564 182b c830 5690 61ac 20c3 5841 86b1  .d.+.0V.a. .XA..
-00003a10: e25f 19fb eedc fcaf bf62 dbb5 3052 d95d  ._.......b..0R.]
-00003a20: 00d6 fd2d 987c 0250 4b01 0214 0314 0000  ...-.|.PK.......
-00003a30: 0008 00d0 50a8 5846 5ac1 0c82 0000 00b1  ....P.XFZ.......
-00003a40: 0000 0010 0000 0000 0000 0000 0000 0080  ................
-00003a50: 0100 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
-00003a60: 702e 786d 6c50 4b01 0214 0314 0000 0008  p.xmlPK.........
-00003a70: 00d0 50a8 5815 0f74 b6ee 0000 00cb 0100  ..P.X..t........
-00003a80: 0011 0000 0000 0000 0000 0000 0080 01b0  ................
-00003a90: 0000 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
-00003aa0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00003ab0: d050 a858 995c 9c23 1006 0000 9c27 0000  .P.X.\.#.....'..
-00003ac0: 1300 0000 0000 0000 0000 0000 8001 cd01  ................
-00003ad0: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
-00003ae0: 312e 786d 6c50 4b01 0214 0314 0000 0008  1.xmlPK.........
-00003af0: 00d0 50a8 58bb e88b 3838 0100 0011 0200  ..P.X...88......
-00003b00: 0018 0000 0000 0000 0000 0000 0080 810e  ................
-00003b10: 0800 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00003b20: 2f73 6865 6574 312e 786d 6c50 4b01 0214  /sheet1.xmlPK...
-00003b30: 0314 0000 0008 00d0 50a8 5807 12de aaee  ........P.X.....
-00003b40: 0100 0021 0400 0018 0000 0000 0000 0000  ...!............
-00003b50: 0000 0080 817c 0900 0078 6c2f 776f 726b  .....|...xl/work
-00003b60: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
-00003b70: 6c50 4b01 0214 0314 0000 0008 00d0 50a8  lPK...........P.
-00003b80: 58a4 976e 8956 0100 00a5 0200 0018 0000  X..n.V..........
-00003b90: 0000 0000 0000 0000 0080 81a0 0b00 0078  ...............x
-00003ba0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00003bb0: 6574 332e 786d 6c50 4b01 0214 0314 0000  et3.xmlPK.......
-00003bc0: 0008 00d0 50a8 5832 c066 ed4c 0100 004d  ....P.X2.f.L...M
-00003bd0: 0200 0018 0000 0000 0000 0000 0000 0080  ................
-00003be0: 812c 0d00 0078 6c2f 776f 726b 7368 6565  .,...xl/workshee
-00003bf0: 7473 2f73 6865 6574 342e 786d 6c50 4b01  ts/sheet4.xmlPK.
-00003c00: 0214 0314 0000 0008 00d0 50a8 5808 4026  ..........P.X.@&
-00003c10: f85c 0100 008b 0200 0018 0000 0000 0000  .\..............
-00003c20: 0000 0000 0080 81ae 0e00 0078 6c2f 776f  ...........xl/wo
-00003c30: 726b 7368 6565 7473 2f73 6865 6574 352e  rksheets/sheet5.
-00003c40: 786d 6c50 4b01 0214 0314 0000 0008 00d0  xmlPK...........
-00003c50: 50a8 584e c75d 808a 0100 0091 0300 0018  P.XN.]..........
-00003c60: 0000 0000 0000 0000 0000 0080 8140 1000  .............@..
-00003c70: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003c80: 6865 6574 362e 786d 6c50 4b01 0214 0314  heet6.xmlPK.....
-00003c90: 0000 0008 00d0 50a8 5844 0990 06e7 0100  ......P.XD......
-00003ca0: 0037 0400 0018 0000 0000 0000 0000 0000  .7..............
-00003cb0: 0080 8100 1200 0078 6c2f 776f 726b 7368  .......xl/worksh
-00003cc0: 6565 7473 2f73 6865 6574 372e 786d 6c50  eets/sheet7.xmlP
-00003cd0: 4b01 0214 0314 0000 0008 00d0 50a8 5891  K...........P.X.
-00003ce0: c100 8bd2 0100 00f6 0300 0018 0000 0000  ................
-00003cf0: 0000 0000 0000 0080 811d 1400 0078 6c2f  .............xl/
-00003d00: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00003d10: 382e 786d 6c50 4b01 0214 0314 0000 0008  8.xmlPK.........
-00003d20: 00d0 50a8 58d3 d762 9c0b 0200 0031 0500  ..P.X..b.....1..
-00003d30: 0018 0000 0000 0000 0000 0000 0080 8125  ...............%
-00003d40: 1600 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00003d50: 2f73 6865 6574 392e 786d 6c50 4b01 0214  /sheet9.xmlPK...
-00003d60: 0314 0000 0008 00d0 50a8 581a 828f 869c  ........P.X.....
-00003d70: 0100 001a 0400 0019 0000 0000 0000 0000  ................
-00003d80: 0000 0080 8166 1800 0078 6c2f 776f 726b  .....f...xl/work
-00003d90: 7368 6565 7473 2f73 6865 6574 3130 2e78  sheets/sheet10.x
-00003da0: 6d6c 504b 0102 1403 1400 0000 0800 d050  mlPK...........P
-00003db0: a858 82b2 f49d 6701 0000 0f03 0000 1900  .X....g.........
-00003dc0: 0000 0000 0000 0000 0000 8081 391a 0000  ............9...
-00003dd0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00003de0: 6565 7431 312e 786d 6c50 4b01 0214 0314  eet11.xmlPK.....
-00003df0: 0000 0008 00d0 50a8 5882 b2f4 9d67 0100  ......P.X....g..
-00003e00: 000f 0300 0019 0000 0000 0000 0000 0000  ................
-00003e10: 0080 81d7 1b00 0078 6c2f 776f 726b 7368  .......xl/worksh
-00003e20: 6565 7473 2f73 6865 6574 3132 2e78 6d6c  eets/sheet12.xml
-00003e30: 504b 0102 1403 1400 0000 0800 d050 a858  PK...........P.X
-00003e40: fbc7 128d 4a01 0000 7502 0000 1900 0000  ....J...u.......
-00003e50: 0000 0000 0000 0000 8081 751d 0000 786c  ..........u...xl
-00003e60: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00003e70: 7431 332e 786d 6c50 4b01 0214 0314 0000  t13.xmlPK.......
-00003e80: 0008 00d0 50a8 5827 517b 715a 0100 00c9  ....P.X'Q{qZ....
-00003e90: 0200 0019 0000 0000 0000 0000 0000 0080  ................
-00003ea0: 81f6 1e00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00003eb0: 7473 2f73 6865 6574 3134 2e78 6d6c 504b  ts/sheet14.xmlPK
-00003ec0: 0102 1403 1400 0000 0800 d050 a858 44ff  ...........P.XD.
-00003ed0: 8108 6901 0000 0c03 0000 1900 0000 0000  ..i.............
-00003ee0: 0000 0000 0000 8081 8720 0000 786c 2f77  ......... ..xl/w
-00003ef0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00003f00: 352e 786d 6c50 4b01 0214 0314 0000 0008  5.xmlPK.........
-00003f10: 00d0 50a8 5811 26ee aa80 0100 0080 0300  ..P.X.&.........
-00003f20: 0019 0000 0000 0000 0000 0000 0080 8127  ...............'
-00003f30: 2200 0078 6c2f 776f 726b 7368 6565 7473  "..xl/worksheets
-00003f40: 2f73 6865 6574 3136 2e78 6d6c 504b 0102  /sheet16.xmlPK..
-00003f50: 1403 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
-00003f60: 6901 0000 0c03 0000 1900 0000 0000 0000  i...............
-00003f70: 0000 0000 8081 de23 0000 786c 2f77 6f72  .......#..xl/wor
-00003f80: 6b73 6865 6574 732f 7368 6565 7431 372e  ksheets/sheet17.
-00003f90: 786d 6c50 4b01 0214 0314 0000 0008 00d0  xmlPK...........
-00003fa0: 50a8 5844 ff81 0869 0100 000c 0300 0019  P.XD...i........
-00003fb0: 0000 0000 0000 0000 0000 0080 817e 2500  .............~%.
-00003fc0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003fd0: 6865 6574 3138 2e78 6d6c 504b 0102 1403  heet18.xmlPK....
-00003fe0: 1400 0000 0800 d050 a858 44ff 8108 6901  .......P.XD...i.
-00003ff0: 0000 0c03 0000 1900 0000 0000 0000 0000  ................
-00004000: 0000 8081 1e27 0000 786c 2f77 6f72 6b73  .....'..xl/works
-00004010: 6865 6574 732f 7368 6565 7431 392e 786d  heets/sheet19.xm
-00004020: 6c50 4b01 0214 0314 0000 0008 00d0 50a8  lPK...........P.
-00004030: 5819 ef2f 387b 0100 004b 0300 0019 0000  X../8{...K......
-00004040: 0000 0000 0000 0000 0080 81be 2800 0078  ............(..x
-00004050: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00004060: 6574 3230 2e78 6d6c 504b 0102 1403 1400  et20.xmlPK......
-00004070: 0000 0800 d050 a858 caac fec0 7101 0000  .....P.X....q...
-00004080: 3e03 0000 1900 0000 0000 0000 0000 0000  >...............
-00004090: 8081 702a 0000 786c 2f77 6f72 6b73 6865  ..p*..xl/workshe
-000040a0: 6574 732f 7368 6565 7432 312e 786d 6c50  ets/sheet21.xmlP
-000040b0: 4b01 0214 0314 0000 0008 00d0 50a8 5825  K...........P.X%
-000040c0: 1336 5183 0100 0057 0300 0019 0000 0000  .6Q....W........
-000040d0: 0000 0000 0000 0080 8118 2c00 0078 6c2f  ..........,..xl/
-000040e0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-000040f0: 3232 2e78 6d6c 504b 0102 1403 1400 0000  22.xmlPK........
-00004100: 0800 d050 a858 a50c 764f 5301 0000 a402  ...P.X..vOS.....
-00004110: 0000 1900 0000 0000 0000 0000 0000 8081  ................
-00004120: d22d 0000 786c 2f77 6f72 6b73 6865 6574  .-..xl/worksheet
-00004130: 732f 7368 6565 7432 332e 786d 6c50 4b01  s/sheet23.xmlPK.
-00004140: 0214 0314 0000 0008 00d0 50a8 5865 1756  ..........P.Xe.V
-00004150: 075c 0100 00b5 0200 0019 0000 0000 0000  .\..............
-00004160: 0000 0000 0080 815c 2f00 0078 6c2f 776f  .......\/..xl/wo
-00004170: 726b 7368 6565 7473 2f73 6865 6574 3234  rksheets/sheet24
-00004180: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00004190: d050 a858 d205 f146 5202 0000 470a 0000  .P.X...FR...G...
-000041a0: 0d00 0000 0000 0000 0000 0000 8001 ef30  ...............0
-000041b0: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
-000041c0: 4b01 0214 0314 0000 0008 00d0 50a8 58b7  K...........P.X.
-000041d0: 47eb 8ac0 0000 0016 0200 000b 0000 0000  G...............
-000041e0: 0000 0000 0000 0080 016c 3300 005f 7265  .........l3.._re
-000041f0: 6c73 2f2e 7265 6c73 504b 0102 1403 1400  ls/.relsPK......
-00004200: 0000 0800 d050 a858 dc9a 467c 9402 0000  .....P.X..F|....
-00004210: 0f09 0000 0f00 0000 0000 0000 0000 0000  ................
-00004220: 8001 5534 0000 786c 2f77 6f72 6b62 6f6f  ..U4..xl/workboo
-00004230: 6b2e 786d 6c50 4b01 0214 0314 0000 0008  k.xmlPK.........
-00004240: 00d0 50a8 5872 967e 9137 0100 0039 0f00  ..P.Xr.~.7...9..
-00004250: 001a 0000 0000 0000 0000 0000 0080 0116  ................
-00004260: 3700 0078 6c2f 5f72 656c 732f 776f 726b  7..xl/_rels/work
-00004270: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
-00004280: 0214 0314 0000 0008 00d0 50a8 588b 1ae4  ..........P.X...
-00004290: a471 0100 0035 1000 0013 0000 0000 0000  .q...5..........
-000042a0: 0000 0000 0080 0185 3800 005b 436f 6e74  ........8..[Cont
-000042b0: 656e 745f 5479 7065 735d 2e78 6d6c 504b  ent_Types].xmlPK
-000042c0: 0506 0000 0000 2000 2000 9708 0000 273a  ...... . .....':
-000042d0: 0000 0000                                ....
+00001f20: 732f 7368 6565 7431 342e 786d 6c75 52db  s/sheet14.xmluR.
+00001f30: 4ec3 300c fd95 2a1f b074 485c 34b5 95d8  N.0...*..tH\4...
+00001f40: 1082 07a4 6913 f088 b2d6 5da3 2571 97b8  ....i.....].%q..
+00001f50: 2bfc 3d4e 7745 624f b11d 9fe3 739c 643d  +.=NwEbO....s.d=
+00001f60: fa4d 6800 28f9 b6c6 855c 3444 ed44 ca50  .Mh.(....\4D.D.P
+00001f70: 3660 5518 610b 8e6f 6af4 5611 a77e 2d43  6`U.a..oj.V..~-C
+00001f80: eb41 5503 c81a 7993 a677 d22a ed44 910d  .AU...y..w.*.D..
+00001f90: b5b9 2f32 ecc8 6807 739f 84ce 5ae5 7fa6  ../2..h.s...Z...
+00001fa0: 60b0 cfc5 581c 0b0b bd6e 6828 c822 6bd5  `...X....nh(."k.
+00001fb0: 1a96 40ef 2d03 3895 279e 4a5b 7041 a34b  ..@.-.8.'.J[pA.K
+00001fc0: 3cd4 b978 1c4f 667b c4d0 f1a1 a10f 1771  <..x.Of{.......q
+00001fd0: 12cd ac10 3731 79ad 7291 464d 60a0 a448  ....71y.r.FM`..H
+00001fe0: a1f8 d8c1 0c8c 894c ac64 7b20 15e7 a111  .......L.d{ ....
+00001ff0: 7919 1fe9 9f07 ff2c 6fa5 02cc d07c ea8a  y......,o....|..
+00002000: 9a5c 3c88 a482 5a75 8616 d8bf c0c1 d3ed  .\<...Zu........
+00002010: 59e2 9322 5564 1efb c447 b345 56c6 208e  Y.."Ud...G.EV. .
+00002020: e446 ede2 9296 e4b9 ae79 1215 01b6 1db8  .F.......y......
+00002030: 1232 49ac 22d6 6479 c04c af61 0c96 2afa  .2I.".dy.L.a..*.
+00002040: fb07 33bb 86f1 b003 1fe0 ab44 db1a e01d  ..3........D....
+00002050: 1354 7ff1 9235 1f17 b137 111f e94d f9b5  .T...5...7...M..
+00002060: 7621 3150 336f 3aba 67ab 7eef 7a9f 10b6  v!1P3o:.g.~.z...
+00002070: c3a3 ae90 08ed 1036 fc59 c0c7 06be af11  .......6.Y......
+00002080: e994 c4ad 9ffe 5ff1 0b50 4b03 0414 0000  ......_..PK.....
+00002090: 0008 00d2 63a8 580c 5719 2b43 0100 0044  ....c.X.W.+C...D
+000020a0: 0200 0019 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
+000020b0: 6565 7473 2f73 6865 6574 3135 2e78 6d6c  eets/sheet15.xml
+000020c0: 7552 db4e c330 0cfd 952a 1fb0 6c48 5c34  uR.N.0...*..lH\4
+000020d0: b595 d810 8207 a469 13f0 9cad 6e1b 2d89  .......i....n.-.
+000020e0: 4be2 51f8 7bec 7617 78e0 293e 8e7d ceb1  K.Q.{.v.x.)>.}..
+000020f0: 93bc c7b8 4f2d 0065 5fde 8554 a896 a89b  ....O-.e_..T....
+00002100: 6b9d 762d 7893 26d8 41e0 9b1a a337 c430  k.v-x.&.A....7.0
+00002110: 363a 7511 4c35 3479 a7af a6d3 1bed 8d0d  6:u.L54y........
+00002120: aacc 87dc 2a96 391e c8d9 00ab 98a5 83f7  ....*.9.........
+00002130: 267e 2fc0 615f a899 3a25 d6b6 6969 48e8  &~/.a_..:%..iiH.
+00002140: 32ef 4c03 1ba0 d78e 1b18 ea33 4f65 3d84  2.L........3Oe=.
+00002150: 6431 6411 ea42 ddcf e68b b163 a878 b3d0  d1d..B.....c.x..
+00002160: a75f 7126 c36c 11f7 029e ab42 4dc5 1338  ._q&.l.....BM..8
+00002170: d891 5018 3e3e 6109 ce09 133b f938 92aa  ..P.>>a....;.8..
+00002180: 8ba8 74fe 8e4f f48f c3fc 6c6f 6b12 2cd1  ..t..O....lok.,.
+00002190: bddb 8ada 42dd a9ac 82da 1c1c adb1 7f82  ....B...........
+000021a0: e34c d717 8b0f 864c 9947 ecb3 28c3 96f9  .L.....L.G..(...
+000021b0: 4e02 91e4 421b 6449 1b8a 9cb7 ac44 a583  N...B.dI.....D..
+000021c0: 9a72 4dec 40b0 de1d eb17 ffd5 4751 fcdb  .rM.@.......GQ..
+000021d0: a059 ec34 c1a8 2edb 7d31 b1b1 2165 22c0  .Y.4....}1..!e".
+000021e0: 7b99 dcb2 c738 da1d 0161 37bc c616 89d0  {....8...a7.....
+000021f0: 0f61 cbaf 0c51 0af8 be46 a433 9075 9d3f  .a...Q...F.3.u.?
+00002200: 4ef9 0350 4b03 0414 0000 0008 00d2 63a8  N..PK.........c.
+00002210: 5844 ff81 0869 0100 000c 0300 0019 0000  XD...i..........
+00002220: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00002230: 6865 6574 3136 2e78 6d6c 7553 db6e 8330  heet16.xmluS.n.0
+00002240: 0cfd 1594 0f68 da49 bba8 02a4 b55d b53d  .....h.I.....].=
+00002250: 4caa 5a6d 7b0e 604a d45c 5862 c6fa f773  L.Zm{.`J.\Xb...s
+00002260: a0b7 49f0 84ed f81c 1f5f 885b eb0e be02  ..I......_.[....
+00002270: c0e8 572b e313 5621 d673 ce7d 5e81 167e  ..W+..V!.s.}^..~
+00002280: 626b 30f4 525a a705 92eb f6dc d70e 44d1  bk0.RZ........D.
+00002290: 81b4 e277 d3e9 03d7 421a 96c6 5d6c e3d2  ...w....B...]l..
+000022a0: d836 a8a4 818d 8b7c a3b5 70c7 0528 db26  .6.....|..p..(.&
+000022b0: 6cc6 ce81 addc 57d8 0578 1ad7 620f 3bc0  l.....W..x..b.;.
+000022c0: 8f9a 00e4 f20b 4f21 3518 2fad 891c 9409  ......O!5./.....
+000022d0: 7b9e cdd7 3da2 cbf8 94d0 fa1b 3b0a cd64  {...=.......;..d
+000022e0: d61e 82f3 5624 6c1a 3481 821c 0385 a0cf  ....V$l.4.......
+000022f0: 0f2c 41a9 c044 4abe 4fa4 ec5a 3420 6fed  .,A..DJ.O..Z4 o.
+00002300: 33fd baeb 9fe4 65c2 c3d2 aa2f 5960 95b0  3.....e..../Y`..
+00002310: 2716 1550 8a46 e1d6 b6af 70ea e9fe 2a71  '..P.F....p...*q
+00002320: 2550 a4b1 b36d e442 b369 9c07 2394 a444  %P...m.B.i..#..D
+00002330: 69c2 9076 e828 2ea9 12a6 b974 79a3 848b  i..v.(.....ty...
+00002340: 3992 8a10 e3f9 09b3 18c3 08ef 4167 ea38  9...........Ag.8
+00002350: 8059 8e61 a4a9 1b1c 00ac c600 b4d0 61c4  .Y.a..........a.
+00002360: cb18 028f 350c e4af 4725 15ff b339 0ded  ....5...G%...9..
+00002370: bc89 7e8a e14a de85 db4b e323 0525 b14c  ..~..J...K.#.%.L
+00002380: 278f 346b d78f bd77 d0d6 dd55 6516 d1ea  '.4k...w...Ue...
+00002390: ceac e85a c185 047a 2fad c58b 13d6 7ef9  ...Z...z/.....~.
+000023a0: 01d2 3f50 4b03 0414 0000 0008 00d2 63a8  ..?PK.........c.
+000023b0: 5811 26ee aa80 0100 0080 0300 0019 0000  X.&.............
+000023c0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+000023d0: 6865 6574 3137 2e78 6d6c 7593 594f c330  heet17.xmlu.YO.0
+000023e0: 0c80 ff4a 951f 4006 1287 505b 898d 633c  ...J..@...P[..c<
+000023f0: 2021 10f0 88b2 d65d 2372 e1b8 94fd 7b9c   !.....]#r....{.
+00002400: ee00 a4f6 29b6 e3cf 47ec e4bd c78f d802  ....)...G.......
+00002410: 50f6 6d8d 8b85 6889 c2a5 94b1 6ac1 aa78  P.m...h.....j..x
+00002420: e403 38be 693c 5a45 ace2 5ac6 80a0 ea01  ..8.i<ZE..Z.....
+00002430: b246 9ecc 6667 d22a ed44 990f b647 2c73  .F..fg.*.D...G,s
+00002440: df91 d10e 1e31 8b9d b50a 3773 30be 2fc4  .....1....7s0./.
+00002450: b1d8 1b9e f4ba a5c1 20cb 3ca8 353c 03bd  ........ .<.5<..
+00002460: 0406 5895 8738 b5b6 e0a2 f62e 4368 0a71  ..X..8......Ch.q
+00002470: 757c b9dc 1283 c7ab 863e fe91 b3d4 ccca  u|.......>......
+00002480: fb8f a4dc d785 98a5 9ac0 4045 2984 e2e3  ..........@E)...
+00002490: 0b16 604c 8ac4 957c ee82 8adf a489 fc2b  ..`L...|.......+
+000024a0: efc3 df0e fd73 792b 1561 e1cd 9bae a92d  .....sy+.a.....-
+000024b0: c485 c86a 6854 67e8 c9f7 4bd8 f574 fa5b  ...jhTg...K..t.[
+000024c0: e2b5 2255 e6e8 fb0c 53b3 655e 2521 a564  .."U....S.e^%!.d
+000024d0: 47ed d223 3d13 b25d 7326 2af9 997b 85f5  G..#=..]s&*..{..
+000024e0: 7b40 6e1c 7349 5c4b ba91 d58e 9c4f 9108  {@n.sI\K.....O..
+000024f0: 5f80 11a6 c9c5 1459 69ac 3aa3 c698 eb29  _......Yi.:....)
+00002500: 46c5 0876 6536 23cc cd14 a35d e868 04b8  F..ve6#....].h..
+00002510: 9d02 7889 c689 bb29 8236 0146 fc97 9325  ..x....).6.F...%
+00002520: d5ff bd25 0f6a 3ffd ede4 d266 3e28 5c6b  ...%.j?....f>(\k
+00002530: 1733 030d 4799 1d9d f37c 713b eaad 423e  .3..G....|q;..B>
+00002540: 0c9b bcf2 44de 0e62 cb3f 0430 39f0 7de3  ....D..b.?.09.}.
+00002550: 3d1d 94b4 6a87 4f57 fe00 504b 0304 1400  =...j.OW..PK....
+00002560: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00002570: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+00002580: 6865 6574 732f 7368 6565 7431 382e 786d  heets/sheet18.xm
+00002590: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
+000025a0: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
+000025b0: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
+000025c0: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
+000025d0: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
+000025e0: ebf6 dcd7 0e44 d181 b4e2 77d3 e903 d742  .....D....w....B
+000025f0: 1a96 c65d 6ce3 d2d8 36a8 a481 8d8b 7ca3  ...]l...6.....|.
+00002600: b570 c705 28db 266c c6ce 81ad dc57 d805  .p..(.&l.....W..
+00002610: 781a d762 0f3b c08f 9a00 e4f2 0b4f 2135  x..b.;.......O!5
+00002620: 182f ad89 1c94 097b 9ecd d73d a2cb f894  ./.....{...=....
+00002630: d0fa 1b3b 0acd 64d6 1e82 f356 246c 1a34  ...;..d....V$l.4
+00002640: 8182 1c03 85a0 cf0f 2c41 a9c0 444a be4f  ........,A..DJ.O
+00002650: a4ec 5a34 206f ed33 fdba eb9f e465 c2c3  ..Z4 o.3.....e..
+00002660: d2aa 2f59 6095 b027 1615 508a 46e1 d6b6  ../Y`..'..P.F...
+00002670: af70 eae9 fe2a 7125 50a4 b1b3 6de4 42b3  .p...*q%P...m.B.
+00002680: 699c 0723 94a4 4469 c290 76e8 282e a912  i..#..Di..v.(...
+00002690: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
+000026a0: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
+000026b0: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
+000026c0: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
+000026d0: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
+000026e0: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
+000026f0: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
+00002700: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00002710: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+00002720: 6865 6574 732f 7368 6565 7431 392e 786d  heets/sheet19.xm
+00002730: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
+00002740: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
+00002750: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
+00002760: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
+00002770: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
+00002780: ebf6 dcd7 0e44 d181 b4e2 77d3 e903 d742  .....D....w....B
+00002790: 1a96 c65d 6ce3 d2d8 36a8 a481 8d8b 7ca3  ...]l...6.....|.
+000027a0: b570 c705 28db 266c c6ce 81ad dc57 d805  .p..(.&l.....W..
+000027b0: 781a d762 0f3b c08f 9a00 e4f2 0b4f 2135  x..b.;.......O!5
+000027c0: 182f ad89 1c94 097b 9ecd d73d a2cb f894  ./.....{...=....
+000027d0: d0fa 1b3b 0acd 64d6 1e82 f356 246c 1a34  ...;..d....V$l.4
+000027e0: 8182 1c03 85a0 cf0f 2c41 a9c0 444a be4f  ........,A..DJ.O
+000027f0: a4ec 5a34 206f ed33 fdba eb9f e465 c2c3  ..Z4 o.3.....e..
+00002800: d2aa 2f59 6095 b027 1615 508a 46e1 d6b6  ../Y`..'..P.F...
+00002810: af70 eae9 fe2a 7125 50a4 b1b3 6de4 42b3  .p...*q%P...m.B.
+00002820: 699c 0723 94a4 4469 c290 76e8 282e a912  i..#..Di..v.(...
+00002830: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
+00002840: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
+00002850: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
+00002860: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
+00002870: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
+00002880: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
+00002890: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
+000028a0: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+000028b0: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+000028c0: 6865 6574 732f 7368 6565 7432 302e 786d  heets/sheet20.xm
+000028d0: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
+000028e0: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
+000028f0: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
+00002900: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
+00002910: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
+00002920: ebf6 dcd7 0e44 d181 b4e2 77d3 e903 d742  .....D....w....B
+00002930: 1a96 c65d 6ce3 d2d8 36a8 a481 8d8b 7ca3  ...]l...6.....|.
+00002940: b570 c705 28db 266c c6ce 81ad dc57 d805  .p..(.&l.....W..
+00002950: 781a d762 0f3b c08f 9a00 e4f2 0b4f 2135  x..b.;.......O!5
+00002960: 182f ad89 1c94 097b 9ecd d73d a2cb f894  ./.....{...=....
+00002970: d0fa 1b3b 0acd 64d6 1e82 f356 246c 1a34  ...;..d....V$l.4
+00002980: 8182 1c03 85a0 cf0f 2c41 a9c0 444a be4f  ........,A..DJ.O
+00002990: a4ec 5a34 206f ed33 fdba eb9f e465 c2c3  ..Z4 o.3.....e..
+000029a0: d2aa 2f59 6095 b027 1615 508a 46e1 d6b6  ../Y`..'..P.F...
+000029b0: af70 eae9 fe2a 7125 50a4 b1b3 6de4 42b3  .p...*q%P...m.B.
+000029c0: 699c 0723 94a4 4469 c290 76e8 282e a912  i..#..Di..v.(...
+000029d0: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
+000029e0: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
+000029f0: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
+00002a00: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
+00002a10: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
+00002a20: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
+00002a30: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
+00002a40: 0000 0800 d263 a858 19ef 2f38 7b01 0000  .....c.X../8{...
+00002a50: 4b03 0000 1900 0000 786c 2f77 6f72 6b73  K.......xl/works
+00002a60: 6865 6574 732f 7368 6565 7432 312e 786d  heets/sheet21.xm
+00002a70: 6c75 93db 4ec3 300c 865f a5ca 0390 81c4  lu..N.0.._......
+00002a80: 41a8 adc4 364e 1748 6808 b844 59eb ae11  A...6N.Hh..DY...
+00002a90: 3914 c7a5 8ca7 c7e9 8e48 ed55 6dc7 9ff3  9........H.Um...
+00002aa0: 3b76 d3ce e367 a801 28f9 b1c6 854c d444  ;v...g..(....L.D
+00002ab0: cdb5 94a1 a8c1 aa70 e21b 707c 5279 b48a  .......p..p|Ry..
+00002ac0: d8c5 950c 0d82 2a7b c81a 7936 995c 48ab  ......*{..y6.\H.
+00002ad0: b413 79da c79e 314f 7d4b 463b 78c6 24b4  ..y...1O}KF;x.$.
+00002ae0: d62a 5c4f c1f8 2e13 a762 1758 e855 4d7d  .*\O.....b.X.UM}
+00002af0: 40e6 69a3 56f0 02f4 da30 c0ae dcd7 29b5  @.i.V....0....).
+00002b00: 0517 b477 0942 9589 9bd3 ebfb 0dd1 67bc  ...w.B........g.
+00002b10: 69e8 c291 9dc4 6696 de7f 46e7 b1cc c424  i.....f...F....$
+00002b20: 6a02 0305 c512 8a3f df30 0363 6225 56f2  j......?.0.cb%V.
+00002b30: b52d 2a0e 9746 f2d8 de95 bfeb fb67 794b  .-*..F.......gyK
+00002b40: 1560 e6cd bb2e a9ce c495 484a a854 6b68  .`........HJ.Tkh
+00002b50: e1bb 07d8 f674 7e90 3857 a4f2 147d 9760  .....t~.8W...}.`
+00002b60: 6c36 4f8b 68c4 2b39 51bb f848 2f84 1cd7  l6O.h.+9Q..H/...
+00002b70: 7c13 e508 8150 f772 3fc0 fdae 2d84 5412  |....P.r?...-.T.
+00002b80: 0b8a c7b2 d8e2 d331 bcd0 58b4 46e1 0033  .......1..X.F..3
+00002b90: 1b63 5408 6097 663d c0cc c718 ed9a 9606  .cT.`.f=........
+00002ba0: 80db 3180 f761 98b8 1b23 68dd c040 fefd  ..1..a...#h..@..
+00002bb0: a8a4 f27f b6e4 37df 0d72 3384 b864 4f0a  ......7..r3..dO.
+00002bc0: 57da 85c4 40c5 5526 2797 3c2a dc4c 6de3  W...@.U&'.<*.Lm.
+00002bd0: 906f faa5 5c7a 226f 7bb3 e665 078c 097c  .o..\z"o{..e...|
+00002be0: 5e79 4f7b 276e cdfe ffc9 ff00 504b 0304  ^yO{'n......PK..
+00002bf0: 1400 0000 0800 d263 a858 caac fec0 7101  .......c.X....q.
+00002c00: 0000 3e03 0000 1900 0000 786c 2f77 6f72  ..>.......xl/wor
+00002c10: 6b73 6865 6574 732f 7368 6565 7432 322e  ksheets/sheet22.
+00002c20: 786d 6c75 93db 6e83 300c 407f 05e5 039a  xmlu..n.0.@.....
+00002c30: 76d2 2eaa 0069 6dd7 6e0f 93aa 56db 9e53  v....im.n...V..S
+00002c40: 3010 3517 9698 b1fe fd1c 7a9d 044f d88e  0.5.......z..O..
+00002c50: 8fef c4ad 757b 5f01 60f4 ab95 f109 ab10  ....u{_.`.......
+00002c60: eb29 e73e ab40 0b3f b235 187a 29ac d302  .).>.@.?.5.z)...
+00002c70: 4975 25f7 b503 9177 9056 fc6e 3c7e e05a  Iu%....w.V.n<~.Z
+00002c80: 48c3 d2b8 b3ad 5d1a db06 9534 b076 916f  H.....]....4.v.o
+00002c90: b416 ee30 0365 db84 4dd8 d9b0 9165 859d  ...0.e..M....e..
+00002ca0: 81a7 712d 4ad8 027e d404 90ca 2f71 72a9  ..q-J..~..../qr.
+00002cb0: c178 694d e4a0 48d8 f364 ba3a 129d c7a7  .xiM..H..d.:....
+00002cc0: 84d6 dfc8 5168 6667 ed3e 286f 79c2 c6a1  ....Qhfg.>(oy...
+00002cd0: 2650 9061 0821 e8f3 0373 502a 44a2 4abe  &P.a.!...sP*D.J.
+00002ce0: 4f41 d935 6920 6fe5 73f8 65d7 3f95 b713  OA.5i o.s.e.?...
+00002cf0: 1ee6 567d c91c ab84 3db1 2887 4234 0a37  ..V}....=.(.B4.7
+00002d00: b67d 8553 4ff7 d712 1702 451a 3bdb 462e  .}.SO.....E.;.F.
+00002d10: 349b c659 1042 4a72 9426 0c69 8b8e ec92  4..Y.BJr.&.i....
+00002d20: 3261 5a36 3207 1f73 a41a 8285 6727 6236  2aZ62..s....g'b6
+00002d30: 4464 d265 8d12 ae87 990f 31c2 7bd0 3b75  Dd.e......1.{.;u
+00002d40: e861 1643 8c34 7583 3dc0 cb10 4027 d04f  .a.C.4u.=...@'.O
+00002d50: 2c87 083c d4d0 e3bf 1a2c 29ff efcd 69cc  ,..<.....,)...i.
+00002d60: e7dd 1de7 1eee ea5d b852 1a1f 2928 28ca  .......].R..)((.
+00002d70: 78f4 48db 71c7 451d 15b4 7577 873b 8b68  x.H.q.E...uw.;.h
+00002d80: 7527 5674 dfe0 8203 bd17 d6e2 4509 8772  u'Vt........E..r
+00002d90: f965 d23f 504b 0304 1400 0000 0800 d263  .e.?PK.........c
+00002da0: a858 2513 3651 8301 0000 5703 0000 1900  .X%.6Q....W.....
+00002db0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00002dc0: 7368 6565 7432 332e 786d 6c75 53db 6edb  sheet23.xmluS.n.
+00002dd0: 300c fd15 431f 50a5 1bba 0d85 6d60 4d2f  0...C.P.....m`M/
+00002de0: dbc3 80a2 c5b6 c740 b169 5b88 246a 145d  .......@.i[.$j.]
+00002df0: af7f 3fca b9b4 03e2 2793 14cf e1e1 c5e5  ..?.....'.......
+00002e00: 84b4 4b03 0017 7fbd 0ba9 5203 73bc d63a  ..K.......R.s..:
+00002e10: 3503 7893 2e30 4290 970e c91b 1697 7a9d  5.x..0B.......z.
+00002e20: 2281 6967 9077 fac3 6af5 497b 6383 aacb  ".ig.w..j.I{c...
+00002e30: 39f6 4875 8923 3b1b e091 8a34 7a6f e8f5  9.Hu.#;....4zo..
+00002e40: 061c 4e95 ba54 c7c0 93ed 079e 03ba 2ea3  ..N..T..........
+00002e50: e9e1 19f8 6714 80b8 fac4 d35a 0f21 590c  ....g......Z.!Y.
+00002e60: 0541 57a9 af97 d70f 7bc4 9cf1 cbc2 94de  .AW.....{.......
+00002e70: d945 6e66 8bb8 cbce f7b6 52ab ac09 1c34  .Enf......R....4
+00002e80: 9c29 8c7c 5e60 0dce 6526 51f2 e740 aade  .).|^`..e&Q..@..
+00002e90: 8a66 e47b fb48 7f3f f72f f2b6 26c1 1add  .f.{.H.?./..&...
+00002ea0: 6fdb f250 a92f aa68 a133 a3e3 279c bec1  o..P./.h.3..'...
+00002eb0: a1a7 ab37 89b7 864d 5d12 4e05 e566 ebb2  ...7...M].N..f..
+00002ec0: c946 2e29 8936 e421 3d33 49dc 4a25 aef1  .F.).6.!=3I.J%..
+00002ed0: 0568 30a1 df34 649b dde6 6324 1940 a959  .h0..4d...c$.@.Y
+00002ee0: 24e5 04dd 1c08 6e96 0864 4f93 a176 83ce  $.....n..dO..v..
+00002ef0: f678 06b8 5e02 1248 e904 8bc0 db25 a00d  .x..^..H.....%..
+00002f00: 71e4 3380 bbc5 1e47 3e8f b85f 42f0 6b3c  q.3....G>.._B.k<
+00002f10: 3784 8745 49ed ffd9 5ae6 7f5c ea7e 21f9  7..EI...Z..\.~!.
+00002f20: e07e 18ea 6d48 8583 4e58 5617 9f65 6db4  .~..mH..NXV..em.
+00002f30: dfe0 de61 8cf3 816e 9119 fd6c 0e72 f840  ...a...n...l.r.@
+00002f40: 3941 de3b 443e 39f9 824e ff52 fd0f 504b  9A.;D>9..N.R..PK
+00002f50: 0304 1400 0000 0800 d263 a858 a50c 764f  .........c.X..vO
+00002f60: 5301 0000 a402 0000 1900 0000 786c 2f77  S...........xl/w
+00002f70: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00002f80: 342e 786d 6c75 52db 6ac3 300c fd95 e00f  4.xmluR.j.0.....
+00002f90: a8d3 c12e 9424 b0b6 8ced 6150 5ab6 3dbb  .....$....aPZ.=.
+00002fa0: 8992 98fa 365b 59d6 bf9f 9cf4 3668 9f2c  ....6[Y.....6h.,
+00002fb0: c93a 47e7 c8ce 7aeb 77a1 05c0 e457 2b13  .:G...z.w....W+.
+00002fc0: 72d6 22ba 19e7 a16c 418b 30b1 0e0c ddd4  r."....lA.0.....
+00002fd0: d66b 8194 fa86 07e7 4154 0348 2b7e 97a6  .k......AT.H+~..
+00002fe0: 0f5c 0b69 5891 0db5 952f 32db a192 0656  .\.iX..../2....V
+00002ff0: 3e09 9dd6 c2ef e7a0 6c9f b329 3b16 d6b2  >.......l..);...
+00003000: 6971 28f0 2273 a281 0de0 8723 00a5 fcc4  iq(."s.....#....
+00003010: 5349 0d26 486b 120f 75ce 9ea7 b3e5 8818  SI.&Hk..u.......
+00003020: 3a3e 25f4 e122 4ea2 99ad b5bb 98bc 5539  :>%.."N.......U9
+00003030: 4ba3 2650 5062 a410 74fc c002 948a 4ca4  K.&PPb..t.....L.
+00003040: e4fb 40ca ce43 23f2 323e d2bf 0cfe 49de  ..@..C#.2>....I.
+00003050: 5604 5858 f525 2b6c 73f6 c492 0a6a d129  V.XX.%+ls....j.)
+00003060: 5cdb fe15 0e9e eecf 1297 0245 9179 db27  \..........E.y.'
+00003070: 3e9a 2db2 3206 7124 354a 1397 b441 4f75  >.-.2.q$5J...AOu
+00003080: 4993 b090 c675 9871 2409 b1c0 cb03 607e  I....u.q$.....`~
+00003090: 0b40 8bbe 8e58 dc42 e0de c195 fee5 4d49  .@...X.B......MI
+000030a0: d5ff 6e4e 668e 1b1a ddc5 d77b 17be 9126  ..nNf......{...&
+000030b0: 240a 6a62 4927 8fb4 033f ae63 4cd0 bae1  $.jbI'...?.cL...
+000030c0: b5b7 16d1 ea21 6ce9 1781 8f0d 745f 5b8b  .....!l.....t_[.
+000030d0: a724 3ec7 e963 167f 504b 0304 1400 0000  .$>..c..PK......
+000030e0: 0800 d263 a858 6517 5607 5c01 0000 b502  ...c.Xe.V.\.....
+000030f0: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00003100: 6574 732f 7368 6565 7432 352e 786d 6c75  ets/sheet25.xmlu
+00003110: 52db 4ec3 300c fd95 2a1f b06c 485c 84da  R.N.0...*..lH\..
+00003120: 4ab0 09c1 03d2 0402 9eb3 d65d 2392 b873  J..........]#..s
+00003130: 5c0a 7f8f d35d 91d8 536c 27e7 d8e7 38f9  \....]..Sl'...8.
+00003140: 80f4 195b 00ce bebd 0bb1 502d 7377 ab75  ...[......P-sw.u
+00003150: ac5a f026 4eb0 8320 370d 9237 2c29 ad75  .Z.&N.. 7..7,).u
+00003160: ec08 4c3d 82bc d317 d3e9 95f6 c606 55e6  ..L=..........U.
+00003170: 636d 4965 8e3d 3b1b 6049 59ec bd37 f473  cmIe.=;.`IY..7.s
+00003180: 0f0e 8742 cdd4 bef0 62d7 2d8f 055d e69d  ...B....b.-..]..
+00003190: 59c3 2bf0 5b27 0049 f581 a7b6 1e42 b418  Y.+.['.I.....B..
+000031a0: 3282 a650 77b3 dbc5 1631 be78 b730 c493  2..Pw....1.x.0..
+000031b0: 384b 6256 889f 2979 aa0b 354d 3381 838a  8KbV..)y..5M3...
+000031c0: 1385 91e3 0be6 e05c 6292 4936 3b52 756c  .......\b.I6;Rul
+000031d0: 9a90 a7f1 9efe 61d4 2fe3 ad4c 8439 ba0f  ......a./..L.9..
+000031e0: 5b73 5ba8 1b95 d5d0 98de f10b 0e8f b0d3  [s[.............
+000031f0: 7479 1c71 61d8 9439 e190 5112 5be6 550a  ty.qa..9..Q.[.U.
+00003200: 524b 7968 4332 e995 49ea 563a 7119 61d3  RKyhC2..I.V:q.a.
+00003210: 43a8 20e6 9a65 8c54 d4d5 0e74 7f16 843d  C. ..e.T...t...=
+00003220: fd0f 999f 8374 24c6 d27f 90c5 3948 0db1  .....t$.....9H..
+00003230: 22db 2527 ffc2 b4a8 db5b b695 9bd6 f96c  ".%'.....[.....l
+00003240: 686d 43cc 1c34 4237 9d5c 8b29 b4f5 679b  hmC..4B7.\.)..g.
+00003250: 3076 e3fa 57c8 8c7e 0c5b f956 40e9 81dc  0v..W..~.[.V@...
+00003260: 3788 7c48 d27e 0e3f b5fc 0550 4b03 0414  7.|H.~.?...PK...
+00003270: 0000 0008 00d2 63a8 58d2 05f1 4652 0200  ......c.X...FR..
+00003280: 0047 0a00 000d 0000 0078 6c2f 7374 796c  .G.......xl/styl
+00003290: 6573 2e78 6d6c dd56 db8a db30 10fd 15e3  es.xml.V...0....
+000032a0: 0fa8 9398 9ab8 2479 a821 5068 cbc2 ee43  ......$y.!Ph...C
+000032b0: 5fe5 584e 04ba b8b2 bc24 fdfa 6a24 e7b6  _.XN.....$..j$..
+000032c0: 9be3 52fa 569b e099 393a 3367 a431 ceaa  ..R.V...9:3g.1..
+000032d0: 7727 c99f 0f9c bbe4 a8a4 eed7 e9c1 b9ee  w'..............
+000032e0: 5396 f5bb 0357 acff 603a ae3d d21a ab98  S....W..`:.=....
+000032f0: f3ae dd67 7d67 396b 7a22 2999 2d66 b322  ...g}g9kz").-f."
+00003300: 534c e874 b3d2 83da 2ad7 273b 3368 b74e  SL.t....*.';3h.N
+00003310: 6769 926d 56ad d1d7 d03c 8d01 bf96 299e  gi.mV....<....).
+00003320: bc32 b94e 2b26 456d 455c cc94 90a7 185f  .2.N+&EmE\....._
+00003330: 84c8 ce48 6313 e7d5 70a2 53a8 ff15 17cc  ...Hc...p.S.....
+00003340: 4797 a48e b994 d0c6 8668 16cb 8447 ef13  G........h...G..
+00003350: 0b29 2f2a 1669 0c6c 561d 738e 5bbd f54e  .)/*.i.lV.s.[..N
+00003360: 2485 e87b 6cb4 5f4e 9d57 b1b7 ec34 5f7c  $..{l._N.W...4_|
+00003370: 4c6f 18e1 e1cb d4c6 36dc deb5 1b43 9b95  Lo......6....C..
+00003380: e4ad 2386 15fb 4330 9ce9 e851 1be7 8c22  ..#...C0...Q..."
+00003390: ab11 6c6f 348b 4ace b4d1 f0b9 775c ca67  ..lo4.J.....w\.g
+000033a0: 3aaf 1fed 5d81 639b c48d ffd2 843d a78e  :...].c......=..
+000033b0: cfa6 5735 9a31 cde8 5081 db74 31f9 bfe7  ..W5.1..P..t1...
+000033c0: edc4 ab71 9f07 df90 0efe cfc1 38fe 6479  ...q........8.dy
+000033d0: 2b8e c13f b66f 045c 6a07 2577 e52f d184  +..?.o.\j.%w./..
+000033e0: 4665 9d7e a711 9437 39ea 4148 27f4 e81d  Fe.~...79.AH'...
+000033f0: 44d3 70fd be3b 9fdf b1da 0ff9 5d01 bfaa  D.p..;......]...
+00003400: e12d 1ba4 7bb9 80eb f46a 7fe3 8d18 5479  .-..{....j....Ty
+00003410: 59f5 448d 8dab aef6 573a ca79 719d 535f  Y.D.....W:.yq.S_
+00003420: 4ce8 861f 7953 8dae ddd7 c14c bce1 cb8e  L...yS.....L....
+00003430: 5760 bc85 b6e1 0210 6445 1040 04c2 5a50  W`......dE.@..ZP
+00003440: 0664 451e acf5 3ff6 b5c4 7d45 102a 5c3e  .dE...?...}E.*\>
+00003450: 8696 98b5 c4ac c87b 0855 e186 b500 abf4  .......{.U......
+00003460: 1768 b92c f3bc 28e0 f656 d563 1915 dcc3  .h.,..(..V.c....
+00003470: a2a0 1f48 0815 1207 d6a2 6a7f bbf3 1303  ...H......j.....
+00003480: 3031 367f 980d 78ca 9363 035b 9e18 51d8  016...x..c.[..Q.
+00003490: f2c4 ce13 04f6 9038 6509 0600 d622 0e3c  .......8e....".<
+000034a0: 1438 5124 02d4 a251 03ac 3ca7 7386 0ae1  .8Q$...Q..<.s...
+000034b0: 6b3e 0195 2584 6848 c1f4 1605 daa8 826e  k>..%.hH.......n
+000034c0: 705e f025 caf3 b204 1081 4046 9e43 885e  p^.%......@F.C.^
+000034d0: d809 08ca 2021 10ca f3f8 217d f33d cbce  .... !....!}.=..
+000034e0: dfb9 ecfa d771 f31b 504b 0304 1400 0000  .....q..PK......
+000034f0: 0800 d263 a858 b747 eb8a c000 0000 1602  ...c.X.G........
+00003500: 0000 0b00 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+00003510: 739d 924b 6e02 310c 40af 1265 5f4c a9c4  s..Kn.1.@..e_L..
+00003520: 0231 acd8 b043 880b b889 e7a3 99c4 9163  .1...C.........c
+00003530: c4f4 f68d d8c0 2068 114b ff9e 9e2d af0f  ...... h.K...-..
+00003540: 34a0 761c 73db a56c c630 c45c d956 35ad  4.v.s..l.0.\.V5.
+00003550: 00b2 6b29 609e 71a2 582a 354b 402d a134  ..k)`.q.X*5K@-.4
+00003560: 90d0 f5d8 102c e6f3 25c8 2dc3 6ed6 b74c  .....,..%.-.n..L
+00003570: 73fc 49f4 0a91 ebba 73b4 6577 0a14 f501  s.I.....s.ew....
+00003580: f8ae c39a 234a 435a d971 8033 4bff cddc  ....#JCZ.q.3K...
+00003590: cf0a d49a 9daf acec fca7 35f0 a6cc f3f5  ..........5.....
+000035a0: 2090 a247 4570 2cf4 91a4 4c8b 7694 af3e   ..GEp,...L.v..>
+000035b0: 9edd bea4 f3a5 6362 b478 dfe8 fff3 d0a8  ......cb.x......
+000035c0: 143d f9bf 9d30 a589 d2d7 4509 266f b0f9  .=...0....E.&o..
+000035d0: 0550 4b03 0414 0000 0008 00d2 63a8 58e7  .PK.........c.X.
+000035e0: f3f0 5ba5 0200 005f 0900 000f 0000 0078  ..[...._.......x
+000035f0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 8d96  l/workbook.xml..
+00003600: 6f6f 9b30 10c6 bf4a c407 1881 b6e9 1f35  oo.0...J.......5
+00003610: 952a dab5 99ba 350a 59df 1b7c 494e b57d  .*....5.Y..|IN.}
+00003620: cc36 6dc9 a79f 0165 6533 b1f6 26c4 67fb  .6m....ee3..&.g.
+00003630: c79d 791e dbd7 efa4 5f0b a2d7 c987 14ca  ..y....._.......
+00003640: 5ce9 79b4 b3b6 ba8a 6353 ee40 32f3 852a  \.y.....cS.@2..*
+00003650: 50ae 6f43 5a32 eb9a 7a1b d366 8325 dc51  P.oCZ2..z..f.%.Q
+00003660: 594b 5036 4ea7 d359 ac41 308b a4cc 0e2b  YKP6N..Y.A0....+
+00003670: 13f5 b4ff 6199 4a03 e366 0760 a5e8 5192  ....a.J..f.`..Q.
+00003680: a18a 6eae 0f99 2df5 241e b6c8 42d9 bea9  ..n...-.$...B...
+00003690: 8db6 9117 8477 f339 a06d 4ede d060 8102  .....w.9.mN..`..
+000036a0: 6d33 8fba ff02 a289 4485 12f7 c0e7 d134  m3......D......4
+000036b0: 9a98 1dbd 3f92 c63d 29cb 445e 6a12 621e  ....?..=).D^j.b.
+000036c0: 257d c70b 688b a517 cedb 34d7 ac30 5dc4  %}..h.....4..0].
+000036d0: b262 d5d6 3c8f 6653 07dc a036 b61b d1f1  .b..<.fS...6....
+000036e0: 994b f20d dce0 be55 5bfa 8ac2 82be 6316  .K.....U[.....c.
+000036f0: 1e34 d515 aa6d 8771 65c4 833a baa5 383c  .4...m.qe..:..8<
+00003700: 278a 4998 473f dc2f 5fef dc8c 360f 175f  '.I.G?./_...6.._
+00003710: f03e 27eb 6083 0af5 15ba 0ebd e03d 7688  .>'.`........=v.
+00003720: 58c3 8775 0940 0ebf 6a50 250c 4069 0094  X..u.@..jP%.@i..
+00003730: 7aa0 a546 097a 30fd 2430 fdc4 9b7e 787f  z..F.z0.$0...~x.
+00003740: 56db 01e3 34c0 38f5 182b 3056 6327 8271  V...4.8..+0Vc'.q
+00003750: dc59 0077 e6e1 be33 5533 219a 7553 01cf  .Y.w...3U3!.uS..
+00003760: a9d6 7fad ce2c c09a 79ac 9f95 20c6 8177  .....,..y... ..w
+00003770: 4bfd 2fea 3c80 3a1f a9b2 2283 9674 b3f0  K./.<.:..."..t..
+00003780: b3ba 08a0 2e3c d42d e70f a060 8473 19e0  .....<.-...`.s..
+00003790: 5c7a 1c07 2109 1991 e6a8 dc2c e3f1 9269  \z..!......,...i
+000037a0: 4895 d390 1c7c 5650 e1be c407 b2b8 57fb  H....|VP......W.
+000037b0: 46c2 1d6e 5da8 5589 870e 693e f145 9fa3  F..n].U...i>.E..
+000037c0: ac3e bdf3 4465 b7d7 0d81 2117 24be 0d6e  .>..De....!.$..n
+000037d0: 8d01 5988 e61b a1ca 4856 a4dc 4e3a e485  ..Y.....HV..N:..
+000037e0: 1c91 f896 18f2 8698 9013 12df 0a07 8cbf  ................
+000037f0: 6021 1b24 be0f 96d9 ca67 84f4 9ff8 0678  `!.$.....g.....x
+00003800: c22d 1bff 7a21 f527 befc 1f49 92a0 2dd5  .-..z!.'...I..-.
+00003810: 6605 25c9 a2d5 ee28 37e4 8664 c40e 5818  f.%....(7..d..X.
+00003820: 5247 d72c 0d79 21f5 bd30 d0ef ade2 47ab  RG.,.y!..0....G.
+00003830: 4f43 b648 7d5b 64ab 45be f4bf 461a dcf6  OC.H}[d.E...F...
+00003840: 7d0b 3c0b dcd2 6353 68e4 b83f 9259 c804  }.<...cSh..?.Y..
+00003850: a96f 8225 09e7 52cd 0cdc 7f58 5066 9419  .o.%..R....XPf..
+00003860: 3242 ea1b 2113 a4dc 3999 5bed e66c 9b21  2B..!...9.[..l.!
+00003870: 29e4 85b4 f742 7c38 7d39 6c50 016f 0f5e  )....B|8}9lP.o.^
+00003880: d376 b8bb 40e9 2e22 eda3 df3f 4ecf 5a41  .v..@.."...?N.ZA
+00003890: 6c6a 2132 177b 564f 6edb ff73 9c1f ee22  lj!2.{VOn..s..."
+000038a0: 37bf 0150 4b03 0414 0000 0008 00d2 63a8  7..PK.........c.
+000038b0: 58f9 efd8 af3c 0100 00cd 0f00 001a 0000  X....<..........
+000038c0: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
+000038d0: 6f6b 2e78 6d6c 2e72 656c 73cd d741 8e82  ok.xml.rels..A..
+000038e0: 3014 c6f1 ab90 1ec0 f29e 8a3a 1157 6edc  0..........:.Wn.
+000038f0: 4ebc 4083 1588 4049 dbc9 e8ed 87c8 023f  N.@...@I.......?
+00003900: 328b d998 792b d212 1eff 4d7f 81fd a76d  2...y+....M....m
+00003910: 4cac 5d17 aaba 0fc9 bd6d ba90 ab2a c6fe  L.]......m...*..
+00003920: 43eb 5054 b635 61e1 7adb 0d77 aece b726  C.PT.5a.z..w...&
+00003930: 0e4b 5fea de14 3753 5acd 699a 69ff 3a43  .K_...7SZ.i.i.:C
+00003940: 1df6 af33 93f3 a3b7 7f99 e8ae d7ba b047  ...3...........G
+00003950: 577c b5b6 8bbf 0cd6 dfce df42 656d 54c9  W|.........BemT.
+00003960: d9f8 d2c6 5ce9 7b33 6d07 fdbc d062 98ac  ....\.{3m....b..
+00003970: 92d3 2557 fe74 2195 e8ff 2e62 2862 0145  ..%W.t!....b(b.E
+00003980: 4b28 5a0a 285a 41d1 4a40 d11a 8ad6 028a  K(Z.(ZA.J@......
+00003990: 3228 ca04 146d a068 23a0 680b 455b 0145  2(...m.h#.h.E[.E
+000039a0: 3b28 da09 28a2 1489 4c25 34cd d896 e036  ;(..(...L%4....6
+000039b0: 21dc 2441 6e42 ba49 82dd 8478 9304 bd09  !.$AnB.I...x....
+000039c0: f926 097e 1302 4e12 0427 249c 2418 4e88  .&.~..N..'$.$.N.
+000039d0: 3849 509c 9071 92e0 38a3 e32c c171 46c7  8IP..q..8..,.qF.
+000039e0: 5982 e33c fb00 97e0 38a3 e32c c171 46c7  Y..<....8..,.qF.
+000039f0: 5982 e38c 8ef3 5b1d 0ff1 d1d8 3005 8d6b  Y.....[.....0..k
+00003a00: 0c78 2bda 7178 d64e ef7f 2ec7 cdd9 b11a  .x+.qx.N........
+00003a10: 99d6 f0f7 7ef8 0150 4b03 0414 0000 0008  ....~..PK.......
+00003a20: 00d2 63a8 5872 079d 5874 0100 00bf 1000  ..c.Xr..Xt......
+00003a30: 0013 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
+00003a40: 7065 735d 2e78 6d6c cd98 cb6e c230 1045  pes].xml...n.0.E
+00003a50: 7f25 ca16 1163 b7a5 0f01 9bb6 db96 457f  .%...c........E.
+00003a60: c04d 26c4 c22f d986 c2df 7712 0a52 2bca  .M&../....w..R+.
+00003a70: 4354 ea6c 6225 9eb9 f7c6 231d 2919 bdad  CT.lb%....#.)...
+00003a80: 3dc4 6c65 b48d e3bc 49c9 3f30 16cb 068c  =.le....I.?0....
+00003a90: 8c85 f360 71a7 76c1 c884 b761 c6bc 2ce7  ...`q.v....a..,.
+00003aa0: 7206 4c0c 0643 563a 9bc0 a67e 6a35 f2c9  r.L..CV:...~j5..
+00003ab0: e809 6ab9 d029 7b5e e1e3 a89c 1de7 0174  ..j..){^.......t
+00003ac0: ccb3 c74d 61eb 35ce a5f7 5a95 32e1 3e5b  ...Ma.5...Z.2.>[
+00003ad0: daea 874b ffcb a1c0 ceae 2636 cac7 1e16  ...K......&6....
+00003ae0: e419 db6b d16d fdea b06d 7c5d 4208 aa82  ...k.m...m|]B...
+00003af0: 6c2a 437a 9106 cbd8 4ab3 98d6 1a62 7158  l*Cz....J....bqX
+00003b00: 634f 4a57 d7aa 84ca 950b 832d 45f4 0164  cOJW.......-E..d
+00003b10: 151b 8064 74b1 11ed 1db1 4e78 c8b0 b9f2  ...dt.....Nx....
+00003b20: 8b03 7432 071d b174 1a9c 8f38 b500 e7fb  ..t2...t...8....
+00003b30: 6dc7 d276 f73d 0a41 48ea c84b ee2c 51fb  m..v.=.AH..K.,Q.
+00003b40: e237 8476 e215 54a7 9ae3 097f b830 ef66  .7.v..T......0.f
+00003b50: 1259 b75c 7ecc dfe7 bcd3 3f37 88a0 12e4  .Y.\~.....?7....
+00003b60: 8a4a 906b 2a41 6ea8 0419 5209 724b 25c8  .J.k*An...R.rK%.
+00003b70: 1d95 20f7 5482 f001 9924 64d8 cac9 c095  .. .T....$d.....
+00003b80: 93a1 2b27 8357 4e86 af9c 0c60 3919 c272  ..+'.WN....`9..r
+00003b90: 3288 e564 182b c830 5690 61ac 20c3 5841  2..d.+.0V.a. .XA
+00003ba0: 86b1 820c 63c5 bf32 f6dd b9f9 5f7f 4fb7  ....c..2...._.O.
+00003bb0: 6b61 a4b2 bb00 acfb 6f31 f904 504b 0102  ka......o1..PK..
+00003bc0: 1403 1400 0000 0800 d263 a858 465a c10c  .........c.XFZ..
+00003bd0: 8200 0000 b100 0000 1000 0000 0000 0000  ................
+00003be0: 0000 0000 8001 0000 0000 646f 6350 726f  ..........docPro
+00003bf0: 7073 2f61 7070 2e78 6d6c 504b 0102 1403  ps/app.xmlPK....
+00003c00: 1400 0000 0800 d263 a858 9d88 5136 ee00  .......c.X..Q6..
+00003c10: 0000 cb01 0000 1100 0000 0000 0000 0000  ................
+00003c20: 0000 8001 b000 0000 646f 6350 726f 7073  ........docProps
+00003c30: 2f63 6f72 652e 786d 6c50 4b01 0214 0314  /core.xmlPK.....
+00003c40: 0000 0008 00d2 63a8 5899 5c9c 2310 0600  ......c.X.\.#...
+00003c50: 009c 2700 0013 0000 0000 0000 0000 0000  ..'.............
+00003c60: 0080 01cd 0100 0078 6c2f 7468 656d 652f  .......xl/theme/
+00003c70: 7468 656d 6531 2e78 6d6c 504b 0102 1403  theme1.xmlPK....
+00003c80: 1400 0000 0800 d263 a858 bbe8 8b38 3801  .......c.X...88.
+00003c90: 0000 1102 0000 1800 0000 0000 0000 0000  ................
+00003ca0: 0000 8081 0e08 0000 786c 2f77 6f72 6b73  ........xl/works
+00003cb0: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
+00003cc0: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00003cd0: 0712 deaa ee01 0000 2104 0000 1800 0000  ........!.......
+00003ce0: 0000 0000 0000 0000 8081 7c09 0000 786c  ..........|...xl
+00003cf0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00003d00: 7432 2e78 6d6c 504b 0102 1403 1400 0000  t2.xmlPK........
+00003d10: 0800 d263 a858 a497 6e89 5601 0000 a502  ...c.X..n.V.....
+00003d20: 0000 1800 0000 0000 0000 0000 0000 8081  ................
+00003d30: a00b 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00003d40: 732f 7368 6565 7433 2e78 6d6c 504b 0102  s/sheet3.xmlPK..
+00003d50: 1403 1400 0000 0800 d263 a858 32c0 66ed  .........c.X2.f.
+00003d60: 4c01 0000 4d02 0000 1800 0000 0000 0000  L...M...........
+00003d70: 0000 0000 8081 2c0d 0000 786c 2f77 6f72  ......,...xl/wor
+00003d80: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
+00003d90: 6d6c 504b 0102 1403 1400 0000 0800 d263  mlPK...........c
+00003da0: a858 0840 26f8 5c01 0000 8b02 0000 1800  .X.@&.\.........
+00003db0: 0000 0000 0000 0000 0000 8081 ae0e 0000  ................
+00003dc0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00003dd0: 6565 7435 2e78 6d6c 504b 0102 1403 1400  eet5.xmlPK......
+00003de0: 0000 0800 d263 a858 4ec7 5d80 8a01 0000  .....c.XN.].....
+00003df0: 9103 0000 1800 0000 0000 0000 0000 0000  ................
+00003e00: 8081 4010 0000 786c 2f77 6f72 6b73 6865  ..@...xl/workshe
+00003e10: 6574 732f 7368 6565 7436 2e78 6d6c 504b  ets/sheet6.xmlPK
+00003e20: 0102 1403 1400 0000 0800 d263 a858 4409  ...........c.XD.
+00003e30: 9006 e701 0000 3704 0000 1800 0000 0000  ......7.........
+00003e40: 0000 0000 0000 8081 0012 0000 786c 2f77  ............xl/w
+00003e50: 6f72 6b73 6865 6574 732f 7368 6565 7437  orksheets/sheet7
+00003e60: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00003e70: d263 a858 91c1 008b d201 0000 f603 0000  .c.X............
+00003e80: 1800 0000 0000 0000 0000 0000 8081 1d14  ................
+00003e90: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00003ea0: 7368 6565 7438 2e78 6d6c 504b 0102 1403  sheet8.xmlPK....
+00003eb0: 1400 0000 0800 d263 a858 d3d7 629c 0b02  .......c.X..b...
+00003ec0: 0000 3105 0000 1800 0000 0000 0000 0000  ..1.............
+00003ed0: 0000 8081 2516 0000 786c 2f77 6f72 6b73  ....%...xl/works
+00003ee0: 6865 6574 732f 7368 6565 7439 2e78 6d6c  heets/sheet9.xml
+00003ef0: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00003f00: 1a82 8f86 9c01 0000 1a04 0000 1900 0000  ................
+00003f10: 0000 0000 0000 0000 8081 6618 0000 786c  ..........f...xl
+00003f20: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00003f30: 7431 302e 786d 6c50 4b01 0214 0314 0000  t10.xmlPK.......
+00003f40: 0008 00d2 63a8 5882 b2f4 9d67 0100 000f  ....c.X....g....
+00003f50: 0300 0019 0000 0000 0000 0000 0000 0080  ................
+00003f60: 8139 1a00 0078 6c2f 776f 726b 7368 6565  .9...xl/workshee
+00003f70: 7473 2f73 6865 6574 3131 2e78 6d6c 504b  ts/sheet11.xmlPK
+00003f80: 0102 1403 1400 0000 0800 d263 a858 82b2  ...........c.X..
+00003f90: f49d 6701 0000 0f03 0000 1900 0000 0000  ..g.............
+00003fa0: 0000 0000 0000 8081 d71b 0000 786c 2f77  ............xl/w
+00003fb0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00003fc0: 322e 786d 6c50 4b01 0214 0314 0000 0008  2.xmlPK.........
+00003fd0: 00d2 63a8 58fb c712 8d4a 0100 0075 0200  ..c.X....J...u..
+00003fe0: 0019 0000 0000 0000 0000 0000 0080 8175  ...............u
+00003ff0: 1d00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00004000: 2f73 6865 6574 3133 2e78 6d6c 504b 0102  /sheet13.xmlPK..
+00004010: 1403 1400 0000 0800 d263 a858 f666 8318  .........c.X.f..
+00004020: 5c01 0000 8b02 0000 1900 0000 0000 0000  \...............
+00004030: 0000 0000 8081 f61e 0000 786c 2f77 6f72  ..........xl/wor
+00004040: 6b73 6865 6574 732f 7368 6565 7431 342e  ksheets/sheet14.
+00004050: 786d 6c50 4b01 0214 0314 0000 0008 00d2  xmlPK...........
+00004060: 63a8 580c 5719 2b43 0100 0044 0200 0019  c.X.W.+C...D....
+00004070: 0000 0000 0000 0000 0000 0080 8189 2000  .............. .
+00004080: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00004090: 6865 6574 3135 2e78 6d6c 504b 0102 1403  heet15.xmlPK....
+000040a0: 1400 0000 0800 d263 a858 44ff 8108 6901  .......c.XD...i.
+000040b0: 0000 0c03 0000 1900 0000 0000 0000 0000  ................
+000040c0: 0000 8081 0322 0000 786c 2f77 6f72 6b73  ....."..xl/works
+000040d0: 6865 6574 732f 7368 6565 7431 362e 786d  heets/sheet16.xm
+000040e0: 6c50 4b01 0214 0314 0000 0008 00d2 63a8  lPK...........c.
+000040f0: 5811 26ee aa80 0100 0080 0300 0019 0000  X.&.............
+00004100: 0000 0000 0000 0000 0080 81a3 2300 0078  ............#..x
+00004110: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00004120: 6574 3137 2e78 6d6c 504b 0102 1403 1400  et17.xmlPK......
+00004130: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00004140: 0c03 0000 1900 0000 0000 0000 0000 0000  ................
+00004150: 8081 5a25 0000 786c 2f77 6f72 6b73 6865  ..Z%..xl/workshe
+00004160: 6574 732f 7368 6565 7431 382e 786d 6c50  ets/sheet18.xmlP
+00004170: 4b01 0214 0314 0000 0008 00d2 63a8 5844  K...........c.XD
+00004180: ff81 0869 0100 000c 0300 0019 0000 0000  ...i............
+00004190: 0000 0000 0000 0080 81fa 2600 0078 6c2f  ..........&..xl/
+000041a0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+000041b0: 3139 2e78 6d6c 504b 0102 1403 1400 0000  19.xmlPK........
+000041c0: 0800 d263 a858 44ff 8108 6901 0000 0c03  ...c.XD...i.....
+000041d0: 0000 1900 0000 0000 0000 0000 0000 8081  ................
+000041e0: 9a28 0000 786c 2f77 6f72 6b73 6865 6574  .(..xl/worksheet
+000041f0: 732f 7368 6565 7432 302e 786d 6c50 4b01  s/sheet20.xmlPK.
+00004200: 0214 0314 0000 0008 00d2 63a8 5819 ef2f  ..........c.X../
+00004210: 387b 0100 004b 0300 0019 0000 0000 0000  8{...K..........
+00004220: 0000 0000 0080 813a 2a00 0078 6c2f 776f  .......:*..xl/wo
+00004230: 726b 7368 6565 7473 2f73 6865 6574 3231  rksheets/sheet21
+00004240: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00004250: d263 a858 caac fec0 7101 0000 3e03 0000  .c.X....q...>...
+00004260: 1900 0000 0000 0000 0000 0000 8081 ec2b  ...............+
+00004270: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00004280: 7368 6565 7432 322e 786d 6c50 4b01 0214  sheet22.xmlPK...
+00004290: 0314 0000 0008 00d2 63a8 5825 1336 5183  ........c.X%.6Q.
+000042a0: 0100 0057 0300 0019 0000 0000 0000 0000  ...W............
+000042b0: 0000 0080 8194 2d00 0078 6c2f 776f 726b  ......-..xl/work
+000042c0: 7368 6565 7473 2f73 6865 6574 3233 2e78  sheets/sheet23.x
+000042d0: 6d6c 504b 0102 1403 1400 0000 0800 d263  mlPK...........c
+000042e0: a858 a50c 764f 5301 0000 a402 0000 1900  .X..vOS.........
+000042f0: 0000 0000 0000 0000 0000 8081 4e2f 0000  ............N/..
+00004300: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00004310: 6565 7432 342e 786d 6c50 4b01 0214 0314  eet24.xmlPK.....
+00004320: 0000 0008 00d2 63a8 5865 1756 075c 0100  ......c.Xe.V.\..
+00004330: 00b5 0200 0019 0000 0000 0000 0000 0000  ................
+00004340: 0080 81d8 3000 0078 6c2f 776f 726b 7368  ....0..xl/worksh
+00004350: 6565 7473 2f73 6865 6574 3235 2e78 6d6c  eets/sheet25.xml
+00004360: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00004370: d205 f146 5202 0000 470a 0000 0d00 0000  ...FR...G.......
+00004380: 0000 0000 0000 0000 8001 6b32 0000 786c  ..........k2..xl
+00004390: 2f73 7479 6c65 732e 786d 6c50 4b01 0214  /styles.xmlPK...
+000043a0: 0314 0000 0008 00d2 63a8 58b7 47eb 8ac0  ........c.X.G...
+000043b0: 0000 0016 0200 000b 0000 0000 0000 0000  ................
+000043c0: 0000 0080 01e8 3400 005f 7265 6c73 2f2e  ......4.._rels/.
+000043d0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
+000043e0: d263 a858 e7f3 f05b a502 0000 5f09 0000  .c.X...[...._...
+000043f0: 0f00 0000 0000 0000 0000 0000 8001 d135  ...............5
+00004400: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00004410: 6c50 4b01 0214 0314 0000 0008 00d2 63a8  lPK...........c.
+00004420: 58f9 efd8 af3c 0100 00cd 0f00 001a 0000  X....<..........
+00004430: 0000 0000 0000 0000 0080 01a3 3800 0078  ............8..x
+00004440: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00004450: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
+00004460: 0000 0008 00d2 63a8 5872 079d 5874 0100  ......c.Xr..Xt..
+00004470: 00bf 1000 0013 0000 0000 0000 0000 0000  ................
+00004480: 0080 0117 3a00 005b 436f 6e74 656e 745f  ....:..[Content_
+00004490: 5479 7065 735d 2e78 6d6c 504b 0506 0000  Types].xmlPK....
+000044a0: 0000 2100 2100 de08 0000 bc3b 0000 0000  ..!.!......;....
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/graphql/shareyourcloning_linkml.graphql` & `shareyourcloning_linkml-0.1.4a0/project/graphql/shareyourcloning_linkml.graphql`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,23 @@
     repositoryId: String!
     sequenceFileUrl: String
     addgeneSequenceType: AddGeneSequenceType
   }
 
 type AssemblyJoin
   {
-    leftFragment: Sequence!
-    rightFragment: Sequence!
-    leftLocation: SimpleSequenceLocation!
-    rightLocation: SimpleSequenceLocation!
+    left: AssemblyJoinComponent!
+    right: AssemblyJoinComponent!
+  }
+
+type AssemblyJoinComponent
+  {
+    sequence: Sequence!
+    location: SimpleSequenceLocation!
+    reverseComplemented: Boolean!
   }
 
 type AssemblySource
   {
     id: Integer!
     input: [Sequence]
     output: Sequence
@@ -239,8 +244,7 @@
     input: [Sequence]
     output: Sequence
     type: String
     sequenceFileFormat: SequenceFileFormat!
     fileName: String
     indexInFile: Integer
   }
-
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.context.jsonld` & `shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.context.jsonld`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9318627450980392%*

 * *Differences: {"'@context'": "{'left': OrderedDict([('@type', '@id'), ('@id', 'left')]), 'right': "*

 * *               "OrderedDict([('@type', '@id'), ('@id', 'right')]), 'location': "*

 * *               "OrderedDict([('@type', '@id'), ('@id', 'location')]), 'reverse_complemented': "*

 * *               "OrderedDict([('@type', 'xsd:boolean'), ('@id', 'reverse_complemented')]), "*

 * *               "'AssemblyJoinComponent': OrderedDict([('@id', 'AssemblyJoinComponent')]), delete: "*

 * *               "['left_fragment', 'left_location', 'right […]*

```diff
@@ -3,14 +3,17 @@
         "@vocab": "https://w3id.org/genestorian/ShareYourCloning_LinkML/",
         "AddGeneIdSource": {
             "@id": "AddGeneIdSource"
         },
         "AssemblyJoin": {
             "@id": "AssemblyJoin"
         },
+        "AssemblyJoinComponent": {
+            "@id": "AssemblyJoinComponent"
+        },
         "AssemblySource": {
             "@id": "AssemblySource"
         },
         "CRISPRSource": {
             "@id": "CRISPRSource"
         },
         "CloningStrategy": {
@@ -147,27 +150,27 @@
             "@id": "index_in_file",
             "@type": "xsd:integer"
         },
         "input": {
             "@id": "input",
             "@type": "@id"
         },
-        "left_edge": {
-            "@id": "left_edge",
+        "left": {
+            "@id": "left",
             "@type": "@id"
         },
-        "left_fragment": {
-            "@id": "left_fragment",
+        "left_edge": {
+            "@id": "left_edge",
             "@type": "@id"
         },
-        "left_location": {
-            "@id": "left_location",
+        "linkml": "https://w3id.org/linkml/",
+        "location": {
+            "@id": "location",
             "@type": "@id"
         },
-        "linkml": "https://w3id.org/linkml/",
         "locus_tag": {
             "@id": "locus_tag"
         },
         "name": {
             "@id": "schema:name"
         },
         "output": {
@@ -204,32 +207,32 @@
         },
         "restriction_enzyme": {
             "@id": "restriction_enzyme"
         },
         "restriction_enzymes": {
             "@id": "restriction_enzymes"
         },
+        "reverse_complemented": {
+            "@id": "reverse_complemented",
+            "@type": "xsd:boolean"
+        },
         "reverse_oligo": {
             "@id": "reverse_oligo",
             "@type": "@id"
         },
         "reverse_primer": {
             "@id": "reverse_primer",
             "@type": "@id"
         },
-        "right_edge": {
-            "@id": "right_edge",
+        "right": {
+            "@id": "right",
             "@type": "@id"
         },
-        "right_fragment": {
-            "@id": "right_fragment",
-            "@type": "@id"
-        },
-        "right_location": {
-            "@id": "right_location",
+        "right_edge": {
+            "@id": "right_edge",
             "@type": "@id"
         },
         "schema": "http://schema.org/",
         "sequence": {
             "@id": "sequence"
         },
         "sequence_accession": {
@@ -270,11 +273,11 @@
         },
         "user_input": {
             "@id": "user_input"
         }
     },
     "comments": {
         "description": "Auto generated by LinkML jsonld context generator",
-        "generation_date": "2024-05-08T10:06:27",
+        "generation_date": "2024-05-08T12:30:30",
         "source": "shareyourcloning_linkml.yaml"
     }
 }
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.jsonld` & `shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.jsonld`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.926819923085125%*

 * *Differences: {"'classes'": "{16: {'slots': ['assemblyJoin__left', 'assemblyJoin__right'], 'attributes': {0: "*

 * *              "{'name': 'left', 'range': 'AssemblyJoinComponent'}, 1: {'name': 'right', 'range': "*

 * *              "'AssemblyJoinComponent'}, delete: [3, 2]}}, insert: [(15, OrderedDict([('name', "*

 * *              "'AssemblyJoinComponent'), ('definition_uri', "*

 * *              "'https://w3id.org/genestorian/ShareYourCloning_LinkML/AssemblyJoinComponent'), "*

 * *              "('description', 'Represents a component of a j […]*

```diff
@@ -447,52 +447,71 @@
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
-                    "name": "left_fragment",
+                    "name": "sequence",
                     "range": "Sequence",
                     "required": true
                 },
                 {
                     "@type": "SlotDefinition",
-                    "name": "right_fragment",
-                    "range": "Sequence",
+                    "description": "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join.",
+                    "inlined": true,
+                    "name": "location",
+                    "range": "SimpleSequenceLocation",
                     "required": true
                 },
                 {
                     "@type": "SlotDefinition",
-                    "description": "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join.",
-                    "inlined": true,
-                    "name": "left_location",
-                    "range": "SimpleSequenceLocation",
+                    "description": "Whether the sequence is reverse complemented in the join",
+                    "name": "reverse_complemented",
+                    "range": "boolean",
+                    "required": true
+                }
+            ],
+            "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AssemblyJoinComponent",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AssemblyJoinComponent",
+            "description": "Represents a component of a join between two fragments in an assembly",
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "name": "AssemblyJoinComponent",
+            "slot_usage": {},
+            "slots": [
+                "assemblyJoinComponent__sequence",
+                "assemblyJoinComponent__location",
+                "assemblyJoinComponent__reverse_complemented"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "attributes": [
+                {
+                    "@type": "SlotDefinition",
+                    "name": "left",
+                    "range": "AssemblyJoinComponent",
                     "required": true
                 },
                 {
                     "@type": "SlotDefinition",
-                    "description": "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join.",
-                    "inlined": true,
-                    "name": "right_location",
-                    "range": "SimpleSequenceLocation",
+                    "name": "right",
+                    "range": "AssemblyJoinComponent",
                     "required": true
                 }
             ],
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AssemblyJoin",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AssemblyJoin",
             "description": "Represents a joint between two fragments in an assembly",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "AssemblyJoin",
             "slot_usage": {},
             "slots": [
-                "assemblyJoin__left_fragment",
-                "assemblyJoin__right_fragment",
-                "assemblyJoin__left_location",
-                "assemblyJoin__right_location"
+                "assemblyJoin__left",
+                "assemblyJoin__right"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
@@ -811,15 +830,15 @@
                 {
                     "description": "Full sequence of the plasmid performed by Addgene",
                     "text": "addgene-full"
                 }
             ]
         }
     ],
-    "generation_date": "2024-05-08T10:06:27",
+    "generation_date": "2024-05-08T12:30:30",
     "id": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
     "imports": [
         "linkml:types"
     ],
     "license": "MIT",
     "metamodel_version": "1.7.0",
     "name": "ShareYourCloning_LinkML",
@@ -1354,67 +1373,81 @@
             "name": "simpleSequenceLocation__strand",
             "owner": "SimpleSequenceLocation",
             "range": "integer",
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/strand"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "left_fragment",
+            "alias": "sequence",
             "domain_of": [
-                "AssemblyJoin"
+                "AssemblyJoinComponent"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "assemblyJoin__left_fragment",
-            "owner": "AssemblyJoin",
+            "name": "assemblyJoinComponent__sequence",
+            "owner": "AssemblyJoinComponent",
             "range": "Sequence",
             "required": true,
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/left_fragment"
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "right_fragment",
+            "alias": "location",
+            "description": "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join.",
             "domain_of": [
-                "AssemblyJoin"
+                "AssemblyJoinComponent"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "assemblyJoin__right_fragment",
-            "owner": "AssemblyJoin",
-            "range": "Sequence",
+            "inlined": true,
+            "name": "assemblyJoinComponent__location",
+            "owner": "AssemblyJoinComponent",
+            "range": "SimpleSequenceLocation",
             "required": true,
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/right_fragment"
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/location"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "left_location",
-            "description": "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join.",
+            "alias": "reverse_complemented",
+            "description": "Whether the sequence is reverse complemented in the join",
+            "domain_of": [
+                "AssemblyJoinComponent"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "name": "assemblyJoinComponent__reverse_complemented",
+            "owner": "AssemblyJoinComponent",
+            "range": "boolean",
+            "required": true,
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/reverse_complemented"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "left",
             "domain_of": [
                 "AssemblyJoin"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "inlined": true,
-            "name": "assemblyJoin__left_location",
+            "name": "assemblyJoin__left",
             "owner": "AssemblyJoin",
-            "range": "SimpleSequenceLocation",
+            "range": "AssemblyJoinComponent",
             "required": true,
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/left_location"
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/left"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "right_location",
-            "description": "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join.",
+            "alias": "right",
             "domain_of": [
                 "AssemblyJoin"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "inlined": true,
-            "name": "assemblyJoin__right_location",
+            "name": "assemblyJoin__right",
             "owner": "AssemblyJoin",
-            "range": "SimpleSequenceLocation",
+            "range": "AssemblyJoinComponent",
             "required": true,
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/right_location"
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/right"
         },
         {
             "@type": "SlotDefinition",
             "alias": "circular",
             "description": "Whether the assembly is circular or not",
             "domain_of": [
                 "AssemblySource"
@@ -1932,16 +1965,16 @@
             "owner": "PolymeraseExtensionSource",
             "range": "Sequence",
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
             "usage_slot_name": "input"
         }
     ],
     "source_file": "shareyourcloning_linkml.yaml",
-    "source_file_date": "2024-05-08T09:28:36",
-    "source_file_size": 15500,
+    "source_file_date": "2024-05-08T12:30:24",
+    "source_file_size": 15604,
     "title": "ShareYourCloning_LinkML",
     "types": [
         {
             "@type": "TypeDefinition",
             "base": "str",
             "definition_uri": "https://w3id.org/linkml/String",
             "description": "A character string",
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/jsonschema/shareyourcloning_linkml.schema.json` & `shareyourcloning_linkml-0.1.4a0/project/jsonschema/shareyourcloning_linkml.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975818452380952%*

 * *Differences: {"'$defs'": "{'AssemblyJoin': {'properties': {replace: OrderedDict([('left', OrderedDict([('$ref', "*

 * *            "'#/$defs/AssemblyJoinComponent')])), ('right', OrderedDict([('$ref', "*

 * *            "'#/$defs/AssemblyJoinComponent')]))])}, 'required': ['left', 'right']}, "*

 * *            "'AssemblyJoinComponent': OrderedDict([('additionalProperties', False), "*

 * *            "('description', 'Represents a component of a join between two fragments in an "*

 * *            "assembly'), ('properties', OrderedDict([('locati […]*

```diff
@@ -59,36 +59,50 @@
             "title": "AddGeneSequenceType",
             "type": "string"
         },
         "AssemblyJoin": {
             "additionalProperties": false,
             "description": "Represents a joint between two fragments in an assembly",
             "properties": {
-                "left_fragment": {
-                    "type": "integer"
+                "left": {
+                    "$ref": "#/$defs/AssemblyJoinComponent"
                 },
-                "left_location": {
+                "right": {
+                    "$ref": "#/$defs/AssemblyJoinComponent"
+                }
+            },
+            "required": [
+                "left",
+                "right"
+            ],
+            "title": "AssemblyJoin",
+            "type": "object"
+        },
+        "AssemblyJoinComponent": {
+            "additionalProperties": false,
+            "description": "Represents a component of a join between two fragments in an assembly",
+            "properties": {
+                "location": {
                     "$ref": "#/$defs/SimpleSequenceLocation",
-                    "description": "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join."
+                    "description": "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join."
                 },
-                "right_fragment": {
-                    "type": "integer"
+                "reverse_complemented": {
+                    "description": "Whether the sequence is reverse complemented in the join",
+                    "type": "boolean"
                 },
-                "right_location": {
-                    "$ref": "#/$defs/SimpleSequenceLocation",
-                    "description": "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join."
+                "sequence": {
+                    "type": "integer"
                 }
             },
             "required": [
-                "left_fragment",
-                "right_fragment",
-                "left_location",
-                "right_location"
+                "sequence",
+                "location",
+                "reverse_complemented"
             ],
-            "title": "AssemblyJoin",
+            "title": "AssemblyJoinComponent",
             "type": "object"
         },
         "AssemblySource": {
             "additionalProperties": false,
             "description": "Represents the source of a sequence that is an assembly of other sequences",
             "properties": {
                 "assembly": {
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/owl/shareyourcloning_linkml.owl.ttl` & `shareyourcloning_linkml-0.1.4a0/project/owl/shareyourcloning_linkml.owl.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -9,102 +9,117 @@
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 shareyourcloning_linkml:CloningStrategy a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "CloningStrategy" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sources ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:primers ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:primers ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequences ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Source ;
-            owl:onProperty shareyourcloning_linkml:sources ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:primers ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:sequences ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequences ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:Source ;
             owl:onProperty shareyourcloning_linkml:sources ] ;
     skos:definition "Represents a cloning strategy" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:AssemblyJoin a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblyJoin" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:AssemblyJoinComponent ;
+            owl:onProperty shareyourcloning_linkml:right ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_location ],
+            owl:onProperty shareyourcloning_linkml:right ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_location ],
+            owl:onProperty shareyourcloning_linkml:left ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:right_fragment ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:right ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
-            owl:onProperty shareyourcloning_linkml:right_location ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:left ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
-            owl:onProperty shareyourcloning_linkml:left_location ],
+            owl:allValuesFrom shareyourcloning_linkml:AssemblyJoinComponent ;
+            owl:onProperty shareyourcloning_linkml:left ] ;
+    skos:definition "Represents a joint between two fragments in an assembly" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
+shareyourcloning_linkml:SimpleSequenceLocation a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "SimpleSequenceLocation" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left_fragment ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left_location ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left_fragment ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:end ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left_location ],
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_fragment ],
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_fragment ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:left_fragment ] ;
-    skos:definition "Represents a joint between two fragments in an assembly" ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ] ;
+    skos:definition "Represents a location within a sequence, for now support for ranges only" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:AddGeneIdSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AddGeneIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
+            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:AddGeneSequenceType ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:AddGeneSequenceType ;
             owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:sequence_file_url ],
@@ -118,14 +133,47 @@
     rdfs:subClassOf shareyourcloning_linkml:AddGeneSequenceType .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#depositor-full> a owl:Class,
         shareyourcloning_linkml:AddGeneSequenceType ;
     rdfs:label "depositor-full" ;
     rdfs:subClassOf shareyourcloning_linkml:AddGeneSequenceType .
 
+shareyourcloning_linkml:AssemblyJoinComponent a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "AssemblyJoinComponent" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:location ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:location ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
+            owl:onProperty shareyourcloning_linkml:location ] ;
+    skos:definition "Represents a component of a join between two fragments in an assembly" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:CRISPRSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "CRISPRSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:guides ],
         [ a owl:Restriction ;
@@ -135,76 +183,76 @@
     skos:definition "Represents the source of a sequence that is generated by CRISPR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:GenomeCoordinatesSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "GenomeCoordinatesSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:gene_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:end ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:locus_tag ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:gene_id ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_accession ],
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:strand ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:strand ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:GibsonAssemblySource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "GibsonAssemblySource" ;
@@ -232,131 +280,131 @@
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:ManuallyTypedSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "ManuallyTypedSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:user_input ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
-            owl:allValuesFrom [ a rdfs:Datatype ;
-                    owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
-                                owl:onDatatype xsd:string ;
-                                owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
-            owl:onProperty shareyourcloning_linkml:user_input ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:user_input ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:user_input ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
+            owl:allValuesFrom [ a rdfs:Datatype ;
+                    owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
+                                owl:onDatatype xsd:string ;
+                                owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
+            owl:onProperty shareyourcloning_linkml:user_input ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Boolean ;
             owl:onProperty shareyourcloning_linkml:circular ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is manually typed by the user" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:NamedThing a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "NamedThing" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:id ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:id ] ;
     skos:exactMatch schema1:Thing ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:OligoHybridizationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "OligoHybridizationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_oligo ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is generated by oligo hybridization" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:PCRSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "PCRSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:forward_primer ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:input ],
-        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_primer ],
         [ a owl:Restriction ;
             owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_primer ],
+            owl:onProperty shareyourcloning_linkml:reverse_primer ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_primer ],
+            owl:onProperty shareyourcloning_linkml:forward_primer ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by PCR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:PolymeraseExtensionSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "PolymeraseExtensionSource" ;
@@ -380,50 +428,50 @@
     rdfs:label "genbank" ;
     rdfs:subClassOf shareyourcloning_linkml:RepositoryName .
 
 shareyourcloning_linkml:RestrictionAndLigationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionAndLigationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by restriction and ligation" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionEnzymeDigestionSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:right_edge ],
         shareyourcloning_linkml:SequenceCutSource ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionSequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionSequenceCut" ;
@@ -451,120 +499,87 @@
     rdfs:subClassOf shareyourcloning_linkml:SequenceFileFormat .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> a owl:Class,
         shareyourcloning_linkml:SequenceFileFormat ;
     rdfs:label "snapgene" ;
     rdfs:subClassOf shareyourcloning_linkml:SequenceFileFormat .
 
-shareyourcloning_linkml:SimpleSequenceLocation a owl:Class,
-        linkml:ClassDefinition ;
-    rdfs:label "SimpleSequenceLocation" ;
-    rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:strand ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:end ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ] ;
-    skos:definition "Represents a location within a sequence, for now support for ranges only" ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
 shareyourcloning_linkml:TextFileSequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TextFileSequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:file_content ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "A sequence (may have features) defined by the content of a text file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:UploadedFileSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "UploadedFileSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:index_in_file ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:file_name ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:index_in_file ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:index_in_file ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is uploaded as a file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:assembly a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "assembly" ;
@@ -615,86 +630,86 @@
     skos:definition "Represents the source of a sequence that is generated by homologous recombination" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RepositoryIdSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RepositoryIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:repository_name ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:repository_name ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:RepositoryName ;
+            owl:onProperty shareyourcloning_linkml:repository_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:repository_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:RepositoryName ;
-            owl:onProperty shareyourcloning_linkml:repository_name ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is identified by a repository id" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCut" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang ],
+            owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:cut_watson ] ;
+            owl:onProperty shareyourcloning_linkml:overhang ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang ] ;
     skos:definition "Represents a cut in a DNA sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceCutSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCutSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
+            owl:onProperty shareyourcloning_linkml:left_edge ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
-            owl:onProperty shareyourcloning_linkml:input ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:left_edge ],
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:addgene_sequence_type a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "addgene_sequence_type" ;
@@ -749,23 +764,23 @@
 
 shareyourcloning_linkml:index_in_file a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "index_in_file" ;
     skos:definition "The index of the sequence in the file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:left_fragment a owl:ObjectProperty,
+shareyourcloning_linkml:left a owl:ObjectProperty,
         linkml:SlotDefinition ;
-    rdfs:label "left_fragment" ;
+    rdfs:label "left" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:left_location a owl:ObjectProperty,
+shareyourcloning_linkml:location a owl:ObjectProperty,
         linkml:SlotDefinition ;
-    rdfs:label "left_location" ;
-    skos:definition "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join." ;
+    rdfs:label "location" ;
+    skos:definition "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:locus_tag a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "locus_tag" ;
     skos:definition "The locus tag of the sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
@@ -804,40 +819,35 @@
 shareyourcloning_linkml:restriction_enzyme a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "restriction_enzyme" ;
     rdfs:range linkml:String ;
     skos:exactMatch OBI:0000732 ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:reverse_complemented a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "reverse_complemented" ;
+    skos:definition "Whether the sequence is reverse complemented in the join" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:reverse_oligo a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "reverse_oligo" ;
     skos:definition "The reverse oligo used in the hybridization" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:reverse_primer a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "reverse_primer" ;
     skos:definition "The reverse primer used in the PCR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:right_fragment a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "right_fragment" ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
-shareyourcloning_linkml:right_location a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "right_location" ;
-    skos:definition "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join." ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
-shareyourcloning_linkml:sequence a owl:ObjectProperty,
+shareyourcloning_linkml:right a owl:ObjectProperty,
         linkml:SlotDefinition ;
-    rdfs:label "sequence" ;
+    rdfs:label "right" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:sequence_accession a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "sequence_accession" ;
     skos:definition "The accession of the sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
@@ -891,14 +901,17 @@
     rdfs:range linkml:Integer ;
     skos:definition "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:right_edge a owl:ObjectProperty,
         linkml:SlotDefinition .
 
+shareyourcloning_linkml:sequence a owl:ObjectProperty,
+        linkml:SlotDefinition .
+
 shareyourcloning_linkml:sequence_file_format a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "sequence_file_format" ;
     rdfs:range shareyourcloning_linkml:SequenceFileFormat ;
     skos:definition "The format of a sequence file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
@@ -914,50 +927,50 @@
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:Boolean ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:assembly ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:AssemblyJoin ;
             owl:onProperty shareyourcloning_linkml:assembly ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:circular ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is an assembly of other sequences" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Primer a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Primer" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:name ],
+        [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:name ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "An oligonucleotide or primer" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceFileFormat a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#genbank> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> ) ;
@@ -972,59 +985,59 @@
     skos:definition "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Sequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Sequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:id ],
-        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:type ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:type ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Source a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Source" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:output ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:input ],
+            owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:type ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents the source of a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
@@ -1051,101 +1064,100 @@
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:PCRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:PCRSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
+    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Sequence .
+    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:AddGeneIdSource ;
+    rdfs:subClassOf shareyourcloning_linkml:RestrictionEnzymeDigestionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:AddGeneIdSource .
+    owl:someValuesFrom shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Primer ;
+    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Primer .
+    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:GenomeCoordinatesSource ;
+    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:GenomeCoordinatesSource .
+    owl:someValuesFrom shareyourcloning_linkml:Sequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
+    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
+    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Source ;
+    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Source .
+    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
+    rdfs:subClassOf shareyourcloning_linkml:Source ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
+    owl:someValuesFrom shareyourcloning_linkml:Source .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:OligoHybridizationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:OligoHybridizationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RestrictionEnzymeDigestionSource ;
+    rdfs:subClassOf shareyourcloning_linkml:TextFileSequence ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
+    owl:someValuesFrom shareyourcloning_linkml:TextFileSequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
+    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
+    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:UploadedFileSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:UploadedFileSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:CRISPRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:CRISPRSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:TextFileSequence ;
+    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:TextFileSequence .
+    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:Primer ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
+    owl:someValuesFrom shareyourcloning_linkml:Primer .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:CRISPRSource ;
+    rdfs:subClassOf shareyourcloning_linkml:RepositoryIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:CRISPRSource .
+    owl:someValuesFrom shareyourcloning_linkml:RepositoryIdSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:GenomeCoordinatesSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:GenomeCoordinatesSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RepositoryIdSource ;
+    rdfs:subClassOf shareyourcloning_linkml:AddGeneIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RepositoryIdSource .
-
+    owl:someValuesFrom shareyourcloning_linkml:AddGeneIdSource .
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/protobuf/shareyourcloning_linkml.proto` & `shareyourcloning_linkml-0.1.4a0/project/protobuf/shareyourcloning_linkml.proto`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,23 @@
   string repositoryId = 0
   string sequenceFileUrl = 0
   addGeneSequenceType addgeneSequenceType = 0
  }
 // Represents a joint between two fragments in an assembly
 message AssemblyJoin
  {
-  sequence leftFragment = 0
-  sequence rightFragment = 0
-  simpleSequenceLocation leftLocation = 0
-  simpleSequenceLocation rightLocation = 0
+  assemblyJoinComponent left = 0
+  assemblyJoinComponent right = 0
+ }
+// Represents a component of a join between two fragments in an assembly
+message AssemblyJoinComponent
+ {
+  sequence sequence = 0
+  simpleSequenceLocation location = 0
+  boolean reverseComplemented = 0
  }
 // Represents the source of a sequence that is an assembly of other sequences
 message AssemblySource
  {
   integer id = 0
  repeated  sequence input = 0
   sequence output = 0
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/python/shareyourcloning_linkml.py` & `shareyourcloning_linkml-0.1.4a0/project/python/shareyourcloning_linkml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from shareyourcloning_linkml.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-05-08T10:06:28
+# Generation date: 2024-05-08T12:30:31
 # Schema: ShareYourCloning_LinkML
 #
 # id: https://w3id.org/genestorian/ShareYourCloning_LinkML
 # description: A LinkML data model for ShareYourCloning
 # license: MIT
 
 import dataclasses
@@ -692,51 +692,75 @@
         if self.strand is not None and not isinstance(self.strand, int):
             self.strand = int(self.strand)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
+class AssemblyJoinComponent(YAMLRoot):
+    """
+    Represents a component of a join between two fragments in an assembly
+    """
+
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["AssemblyJoinComponent"]
+    class_class_curie: ClassVar[str] = "shareyourcloning_linkml:AssemblyJoinComponent"
+    class_name: ClassVar[str] = "AssemblyJoinComponent"
+    class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.AssemblyJoinComponent
+
+    sequence: Union[int, SequenceId] = None
+    location: Union[dict, SimpleSequenceLocation] = None
+    reverse_complemented: Union[bool, Bool] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.sequence):
+            self.MissingRequiredField("sequence")
+        if not isinstance(self.sequence, SequenceId):
+            self.sequence = SequenceId(self.sequence)
+
+        if self._is_empty(self.location):
+            self.MissingRequiredField("location")
+        if not isinstance(self.location, SimpleSequenceLocation):
+            self.location = SimpleSequenceLocation(**as_dict(self.location))
+
+        if self._is_empty(self.reverse_complemented):
+            self.MissingRequiredField("reverse_complemented")
+        if not isinstance(self.reverse_complemented, Bool):
+            self.reverse_complemented = Bool(self.reverse_complemented)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
 class AssemblyJoin(YAMLRoot):
     """
     Represents a joint between two fragments in an assembly
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["AssemblyJoin"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:AssemblyJoin"
     class_name: ClassVar[str] = "AssemblyJoin"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.AssemblyJoin
 
-    left_fragment: Union[int, SequenceId] = None
-    right_fragment: Union[int, SequenceId] = None
-    left_location: Union[dict, SimpleSequenceLocation] = None
-    right_location: Union[dict, SimpleSequenceLocation] = None
-
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self._is_empty(self.left_fragment):
-            self.MissingRequiredField("left_fragment")
-        if not isinstance(self.left_fragment, SequenceId):
-            self.left_fragment = SequenceId(self.left_fragment)
-
-        if self._is_empty(self.right_fragment):
-            self.MissingRequiredField("right_fragment")
-        if not isinstance(self.right_fragment, SequenceId):
-            self.right_fragment = SequenceId(self.right_fragment)
-
-        if self._is_empty(self.left_location):
-            self.MissingRequiredField("left_location")
-        if not isinstance(self.left_location, SimpleSequenceLocation):
-            self.left_location = SimpleSequenceLocation(**as_dict(self.left_location))
-
-        if self._is_empty(self.right_location):
-            self.MissingRequiredField("right_location")
-        if not isinstance(self.right_location, SimpleSequenceLocation):
-            self.right_location = SimpleSequenceLocation(**as_dict(self.right_location))
+    left: Union[dict, AssemblyJoinComponent] = None
+    right: Union[dict, AssemblyJoinComponent] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.left):
+            self.MissingRequiredField("left")
+        if not isinstance(self.left, AssemblyJoinComponent):
+            self.left = AssemblyJoinComponent(**as_dict(self.left))
+
+        if self._is_empty(self.right):
+            self.MissingRequiredField("right")
+        if not isinstance(self.right, AssemblyJoinComponent):
+            self.right = AssemblyJoinComponent(**as_dict(self.right))
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class AssemblySource(Source):
     """
@@ -1462,48 +1486,57 @@
     name="simpleSequenceLocation__strand",
     curie=SHAREYOURCLONING_LINKML.curie("strand"),
     model_uri=SHAREYOURCLONING_LINKML.simpleSequenceLocation__strand,
     domain=None,
     range=Optional[int],
 )
 
-slots.assemblyJoin__left_fragment = Slot(
-    uri=SHAREYOURCLONING_LINKML.left_fragment,
-    name="assemblyJoin__left_fragment",
-    curie=SHAREYOURCLONING_LINKML.curie("left_fragment"),
-    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__left_fragment,
+slots.assemblyJoinComponent__sequence = Slot(
+    uri=SHAREYOURCLONING_LINKML.sequence,
+    name="assemblyJoinComponent__sequence",
+    curie=SHAREYOURCLONING_LINKML.curie("sequence"),
+    model_uri=SHAREYOURCLONING_LINKML.assemblyJoinComponent__sequence,
     domain=None,
     range=Union[int, SequenceId],
 )
 
-slots.assemblyJoin__right_fragment = Slot(
-    uri=SHAREYOURCLONING_LINKML.right_fragment,
-    name="assemblyJoin__right_fragment",
-    curie=SHAREYOURCLONING_LINKML.curie("right_fragment"),
-    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__right_fragment,
+slots.assemblyJoinComponent__location = Slot(
+    uri=SHAREYOURCLONING_LINKML.location,
+    name="assemblyJoinComponent__location",
+    curie=SHAREYOURCLONING_LINKML.curie("location"),
+    model_uri=SHAREYOURCLONING_LINKML.assemblyJoinComponent__location,
     domain=None,
-    range=Union[int, SequenceId],
+    range=Union[dict, SimpleSequenceLocation],
 )
 
-slots.assemblyJoin__left_location = Slot(
-    uri=SHAREYOURCLONING_LINKML.left_location,
-    name="assemblyJoin__left_location",
-    curie=SHAREYOURCLONING_LINKML.curie("left_location"),
-    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__left_location,
+slots.assemblyJoinComponent__reverse_complemented = Slot(
+    uri=SHAREYOURCLONING_LINKML.reverse_complemented,
+    name="assemblyJoinComponent__reverse_complemented",
+    curie=SHAREYOURCLONING_LINKML.curie("reverse_complemented"),
+    model_uri=SHAREYOURCLONING_LINKML.assemblyJoinComponent__reverse_complemented,
     domain=None,
-    range=Union[dict, SimpleSequenceLocation],
+    range=Union[bool, Bool],
 )
 
-slots.assemblyJoin__right_location = Slot(
-    uri=SHAREYOURCLONING_LINKML.right_location,
-    name="assemblyJoin__right_location",
-    curie=SHAREYOURCLONING_LINKML.curie("right_location"),
-    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__right_location,
+slots.assemblyJoin__left = Slot(
+    uri=SHAREYOURCLONING_LINKML.left,
+    name="assemblyJoin__left",
+    curie=SHAREYOURCLONING_LINKML.curie("left"),
+    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__left,
     domain=None,
-    range=Union[dict, SimpleSequenceLocation],
+    range=Union[dict, AssemblyJoinComponent],
+)
+
+slots.assemblyJoin__right = Slot(
+    uri=SHAREYOURCLONING_LINKML.right,
+    name="assemblyJoin__right",
+    curie=SHAREYOURCLONING_LINKML.curie("right"),
+    model_uri=SHAREYOURCLONING_LINKML.assemblyJoin__right,
+    domain=None,
+    range=Union[dict, AssemblyJoinComponent],
 )
 
 slots.assemblySource__circular = Slot(
     uri=SHAREYOURCLONING_LINKML.circular,
     name="assemblySource__circular",
     curie=SHAREYOURCLONING_LINKML.curie("circular"),
     model_uri=SHAREYOURCLONING_LINKML.assemblySource__circular,
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/shacl/shareyourcloning_linkml.shacl.ttl` & `shareyourcloning_linkml-0.1.4a0/project/shacl/shareyourcloning_linkml.shacl.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -19,91 +19,91 @@
     sh:description "Represents the source of a sequence that is identified by an AddGene id" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:in ( "depositor-full" "addgene-full" ) ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:addgene_sequence_type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:in ( "addgene" "genbank" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "The URL of a sequence file" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:repository_name ],
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence_file_url ;
+            sh:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ],
         [ sh:datatype xsd:string ;
             sh:description "The id of the sequence in the repository" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:repository_id ],
         [ sh:datatype xsd:string ;
-            sh:description "The URL of a sequence file" ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequence_file_url ;
-            sh:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ],
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 7 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:in ( "depositor-full" "addgene-full" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:addgene_sequence_type ],
+        [ sh:in ( "addgene" "genbank" ) ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:repository_name ] ;
     sh:targetClass shareyourcloning_linkml:AddGeneIdSource .
 
 shareyourcloning_linkml:AssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is an assembly of other sequences" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
-        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
-            sh:description "The joins between the fragments in the assembly" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+            sh:description "The joins between the fragments in the assembly" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:assembly ] ;
     sh:targetClass shareyourcloning_linkml:AssemblySource .
 
 shareyourcloning_linkml:CRISPRSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by CRISPR" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
@@ -113,77 +113,83 @@
             sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The guide RNAs used in the CRISPR" ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:guides ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:assembly ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:circular ] ;
     sh:targetClass shareyourcloning_linkml:CRISPRSource .
 
 shareyourcloning_linkml:CloningStrategy a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cloning strategy" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are used in the cloning strategy" ;
-            sh:minCount 1 ;
+    sh:property [ sh:class shareyourcloning_linkml:Primer ;
+            sh:description "The primers that are used in the cloning strategy" ;
             sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequences ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:primers ],
         [ sh:class shareyourcloning_linkml:Source ;
             sh:description "The sources of the sequences that are used in the cloning strategy" ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:sources ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are used in the cloning strategy" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequences ],
         [ sh:datatype xsd:string ;
             sh:description "A description of the cloning strategy" ;
             sh:maxCount 1 ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:description ],
-        [ sh:class shareyourcloning_linkml:Primer ;
-            sh:description "The primers that are used in the cloning strategy" ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:primers ] ;
+            sh:path shareyourcloning_linkml:description ] ;
     sh:targetClass shareyourcloning_linkml:CloningStrategy .
 
 shareyourcloning_linkml:GenomeCoordinatesSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 8 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
             sh:description "The locus tag of the sequence" ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:locus_tag ],
         [ sh:datatype xsd:integer ;
             sh:description "The starting coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
@@ -192,624 +198,666 @@
             sh:path shareyourcloning_linkml:start ],
         [ sh:datatype xsd:integer ;
             sh:description "The ending coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:end ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 8 ;
-            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
             sh:description "The gene id of the sequence" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:gene_id ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 7 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The accession of the assembly" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:assembly_accession ],
         [ sh:datatype xsd:string ;
             sh:description "The accession of the sequence" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:sequence_accession ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 9 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 7 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The accession of the assembly" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 10 ;
-            sh:path schema1:identifier ],
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:assembly_accession ],
         [ sh:datatype xsd:integer ;
             sh:description "The strand of the sequence in the sequence accession, should be 1 or -1" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
-            sh:path shareyourcloning_linkml:strand ] ;
+            sh:path shareyourcloning_linkml:strand ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 10 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:GenomeCoordinatesSource .
 
 shareyourcloning_linkml:GibsonAssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by Gibson assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:assembly ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:GibsonAssemblySource .
 
 shareyourcloning_linkml:HomologousRecombinationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by homologous recombination" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
+    sh:property [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:assembly ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ] ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:HomologousRecombinationSource .
 
 shareyourcloning_linkml:LigationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ] ;
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ] ;
     sh:targetClass shareyourcloning_linkml:LigationSource .
 
 shareyourcloning_linkml:ManuallyTypedSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is manually typed by the user" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+    sh:property [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:user_input ;
+            sh:pattern "^[acgtACGT]+$" ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the sequence is circular or not" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:circular ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 7 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:user_input ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:defaultValue 0 ;
             sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:overhang_crick_3prime ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:integer ;
             sh:defaultValue 0 ;
             sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:overhang_watson_3prime ] ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:ManuallyTypedSource .
 
 shareyourcloning_linkml:OligoHybridizationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by oligo hybridization" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ],
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:overhang_crick_3prime ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The reverse oligo used in the hybridization" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:reverse_oligo ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The forward oligo used in the hybridization" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:forward_oligo ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
-            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:overhang_crick_3prime ] ;
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:OligoHybridizationSource .
 
 shareyourcloning_linkml:PCRSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by PCR" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 7 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:circular ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:assembly ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The forward primer used in the PCR" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:forward_primer ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The reverse primer used in the PCR" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:reverse_primer ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:minCount 1 ;
+            sh:order 7 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:PCRSource .
 
 shareyourcloning_linkml:PolymeraseExtensionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by polymerase extension" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:output ] ;
     sh:targetClass shareyourcloning_linkml:PolymeraseExtensionSource .
 
 shareyourcloning_linkml:RepositoryIdSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by a repository id" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
             sh:description "The id of the sequence in the repository" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:repository_id ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
         [ sh:in ( "addgene" "genbank" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:repository_name ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:RepositoryIdSource .
 
 shareyourcloning_linkml:RestrictionAndLigationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by restriction and ligation" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
+    sh:property [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ],
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:restriction_enzymes ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:assembly ],
         [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionAndLigationSource .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:left_edge ],
+        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:right_edge ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_edge ],
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 shareyourcloning_linkml:SequenceCutSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:SequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:left_edge ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:SequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:right_edge ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ] ;
     sh:targetClass shareyourcloning_linkml:SequenceCutSource .
 
 shareyourcloning_linkml:TextFileSequence a sh:NodeShape ;
     sh:closed true ;
     sh:description "A sequence (may have features) defined by the content of a text file" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:integer ;
             sh:defaultValue 0 ;
-            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:overhang_crick_3prime ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
         [ sh:description "The format of a sequence file" ;
             sh:in ( "fasta" "genbank" "snapgene" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:sequence_file_format ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
-            sh:defaultValue 0 ;
-            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:file_content ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
+            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:overhang_crick_3prime ] ;
     sh:targetClass shareyourcloning_linkml:TextFileSequence .
 
 shareyourcloning_linkml:UploadedFileSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is uploaded as a file" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The name of the file" ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:file_name ],
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:description "The format of a sequence file" ;
             sh:in ( "fasta" "genbank" "snapgene" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:sequence_file_format ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The index of the sequence in the file" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:index_in_file ],
         [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+            sh:description "The name of the file" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:file_name ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
             sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ] ;
+    sh:targetClass shareyourcloning_linkml:UploadedFileSource .
+
+shareyourcloning_linkml:SimpleSequenceLocation a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents a location within a sequence, for now support for ranges only" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:datatype xsd:integer ;
+            sh:description "The starting coordinate (1-based) of the location" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:start ],
         [ sh:datatype xsd:integer ;
-            sh:description "The index of the sequence in the file" ;
+            sh:description "The ending coordinate (1-based) of the location" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:index_in_file ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:minCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:end ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The strand of the location, should be 1 or -1 or null" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ] ;
-    sh:targetClass shareyourcloning_linkml:UploadedFileSource .
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:strand ] ;
+    sh:targetClass shareyourcloning_linkml:SimpleSequenceLocation .
 
 shareyourcloning_linkml:Source a sh:NodeShape ;
     sh:closed false ;
     sh:description "Represents the source of a sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:identifier ],
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:identifier ] ;
+    sh:targetClass shareyourcloning_linkml:Source .
+
+shareyourcloning_linkml:AssemblyJoinComponent a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents a component of a join between two fragments in an assembly" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence ],
+        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
+            sh:description "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+            sh:path shareyourcloning_linkml:location ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the sequence is reverse complemented in the join" ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 2 ;
-            sh:path shareyourcloning_linkml:type ] ;
-    sh:targetClass shareyourcloning_linkml:Source .
+            sh:path shareyourcloning_linkml:reverse_complemented ] ;
+    sh:targetClass shareyourcloning_linkml:AssemblyJoinComponent .
 
 shareyourcloning_linkml:RestrictionSequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence that is made by a restriction enzyme" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
             sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
@@ -831,107 +879,70 @@
     sh:targetClass shareyourcloning_linkml:RestrictionSequenceCut .
 
 shareyourcloning_linkml:SequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
-            sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:cut_watson ],
-        [ sh:datatype xsd:integer ;
             sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:overhang ] ;
-    sh:targetClass shareyourcloning_linkml:SequenceCut .
-
-shareyourcloning_linkml:SimpleSequenceLocation a sh:NodeShape ;
-    sh:closed true ;
-    sh:description "Represents a location within a sequence, for now support for ranges only" ;
-    sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "The ending coordinate (1-based) of the location" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:end ],
+            sh:path shareyourcloning_linkml:overhang ],
         [ sh:datatype xsd:integer ;
-            sh:description "The starting coordinate (1-based) of the location" ;
+            sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
-            sh:path shareyourcloning_linkml:start ],
-        [ sh:datatype xsd:integer ;
-            sh:description "The strand of the location, should be 1 or -1 or null" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:strand ] ;
-    sh:targetClass shareyourcloning_linkml:SimpleSequenceLocation .
+            sh:path shareyourcloning_linkml:cut_watson ] ;
+    sh:targetClass shareyourcloning_linkml:SequenceCut .
 
 shareyourcloning_linkml:Primer a sh:NodeShape ;
     sh:closed true ;
     sh:description "An oligonucleotide or primer" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a thing" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sequence ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sequence ;
+            sh:pattern "^[acgtACGT]+$" ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a thing" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path schema1:name ] ;
     sh:targetClass shareyourcloning_linkml:Primer .
 
 shareyourcloning_linkml:AssemblyJoin a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a joint between two fragments in an assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoinComponent ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_fragment ],
-        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
-            sh:description "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join." ;
+            sh:path shareyourcloning_linkml:left ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoinComponent ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:right_location ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:right_fragment ],
-        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
-            sh:description "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:left_location ] ;
+            sh:path shareyourcloning_linkml:right ] ;
     sh:targetClass shareyourcloning_linkml:AssemblyJoin .
 
 shareyourcloning_linkml:Sequence a sh:NodeShape ;
     sh:closed false ;
     sh:description "Represents a sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
@@ -942,8 +953,7 @@
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:Sequence .
-
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/shex/shareyourcloning_linkml.shex` & `shareyourcloning_linkml-0.1.4a0/project/shex/shareyourcloning_linkml.shex`

 * *Files 5% similar despite different names*

```diff
@@ -51,23 +51,30 @@
              <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full> ] ?
        ) ;
        rdf:type [ <AddGeneIdSource> ]
     )
 }
 
 <AssemblyJoin> CLOSED {
-    (  $<AssemblyJoin_tes> (  <left_fragment> @<Sequence> ;
-          <right_fragment> @<Sequence> ;
-          <left_location> @<SimpleSequenceLocation> ;
-          <right_location> @<SimpleSequenceLocation>
+    (  $<AssemblyJoin_tes> (  <left> @<AssemblyJoinComponent> ;
+          <right> @<AssemblyJoinComponent>
        ) ;
        rdf:type [ <AssemblyJoin> ] ?
     )
 }
 
+<AssemblyJoinComponent> CLOSED {
+    (  $<AssemblyJoinComponent_tes> (  <sequence> @<Sequence> ;
+          <location> @<SimpleSequenceLocation> ;
+          <reverse_complemented> @linkml:Boolean
+       ) ;
+       rdf:type [ <AssemblyJoinComponent> ] ?
+    )
+}
+
 <AssemblySource>  (
     CLOSED {
        (  $<AssemblySource_tes> (  &<Source_tes> ;
              rdf:type [ <Source> ] ? ;
              <circular> @linkml:Boolean ? ;
              <assembly> @<AssemblyJoin> +
           ) ;
@@ -326,9 +333,7 @@
              <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> ] ;
           <file_name> @linkml:String ? ;
           <index_in_file> @linkml:Integer ?
        ) ;
        rdf:type [ <UploadedFileSource> ]
     )
 }
-
-
```

### Comparing `shareyourcloning_linkml-0.1.3a0/project/sqlschema/shareyourcloning_linkml.sql` & `shareyourcloning_linkml-0.1.4a0/project/sqlschema/shareyourcloning_linkml.sql`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,61 @@
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 --     * Slot: CloningStrategy_id Description: Autocreated FK slot
 -- # Class: "TextFileSequence" Description: "A sequence (may have features) defined by the content of a text file"
 --     * Slot: sequence_file_format Description: The format of a sequence file
 --     * Slot: overhang_crick_3prime Description: Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand
 --     * Slot: overhang_watson_3prime Description: The equivalent of `overhang_crick_3prime` but for the watson strand
---     * Slot: file_content Description: 
+--     * Slot: file_content Description:
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 -- # Class: "Primer" Description: "An oligonucleotide or primer"
 --     * Slot: name Description: A human-readable name for a thing
---     * Slot: sequence Description: 
+--     * Slot: sequence Description:
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 -- # Class: "SequenceCut" Description: "Represents a cut in a DNA sequence"
---     * Slot: id Description: 
+--     * Slot: id Description:
 --     * Slot: cut_watson Description: The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.
 --     * Slot: overhang Description: The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.
 -- # Class: "RestrictionSequenceCut" Description: "Represents a cut in a DNA sequence that is made by a restriction enzyme"
---     * Slot: id Description: 
---     * Slot: restriction_enzyme Description: 
+--     * Slot: id Description:
+--     * Slot: restriction_enzyme Description:
 --     * Slot: cut_watson Description: The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.
 --     * Slot: overhang Description: The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.
 -- # Class: "Source" Description: "Represents the source of a sequence"
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: CloningStrategy_id Description: Autocreated FK slot
 -- # Class: "ManuallyTypedSource" Description: "Represents the source of a sequence that is manually typed by the user"
 --     * Slot: overhang_crick_3prime Description: Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand
 --     * Slot: overhang_watson_3prime Description: The equivalent of `overhang_crick_3prime` but for the watson strand
---     * Slot: user_input Description: 
+--     * Slot: user_input Description:
 --     * Slot: circular Description: Whether the sequence is circular or not
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "UploadedFileSource" Description: "Represents the source of a sequence that is uploaded as a file"
 --     * Slot: sequence_file_format Description: The format of a sequence file
 --     * Slot: file_name Description: The name of the file
 --     * Slot: index_in_file Description: The index of the sequence in the file
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "RepositoryIdSource" Description: "Represents the source of a sequence that is identified by a repository id"
---     * Slot: repository_name Description: 
+--     * Slot: repository_name Description:
 --     * Slot: repository_id Description: The id of the sequence in the repository
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "AddGeneIdSource" Description: "Represents the source of a sequence that is identified by an AddGene id"
 --     * Slot: sequence_file_url Description: The URL of a sequence file
---     * Slot: addgene_sequence_type Description: 
---     * Slot: repository_name Description: 
+--     * Slot: addgene_sequence_type Description:
+--     * Slot: repository_name Description:
 --     * Slot: repository_id Description: The id of the sequence in the repository
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "GenomeCoordinatesSource" Description: "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI"
 --     * Slot: assembly_accession Description: The accession of the assembly
 --     * Slot: sequence_accession Description: The accession of the sequence
@@ -70,40 +70,43 @@
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "SequenceCutSource" Description: "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting."
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
---     * Slot: left_edge_id Description: 
---     * Slot: right_edge_id Description: 
+--     * Slot: left_edge_id Description:
+--     * Slot: right_edge_id Description:
 -- # Class: "RestrictionEnzymeDigestionSource" Description: "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes."
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
---     * Slot: left_edge_id Description: 
---     * Slot: right_edge_id Description: 
+--     * Slot: left_edge_id Description:
+--     * Slot: right_edge_id Description:
 -- # Class: "SimpleSequenceLocation" Description: "Represents a location within a sequence, for now support for ranges only"
---     * Slot: id Description: 
+--     * Slot: id Description:
 --     * Slot: start Description: The starting coordinate (1-based) of the location
 --     * Slot: end Description: The ending coordinate (1-based) of the location
 --     * Slot: strand Description: The strand of the location, should be 1 or -1 or null
+-- # Class: "AssemblyJoinComponent" Description: "Represents a component of a join between two fragments in an assembly"
+--     * Slot: id Description:
+--     * Slot: sequence Description:
+--     * Slot: reverse_complemented Description: Whether the sequence is reverse complemented in the join
+--     * Slot: location_id Description: Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join.
 -- # Class: "AssemblyJoin" Description: "Represents a joint between two fragments in an assembly"
---     * Slot: id Description: 
---     * Slot: left_fragment Description: 
---     * Slot: right_fragment Description: 
+--     * Slot: id Description:
 --     * Slot: AssemblySource_id Description: Autocreated FK slot
 --     * Slot: PCRSource_id Description: Autocreated FK slot
 --     * Slot: LigationSource_id Description: Autocreated FK slot
 --     * Slot: HomologousRecombinationSource_id Description: Autocreated FK slot
 --     * Slot: GibsonAssemblySource_id Description: Autocreated FK slot
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
 --     * Slot: CRISPRSource_id Description: Autocreated FK slot
---     * Slot: left_location_id Description: Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join.
---     * Slot: right_location_id Description: Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join.
+--     * Slot: left_id Description:
+--     * Slot: right_id Description:
 -- # Class: "AssemblySource" Description: "Represents the source of a sequence that is an assembly of other sequences"
 --     * Slot: circular Description: Whether the assembly is circular or not
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "PCRSource" Description: "Represents the source of a sequence that is generated by PCR"
 --     * Slot: forward_primer Description: The forward primer used in the PCR
@@ -145,15 +148,15 @@
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "PolymeraseExtensionSource" Description: "Represents the source of a sequence that is generated by polymerase extension"
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "CloningStrategy" Description: "Represents a cloning strategy"
---     * Slot: id Description: 
+--     * Slot: id Description:
 --     * Slot: description Description: A description of the cloning strategy
 -- # Class: "Source_input" Description: ""
 --     * Slot: Source_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "ManuallyTypedSource_input" Description: ""
 --     * Slot: ManuallyTypedSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
@@ -188,15 +191,15 @@
 --     * Slot: HomologousRecombinationSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "GibsonAssemblySource_input" Description: ""
 --     * Slot: GibsonAssemblySource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "RestrictionAndLigationSource_restriction_enzymes" Description: ""
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
---     * Slot: restriction_enzymes Description: 
+--     * Slot: restriction_enzymes Description:
 -- # Class: "RestrictionAndLigationSource_input" Description: ""
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "CRISPRSource_guides" Description: ""
 --     * Slot: CRISPRSource_id Description: Autocreated FK slot
 --     * Slot: guides_id Description: The guide RNAs used in the CRISPR
 -- # Class: "CRISPRSource_input" Description: ""
@@ -209,388 +212,393 @@
 --     * Slot: PolymeraseExtensionSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "CloningStrategy_primers" Description: ""
 --     * Slot: CloningStrategy_id Description: Autocreated FK slot
 --     * Slot: primers_id Description: The primers that are used in the cloning strategy
 
 CREATE TABLE "NamedThing" (
-	id INTEGER NOT NULL, 
+	id INTEGER NOT NULL,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "TextFileSequence" (
-	sequence_file_format VARCHAR(8) NOT NULL, 
-	overhang_crick_3prime INTEGER, 
-	overhang_watson_3prime INTEGER, 
-	file_content TEXT, 
-	id INTEGER NOT NULL, 
-	type TEXT, 
+	sequence_file_format VARCHAR(8) NOT NULL,
+	overhang_crick_3prime INTEGER,
+	overhang_watson_3prime INTEGER,
+	file_content TEXT,
+	id INTEGER NOT NULL,
+	type TEXT,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "Primer" (
-	name TEXT, 
-	sequence TEXT, 
-	id INTEGER NOT NULL, 
-	type TEXT, 
+	name TEXT,
+	sequence TEXT,
+	id INTEGER NOT NULL,
+	type TEXT,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "SequenceCut" (
-	id INTEGER NOT NULL, 
-	cut_watson INTEGER NOT NULL, 
-	overhang INTEGER NOT NULL, 
+	id INTEGER NOT NULL,
+	cut_watson INTEGER NOT NULL,
+	overhang INTEGER NOT NULL,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "RestrictionSequenceCut" (
-	id INTEGER NOT NULL, 
-	restriction_enzyme TEXT NOT NULL, 
-	cut_watson INTEGER NOT NULL, 
-	overhang INTEGER NOT NULL, 
+	id INTEGER NOT NULL,
+	restriction_enzyme TEXT NOT NULL,
+	cut_watson INTEGER NOT NULL,
+	overhang INTEGER NOT NULL,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "SimpleSequenceLocation" (
-	id INTEGER NOT NULL, 
-	start INTEGER NOT NULL, 
-	"end" INTEGER NOT NULL, 
-	strand INTEGER, 
+	id INTEGER NOT NULL,
+	start INTEGER NOT NULL,
+	"end" INTEGER NOT NULL,
+	strand INTEGER,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "CloningStrategy" (
-	id INTEGER NOT NULL, 
-	description TEXT, 
+	id INTEGER NOT NULL,
+	description TEXT,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "Sequence" (
-	id INTEGER NOT NULL, 
-	type TEXT, 
-	"CloningStrategy_id" INTEGER, 
-	PRIMARY KEY (id), 
+	id INTEGER NOT NULL,
+	type TEXT,
+	"CloningStrategy_id" INTEGER,
+	PRIMARY KEY (id),
 	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id)
 );
 CREATE TABLE "CloningStrategy_primers" (
-	"CloningStrategy_id" INTEGER, 
-	primers_id INTEGER, 
-	PRIMARY KEY ("CloningStrategy_id", primers_id), 
-	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id), 
+	"CloningStrategy_id" INTEGER,
+	primers_id INTEGER,
+	PRIMARY KEY ("CloningStrategy_id", primers_id),
+	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id),
 	FOREIGN KEY(primers_id) REFERENCES "Primer" (id)
 );
 CREATE TABLE "Source" (
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	"CloningStrategy_id" INTEGER, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(output) REFERENCES "Sequence" (id), 
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	"CloningStrategy_id" INTEGER,
+	PRIMARY KEY (id),
+	FOREIGN KEY(output) REFERENCES "Sequence" (id),
 	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id)
 );
 CREATE TABLE "ManuallyTypedSource" (
-	overhang_crick_3prime INTEGER, 
-	overhang_watson_3prime INTEGER, 
-	user_input TEXT NOT NULL, 
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	overhang_crick_3prime INTEGER,
+	overhang_watson_3prime INTEGER,
+	user_input TEXT NOT NULL,
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "UploadedFileSource" (
-	sequence_file_format VARCHAR(8) NOT NULL, 
-	file_name TEXT, 
-	index_in_file INTEGER, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	sequence_file_format VARCHAR(8) NOT NULL,
+	file_name TEXT,
+	index_in_file INTEGER,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "RepositoryIdSource" (
-	repository_name VARCHAR(7) NOT NULL, 
-	repository_id TEXT NOT NULL, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	repository_name VARCHAR(7) NOT NULL,
+	repository_id TEXT NOT NULL,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "AddGeneIdSource" (
-	sequence_file_url TEXT, 
-	addgene_sequence_type VARCHAR(14), 
-	repository_name VARCHAR(7) NOT NULL, 
-	repository_id TEXT NOT NULL, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	sequence_file_url TEXT,
+	addgene_sequence_type VARCHAR(14),
+	repository_name VARCHAR(7) NOT NULL,
+	repository_id TEXT NOT NULL,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "GenomeCoordinatesSource" (
-	assembly_accession TEXT, 
-	sequence_accession TEXT NOT NULL, 
-	locus_tag TEXT, 
-	gene_id INTEGER, 
-	start INTEGER NOT NULL, 
-	"end" INTEGER NOT NULL, 
-	strand INTEGER NOT NULL, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	assembly_accession TEXT,
+	sequence_accession TEXT NOT NULL,
+	locus_tag TEXT,
+	gene_id INTEGER,
+	start INTEGER NOT NULL,
+	"end" INTEGER NOT NULL,
+	strand INTEGER NOT NULL,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "SequenceCutSource" (
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	left_edge_id INTEGER, 
-	right_edge_id INTEGER, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(output) REFERENCES "Sequence" (id), 
-	FOREIGN KEY(left_edge_id) REFERENCES "SequenceCut" (id), 
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	left_edge_id INTEGER,
+	right_edge_id INTEGER,
+	PRIMARY KEY (id),
+	FOREIGN KEY(output) REFERENCES "Sequence" (id),
+	FOREIGN KEY(left_edge_id) REFERENCES "SequenceCut" (id),
 	FOREIGN KEY(right_edge_id) REFERENCES "SequenceCut" (id)
 );
 CREATE TABLE "RestrictionEnzymeDigestionSource" (
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	left_edge_id INTEGER, 
-	right_edge_id INTEGER, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(output) REFERENCES "Sequence" (id), 
-	FOREIGN KEY(left_edge_id) REFERENCES "RestrictionSequenceCut" (id), 
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	left_edge_id INTEGER,
+	right_edge_id INTEGER,
+	PRIMARY KEY (id),
+	FOREIGN KEY(output) REFERENCES "Sequence" (id),
+	FOREIGN KEY(left_edge_id) REFERENCES "RestrictionSequenceCut" (id),
 	FOREIGN KEY(right_edge_id) REFERENCES "RestrictionSequenceCut" (id)
 );
+CREATE TABLE "AssemblyJoinComponent" (
+	id INTEGER NOT NULL,
+	sequence INTEGER NOT NULL,
+	reverse_complemented BOOLEAN NOT NULL,
+	location_id INTEGER NOT NULL,
+	PRIMARY KEY (id),
+	FOREIGN KEY(sequence) REFERENCES "Sequence" (id),
+	FOREIGN KEY(location_id) REFERENCES "SimpleSequenceLocation" (id)
+);
 CREATE TABLE "AssemblySource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "PCRSource" (
-	forward_primer INTEGER NOT NULL, 
-	reverse_primer INTEGER NOT NULL, 
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(forward_primer) REFERENCES "Primer" (id), 
-	FOREIGN KEY(reverse_primer) REFERENCES "Primer" (id), 
+	forward_primer INTEGER NOT NULL,
+	reverse_primer INTEGER NOT NULL,
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
+	FOREIGN KEY(forward_primer) REFERENCES "Primer" (id),
+	FOREIGN KEY(reverse_primer) REFERENCES "Primer" (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "LigationSource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "HomologousRecombinationSource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "GibsonAssemblySource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "RestrictionAndLigationSource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "CRISPRSource" (
-	circular BOOLEAN, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	circular BOOLEAN,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "OligoHybridizationSource" (
-	overhang_crick_3prime INTEGER, 
-	forward_oligo INTEGER NOT NULL, 
-	reverse_oligo INTEGER NOT NULL, 
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(forward_oligo) REFERENCES "Primer" (id), 
-	FOREIGN KEY(reverse_oligo) REFERENCES "Primer" (id), 
+	overhang_crick_3prime INTEGER,
+	forward_oligo INTEGER NOT NULL,
+	reverse_oligo INTEGER NOT NULL,
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
+	FOREIGN KEY(forward_oligo) REFERENCES "Primer" (id),
+	FOREIGN KEY(reverse_oligo) REFERENCES "Primer" (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "PolymeraseExtensionSource" (
-	output INTEGER, 
-	type TEXT, 
-	id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
+	output INTEGER,
+	type TEXT,
+	id INTEGER NOT NULL,
+	PRIMARY KEY (id),
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "AssemblyJoin" (
-	id INTEGER NOT NULL, 
-	left_fragment INTEGER NOT NULL, 
-	right_fragment INTEGER NOT NULL, 
-	"AssemblySource_id" INTEGER, 
-	"PCRSource_id" INTEGER, 
-	"LigationSource_id" INTEGER, 
-	"HomologousRecombinationSource_id" INTEGER, 
-	"GibsonAssemblySource_id" INTEGER, 
-	"RestrictionAndLigationSource_id" INTEGER, 
-	"CRISPRSource_id" INTEGER, 
-	left_location_id INTEGER NOT NULL, 
-	right_location_id INTEGER NOT NULL, 
-	PRIMARY KEY (id), 
-	FOREIGN KEY(left_fragment) REFERENCES "Sequence" (id), 
-	FOREIGN KEY(right_fragment) REFERENCES "Sequence" (id), 
-	FOREIGN KEY("AssemblySource_id") REFERENCES "AssemblySource" (id), 
-	FOREIGN KEY("PCRSource_id") REFERENCES "PCRSource" (id), 
-	FOREIGN KEY("LigationSource_id") REFERENCES "LigationSource" (id), 
-	FOREIGN KEY("HomologousRecombinationSource_id") REFERENCES "HomologousRecombinationSource" (id), 
-	FOREIGN KEY("GibsonAssemblySource_id") REFERENCES "GibsonAssemblySource" (id), 
-	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id), 
-	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
-	FOREIGN KEY(left_location_id) REFERENCES "SimpleSequenceLocation" (id), 
-	FOREIGN KEY(right_location_id) REFERENCES "SimpleSequenceLocation" (id)
+	id INTEGER NOT NULL,
+	"AssemblySource_id" INTEGER,
+	"PCRSource_id" INTEGER,
+	"LigationSource_id" INTEGER,
+	"HomologousRecombinationSource_id" INTEGER,
+	"GibsonAssemblySource_id" INTEGER,
+	"RestrictionAndLigationSource_id" INTEGER,
+	"CRISPRSource_id" INTEGER,
+	left_id INTEGER NOT NULL,
+	right_id INTEGER NOT NULL,
+	PRIMARY KEY (id),
+	FOREIGN KEY("AssemblySource_id") REFERENCES "AssemblySource" (id),
+	FOREIGN KEY("PCRSource_id") REFERENCES "PCRSource" (id),
+	FOREIGN KEY("LigationSource_id") REFERENCES "LigationSource" (id),
+	FOREIGN KEY("HomologousRecombinationSource_id") REFERENCES "HomologousRecombinationSource" (id),
+	FOREIGN KEY("GibsonAssemblySource_id") REFERENCES "GibsonAssemblySource" (id),
+	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id),
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id),
+	FOREIGN KEY(left_id) REFERENCES "AssemblyJoinComponent" (id),
+	FOREIGN KEY(right_id) REFERENCES "AssemblyJoinComponent" (id)
 );
 CREATE TABLE "Source_input" (
-	"Source_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("Source_id", input_id), 
-	FOREIGN KEY("Source_id") REFERENCES "Source" (id), 
+	"Source_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("Source_id", input_id),
+	FOREIGN KEY("Source_id") REFERENCES "Source" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "ManuallyTypedSource_input" (
-	"ManuallyTypedSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("ManuallyTypedSource_id", input_id), 
-	FOREIGN KEY("ManuallyTypedSource_id") REFERENCES "ManuallyTypedSource" (id), 
+	"ManuallyTypedSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("ManuallyTypedSource_id", input_id),
+	FOREIGN KEY("ManuallyTypedSource_id") REFERENCES "ManuallyTypedSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "UploadedFileSource_input" (
-	"UploadedFileSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("UploadedFileSource_id", input_id), 
-	FOREIGN KEY("UploadedFileSource_id") REFERENCES "UploadedFileSource" (id), 
+	"UploadedFileSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("UploadedFileSource_id", input_id),
+	FOREIGN KEY("UploadedFileSource_id") REFERENCES "UploadedFileSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "RepositoryIdSource_input" (
-	"RepositoryIdSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("RepositoryIdSource_id", input_id), 
-	FOREIGN KEY("RepositoryIdSource_id") REFERENCES "RepositoryIdSource" (id), 
+	"RepositoryIdSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("RepositoryIdSource_id", input_id),
+	FOREIGN KEY("RepositoryIdSource_id") REFERENCES "RepositoryIdSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "AddGeneIdSource_input" (
-	"AddGeneIdSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("AddGeneIdSource_id", input_id), 
-	FOREIGN KEY("AddGeneIdSource_id") REFERENCES "AddGeneIdSource" (id), 
+	"AddGeneIdSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("AddGeneIdSource_id", input_id),
+	FOREIGN KEY("AddGeneIdSource_id") REFERENCES "AddGeneIdSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "GenomeCoordinatesSource_input" (
-	"GenomeCoordinatesSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("GenomeCoordinatesSource_id", input_id), 
-	FOREIGN KEY("GenomeCoordinatesSource_id") REFERENCES "GenomeCoordinatesSource" (id), 
+	"GenomeCoordinatesSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("GenomeCoordinatesSource_id", input_id),
+	FOREIGN KEY("GenomeCoordinatesSource_id") REFERENCES "GenomeCoordinatesSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "SequenceCutSource_input" (
-	"SequenceCutSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("SequenceCutSource_id", input_id), 
-	FOREIGN KEY("SequenceCutSource_id") REFERENCES "SequenceCutSource" (id), 
+	"SequenceCutSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("SequenceCutSource_id", input_id),
+	FOREIGN KEY("SequenceCutSource_id") REFERENCES "SequenceCutSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "RestrictionEnzymeDigestionSource_input" (
-	"RestrictionEnzymeDigestionSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("RestrictionEnzymeDigestionSource_id", input_id), 
-	FOREIGN KEY("RestrictionEnzymeDigestionSource_id") REFERENCES "RestrictionEnzymeDigestionSource" (id), 
+	"RestrictionEnzymeDigestionSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("RestrictionEnzymeDigestionSource_id", input_id),
+	FOREIGN KEY("RestrictionEnzymeDigestionSource_id") REFERENCES "RestrictionEnzymeDigestionSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "AssemblySource_input" (
-	"AssemblySource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("AssemblySource_id", input_id), 
-	FOREIGN KEY("AssemblySource_id") REFERENCES "AssemblySource" (id), 
+	"AssemblySource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("AssemblySource_id", input_id),
+	FOREIGN KEY("AssemblySource_id") REFERENCES "AssemblySource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "PCRSource_input" (
-	"PCRSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("PCRSource_id", input_id), 
-	FOREIGN KEY("PCRSource_id") REFERENCES "PCRSource" (id), 
+	"PCRSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("PCRSource_id", input_id),
+	FOREIGN KEY("PCRSource_id") REFERENCES "PCRSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "LigationSource_input" (
-	"LigationSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("LigationSource_id", input_id), 
-	FOREIGN KEY("LigationSource_id") REFERENCES "LigationSource" (id), 
+	"LigationSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("LigationSource_id", input_id),
+	FOREIGN KEY("LigationSource_id") REFERENCES "LigationSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "HomologousRecombinationSource_input" (
-	"HomologousRecombinationSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("HomologousRecombinationSource_id", input_id), 
-	FOREIGN KEY("HomologousRecombinationSource_id") REFERENCES "HomologousRecombinationSource" (id), 
+	"HomologousRecombinationSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("HomologousRecombinationSource_id", input_id),
+	FOREIGN KEY("HomologousRecombinationSource_id") REFERENCES "HomologousRecombinationSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "GibsonAssemblySource_input" (
-	"GibsonAssemblySource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("GibsonAssemblySource_id", input_id), 
-	FOREIGN KEY("GibsonAssemblySource_id") REFERENCES "GibsonAssemblySource" (id), 
+	"GibsonAssemblySource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("GibsonAssemblySource_id", input_id),
+	FOREIGN KEY("GibsonAssemblySource_id") REFERENCES "GibsonAssemblySource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "RestrictionAndLigationSource_restriction_enzymes" (
-	"RestrictionAndLigationSource_id" INTEGER, 
-	restriction_enzymes TEXT NOT NULL, 
-	PRIMARY KEY ("RestrictionAndLigationSource_id", restriction_enzymes), 
+	"RestrictionAndLigationSource_id" INTEGER,
+	restriction_enzymes TEXT NOT NULL,
+	PRIMARY KEY ("RestrictionAndLigationSource_id", restriction_enzymes),
 	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id)
 );
 CREATE TABLE "RestrictionAndLigationSource_input" (
-	"RestrictionAndLigationSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("RestrictionAndLigationSource_id", input_id), 
-	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id), 
+	"RestrictionAndLigationSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("RestrictionAndLigationSource_id", input_id),
+	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "CRISPRSource_guides" (
-	"CRISPRSource_id" INTEGER, 
-	guides_id INTEGER NOT NULL, 
-	PRIMARY KEY ("CRISPRSource_id", guides_id), 
-	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
+	"CRISPRSource_id" INTEGER,
+	guides_id INTEGER NOT NULL,
+	PRIMARY KEY ("CRISPRSource_id", guides_id),
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id),
 	FOREIGN KEY(guides_id) REFERENCES "Primer" (id)
 );
 CREATE TABLE "CRISPRSource_input" (
-	"CRISPRSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("CRISPRSource_id", input_id), 
-	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
+	"CRISPRSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("CRISPRSource_id", input_id),
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "OligoHybridizationSource_input" (
-	"OligoHybridizationSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("OligoHybridizationSource_id", input_id), 
-	FOREIGN KEY("OligoHybridizationSource_id") REFERENCES "OligoHybridizationSource" (id), 
+	"OligoHybridizationSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("OligoHybridizationSource_id", input_id),
+	FOREIGN KEY("OligoHybridizationSource_id") REFERENCES "OligoHybridizationSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
 CREATE TABLE "PolymeraseExtensionSource_input" (
-	"PolymeraseExtensionSource_id" INTEGER, 
-	input_id INTEGER, 
-	PRIMARY KEY ("PolymeraseExtensionSource_id", input_id), 
-	FOREIGN KEY("PolymeraseExtensionSource_id") REFERENCES "PolymeraseExtensionSource" (id), 
+	"PolymeraseExtensionSource_id" INTEGER,
+	input_id INTEGER,
+	PRIMARY KEY ("PolymeraseExtensionSource_id", input_id),
+	FOREIGN KEY("PolymeraseExtensionSource_id") REFERENCES "PolymeraseExtensionSource" (id),
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
-);
+);
```

### Comparing `shareyourcloning_linkml-0.1.3a0/pyproject.toml` & `shareyourcloning_linkml-0.1.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Manuel Lera-Ramirez <manuel.lera-ramirez@ucl.ac.uk>"]
 description = "A LinkML data model for ShareYourCloning"
 include = ["README.md", "src/shareyourcloning_linkml/schema", "project"]
 license = "MIT"
 name = "shareyourcloning-linkml"
 readme = "README.md"
-version = "0.1.3a0"
+version = "0.1.4a0"
 
 homepage = "https://github.com/genestorian/ShareYourCloning_LinkML"
 repository = "https://github.com/genestorian/ShareYourCloning_LinkML"
 documentation = "https://genestorian.github.io/ShareYourCloning_LinkML"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/_models.py` & `shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,29 +333,34 @@
     """
 
     start: int = Field(..., description="""The starting coordinate (1-based) of the location""")
     end: int = Field(..., description="""The ending coordinate (1-based) of the location""")
     strand: Optional[int] = Field(None, description="""The strand of the location, should be 1 or -1 or null""")
 
 
-class AssemblyJoin(ConfiguredBaseModel):
+class AssemblyJoinComponent(ConfiguredBaseModel):
     """
-    Represents a joint between two fragments in an assembly
+    Represents a component of a join between two fragments in an assembly
     """
 
-    left_fragment: int = Field(...)
-    right_fragment: int = Field(...)
-    left_location: SimpleSequenceLocation = Field(
-        ...,
-        description="""Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join.""",
-    )
-    right_location: SimpleSequenceLocation = Field(
+    sequence: int = Field(...)
+    location: SimpleSequenceLocation = Field(
         ...,
-        description="""Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join.""",
+        description="""Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join.""",
     )
+    reverse_complemented: bool = Field(..., description="""Whether the sequence is reverse complemented in the join""")
+
+
+class AssemblyJoin(ConfiguredBaseModel):
+    """
+    Represents a joint between two fragments in an assembly
+    """
+
+    left: AssemblyJoinComponent = Field(...)
+    right: AssemblyJoinComponent = Field(...)
 
 
 class AssemblySource(Source):
     """
     Represents the source of a sequence that is an assembly of other sequences
     """
 
@@ -594,14 +599,15 @@
 UploadedFileSource.model_rebuild()
 RepositoryIdSource.model_rebuild()
 AddGeneIdSource.model_rebuild()
 GenomeCoordinatesSource.model_rebuild()
 SequenceCutSource.model_rebuild()
 RestrictionEnzymeDigestionSource.model_rebuild()
 SimpleSequenceLocation.model_rebuild()
+AssemblyJoinComponent.model_rebuild()
 AssemblyJoin.model_rebuild()
 AssemblySource.model_rebuild()
 PCRSource.model_rebuild()
 LigationSource.model_rebuild()
 HomologousRecombinationSource.model_rebuild()
 GibsonAssemblySource.model_rebuild()
 RestrictionAndLigationSource.model_rebuild()
```

### Comparing `shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml` & `shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -271,38 +271,44 @@
           required: true
       - strand:
           range: integer
           description: >-
             The strand of the location, should be 1 or -1 or null
           required: false
 
-  AssemblyJoin:
+  AssemblyJoinComponent:
     description: >-
-      Represents a joint between two fragments in an assembly
+      Represents a component of a join between two fragments in an assembly
     attributes:
-      - left_fragment:
-          range: Sequence
-          required: true
-      - right_fragment:
+      - sequence:
           range: Sequence
           required: true
-      - left_location:
+      - location:
           range: SimpleSequenceLocation
           description: >-
-            Location of the overlap in the left fragment. Might be
+            Location of the overlap in the fragment. Might be
             an empty location (start == end) to indicate blunt join.
           required: true
           inlined: true
-      - right_location:
-          range: SimpleSequenceLocation
+      - reverse_complemented:
+          range: boolean
           description: >-
-            Location of the overlap in the right fragment. Might be
-            an empty location (start == end) to indicate blunt join.
+            Whether the sequence is reverse complemented in the join
+          required: true
+
+  AssemblyJoin:
+    description: >-
+      Represents a joint between two fragments in an assembly
+    attributes:
+      - left:
+          range: AssemblyJoinComponent
+          required: true
+      - right:
+          range: AssemblyJoinComponent
           required: true
-          inlined: true
 
   AssemblySource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is an assembly of other sequences
     attributes:
       - circular:
```

### Comparing `shareyourcloning_linkml-0.1.3a0/PKG-INFO` & `shareyourcloning_linkml-0.1.4a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareyourcloning-linkml
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: A LinkML data model for ShareYourCloning
 Home-page: https://github.com/genestorian/ShareYourCloning_LinkML
 License: MIT
 Author: Manuel Lera-Ramirez
 Author-email: manuel.lera-ramirez@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

