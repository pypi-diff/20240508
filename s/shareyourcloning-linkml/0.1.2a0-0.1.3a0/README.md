# Comparing `tmp/shareyourcloning_linkml-0.1.2a0.tar.gz` & `tmp/shareyourcloning_linkml-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareyourcloning_linkml-0.1.2a0.tar", max compression
+gzip compressed data, was "shareyourcloning_linkml-0.1.3a0.tar", max compression
```

## Comparing `shareyourcloning_linkml-0.1.2a0.tar` & `shareyourcloning_linkml-0.1.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1087 2024-04-24 17:05:35.037819 shareyourcloning_linkml-0.1.2a0/LICENSE
--rw-r--r--   0        0        0      923 2024-04-24 17:05:35.037819 shareyourcloning_linkml-0.1.2a0/README.md
--rw-r--r--   0        0        0    15880 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/excel/shareyourcloning_linkml.xlsx
--rw-r--r--   0        0        0     3623 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/graphql/shareyourcloning_linkml.graphql
--rw-r--r--   0        0        0     6281 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/jsonld/shareyourcloning_linkml.context.jsonld
--rw-r--r--   0        0        0    67794 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/jsonld/shareyourcloning_linkml.jsonld
--rw-r--r--   0        0        0    36392 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/jsonschema/shareyourcloning_linkml.schema.json
--rw-r--r--   0        0        0    46329 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/owl/shareyourcloning_linkml.owl.ttl
--rw-r--r--   0        0        0      400 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/prefixmap/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     5299 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/protobuf/shareyourcloning_linkml.proto
--rw-r--r--   0        0        0    52906 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/python/shareyourcloning_linkml.py
--rw-r--r--   0        0        0    38399 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/shacl/shareyourcloning_linkml.shacl.ttl
--rw-r--r--   0        0        0     8274 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/shex/shareyourcloning_linkml.shex
--rw-r--r--   0        0        0    27043 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/project/sqlschema/shareyourcloning_linkml.sql
--rw-r--r--   0        0        0     1499 2024-04-24 17:05:48.937845 shareyourcloning_linkml-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0      186 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/_version.py
--rw-r--r--   0        0        0       41 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/datamodel/__init__.py
--rw-r--r--   0        0        0    22283 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/datamodel/_models.py
--rw-r--r--   0        0        0       42 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/datamodel/models.py
--rw-r--r--   0        0        0    13200 2024-04-24 17:05:35.041819 shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/LICENSE
+-rw-r--r--   0        0        0      923 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/README.md
+-rw-r--r--   0        0        0    17108 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/excel/shareyourcloning_linkml.xlsx
+-rw-r--r--   0        0        0     4114 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/graphql/shareyourcloning_linkml.graphql
+-rw-r--r--   0        0        0     6825 2024-05-08 09:21:45.372750 shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.context.jsonld
+-rw-r--r--   0        0        0    81533 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.jsonld
+-rw-r--r--   0        0        0    41625 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/jsonschema/shareyourcloning_linkml.schema.json
+-rw-r--r--   0        0        0    54043 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/owl/shareyourcloning_linkml.owl.ttl
+-rw-r--r--   0        0        0      400 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/prefixmap/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     5967 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/protobuf/shareyourcloning_linkml.proto
+-rw-r--r--   0        0        0    63629 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/python/shareyourcloning_linkml.py
+-rw-r--r--   0        0        0    43592 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/shacl/shareyourcloning_linkml.shacl.ttl
+-rw-r--r--   0        0        0     9441 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/shex/shareyourcloning_linkml.shex
+-rw-r--r--   0        0        0    30615 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/project/sqlschema/shareyourcloning_linkml.sql
+-rw-r--r--   0        0        0     1499 2024-05-08 09:21:56.632731 shareyourcloning_linkml-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0      186 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/_version.py
+-rw-r--r--   0        0        0       41 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/__init__.py
+-rw-r--r--   0        0        0    25796 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/_models.py
+-rw-r--r--   0        0        0       42 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/models.py
+-rw-r--r--   0        0        0    15500 2024-05-08 09:21:45.376750 shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.3a0/PKG-INFO
```

### Comparing `shareyourcloning_linkml-0.1.2a0/LICENSE` & `shareyourcloning_linkml-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.2a0/README.md` & `shareyourcloning_linkml-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.2a0/project/excel/shareyourcloning_linkml.xlsx` & `shareyourcloning_linkml-0.1.3a0/project/excel/shareyourcloning_linkml.xlsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,993 +1,1070 @@
-00000000: 504b 0304 1400 0000 0800 7d88 9858 465a  PK........}..XFZ
+00000000: 504b 0304 1400 0000 0800 d050 a858 465a  PK.........P.XFZ
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
-000000b0: 504b 0304 1400 0000 0800 7d88 9858 922b  PK........}..X.+
-000000c0: 0ab7 eb00 0000 cb01 0000 1100 0000 646f  ..............do
-000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6ca5  cProps/core.xml.
-000000e0: 914d 4fc3 300c 86ff ca94 7beb 7e31 89a8  .MO.0.....{.~1..
-000000f0: cb05 c409 2424 2681 b845 89b7 456b 9a28  ....$$&..E..Ek.(
-00000100: 316a f7ef 49cb d681 e0c6 317e 1f3f b695  1j..I.....1~.?..
-00000110: 5679 ae5c c0e7 e03c 0632 1857 a3ed fac8  Vy.\...<.2.W....
-00000120: 95df b003 91e7 0051 1dd0 ca98 27a2 4fe1  .......Q....'.O.
-00000130: ce05 2b29 3dc3 1ebc 5447 b947 a88a 620d  ..+)=...TG.G..b.
-00000140: 1649 6a49 1226 61e6 1723 3b2b b55a 94fe  .IjI.&a..#;+.Z..
-00000150: 2374 b340 2bc0 0e2d f614 a1cc 4bb8 b284  #t.@+..-....K...
-00000160: c1c6 3f1b e664 21c7 6816 6a18 867c a867  ..?..d!.h.j..|.g
-00000170: 2e6d 54c2 dbd3 e3cb bc7c 66fa 48b2 57c8  .mT......|f.H.W.
-00000180: 44ab 1557 0125 b920 a68b fc69 ec5a f856  D..W.%. ...i.Z.V
-00000190: 6ccf b3bf 0aa8 5769 02a7 93c7 0dbb 24af  l.....Wi......$.
-000001a0: f5dd fdf6 8189 aaa8 9aac 68b2 aad9 966b  ..........h....k
-000001b0: 5ed4 fce6 f67d 72fd e8bf 0aad d366 67fe  ^....}r......fg.
-000001c0: 61bc 0844 0bbf fe4d 7c02 504b 0304 1400  a..D...M|.PK....
-000001d0: 0000 0800 7d88 9858 995c 9c23 1006 0000  ....}..X.\.#....
-000001e0: 9c27 0000 1300 0000 786c 2f74 6865 6d65  .'......xl/theme
-000001f0: 2f74 6865 6d65 312e 786d 6ced 5a5b 73da  /theme1.xml.Z[s.
-00000200: 3814 7eef afd0 7867 f66d 0bc6 3681 b6b4  8.~...xg.m..6...
-00000210: 1373 6976 dbb4 9984 ed4e 1f85 1158 8d6c  .siv.....N...X.l
-00000220: 7964 9184 7fbf 4736 10cb 960d ed92 4dba  yd....G6......M.
-00000230: 9b3c 042c e9fb ce45 47e7 e838 79f3 ee2e  .<.,...EG..8y...
-00000240: 62e8 8688 94f2 7860 d92f dbd6 bbb7 2fde  b.....x`./..../.
-00000250: e057 3224 1141 3019 a7af f0c0 0aa5 4c5e  .W2$.A0.......L^
-00000260: b55a 6900 c338 7dc9 1312 c3dc 828b 084b  .Zi..8}........K
-00000270: 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db dd56  x...\.[./#.....V
-00000280: 8469 6ca1 1847 6460 7d5e 2c68 40d0 5451  .il..Gd`}^,h@.TQ
-00000290: 5a6f 5f20 b4e5 1f33 f815 cb54 8d65 a301  Zo_ ...3...T.e..
-000002a0: 1357 4126 b988 b4f2 f96c c5fc dade 3e65  .WA&.....l....>e
-000002b0: cfe9 3a1d 3281 6e30 1b58 207f ce6f a7e4  ..:.2.n0.X ..o..
-000002c0: 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7 d1d2  NZ..T...jg?Vk...
-000002d0: 4880 82c9 7d94 05ba 49f6 a3d3 1508 320d  H...}...I.....2.
-000002e0: 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada 7434  ;:.X.v|.......t4
-000002f0: 6d1a e0e3 f178 38b6 cbd2 8b70 1c04 e051  m....x8....p...Q
-00000300: bb9e c29d f46c bfa4 4109 b4a3 69d0 64d8  .....l..A...i.d.
-00000310: f6da ae91 a6aa 8d53 4fd3 f77d dfeb 9b68  .......SO..}...h
-00000320: 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad d078  ...[O.kw.......x
-00000330: 0dbe f14f 87c3 ae89 c6ab d074 eb69 2627  ...O.......t.i&'
-00000340: fdae 6ba4 e916 6842 46e3 eb7a 1215 b5e5  ..k...hBF..z....
-00000350: 40d3 2000 5870 76d6 ccd2 0396 5e29 fa75  @. .Xpv.....^).u
-00000360: 941a d91d bbdd 415c f058 ee39 8911 fec6  ......A\.X.9....
-00000370: c504 d669 d219 9634 4672 9d90 050e 0037  ...i...4Fr.....7
-00000380: c4d1 4c50 7caf 41b6 8ae0 c292 d25c 90d6  ..LP|.A......\..
-00000390: cf29 b550 1a08 9ac8 81f5 4782 21c5 dcaf  .).P......G.!...
-000003a0: fdf5 97bb c9a4 337a 9d7d 3ace 6b94 7f69  ......3z.}:.k..i
-000003b0: ab01 a7ed bb9b cf93 fc73 e8e4 9fa7 93d7  .........s......
-000003c0: 4d42 ce70 bc2c 09f1 fb23 5b61 8727 6e3b  MB.p.,...#[a.'n;
-000003d0: 1372 3a1c 6742 7ccf f6f6 91a5 2532 cfef  .r:.gB|.....%2..
-000003e0: f90a eb4e 3c67 1f56 96b0 5dcf cfe4 9e8c  ...N<g.V..].....
-000003f0: 7223 bbdd f658 7df6 4f47 6e23 d7a9 c0b3  r#...X}.OGn#....
-00000400: 22d7 9446 2445 9fc8 2dba e411 38b5 490d  "..F$E..-...8.I.
-00000410: 3213 3f08 9d86 986a 501c 02a4 0931 96a1  2.?....jP....1..
-00000420: 86f8 b4c6 ac11 e013 7db7 be08 c8df 8d88  ........}.......
-00000430: f7ab 6f9a 3d57 a158 49da 84f8 1046 1ae2  ..o.=W.XI....F..
-00000440: 9c73 e673 d16c fb07 a546 d1f6 55bc dca3  .s.s.l...F..U...
-00000450: 9758 1501 9718 df34 aa35 2cc5 d678 95c0  .X.....4.5,..x..
-00000460: f1ad 9c3c 1d13 12cd 940b 0641 8697 2426  ...<.......A..$&
-00000470: 12a9 397e 4d48 13fe 2ba5 dafe 9cd3 40f0  ..9~MH..+.....@.
-00000480: 942f 24fa 4a91 8f69 b323 a774 26cd e833  ./$.J..i.#.t&..3
-00000490: 1ac1 46af 1b75 8768 d23c 7afe 05f9 9c35  ..F..u.h.<z....5
-000004a0: 0a1c 911b 1d02 671b b346 2184 69bb f01e  ......g..F!.i...
-000004b0: af24 8e9a adc2 112b 423e 6219 361a 72b5  .$.....+B>b.6.r.
-000004c0: 1681 b671 a984 605a 12c6 d178 4ed2 b411  ...q..`Z...xN...
-000004d0: fc59 ac35 933e 60c8 eccd 9175 ced6 910e  .Y.5.>`....u....
-000004e0: 1192 5e37 423e 62ce 8b90 11bf 1e86 384a  ..^7B>b.......8J
-000004f0: 9aed a271 5804 fd9e 5ec3 49c1 e882 cb66  ...qX...^.I....f
-00000500: fdb8 7e86 d533 6c2c 8ef7 47d4 174a e40f  ..~..3l,..G..J..
-00000510: 26a7 3fe9 3234 07a3 9a59 09bd 8456 6a9f  &.?.24...Y...Vj.
-00000520: aa87 343e a81e 320a 05f1 b91e 3ee5 7a78  ..4>..2.....>.zx
-00000530: 0a37 96c6 bc50 ae82 7b01 ffd1 da37 c2ab  .7...P..{....7..
-00000540: f882 c039 7f2e 7dcf a5ef b9f4 3da1 d2b7  ...9..}.....=...
-00000550: 3723 7d67 c1d3 8b5b de46 6e5b c4fb ae31  7#}g...[.Fn[...1
-00000560: dad7 342e 2863 5772 cdc8 c754 af93 29d8  ..4.(cWr...T..).
-00000570: 399f c0ec fd68 3e9e f1ed fad9 2484 af9a  9....h>.....$...
-00000580: 592d 2316 904b 81b3 4124 b8fc 8bca f02a  Y-#..K..A$.....*
-00000590: c409 e864 5b25 09cb 54d3 6537 8a12 9e42  ...d[%..T.e7...B
-000005a0: 1b6e e953 f54a 95d7 e5af b928 b83c 5be4  .n.S.J.....(.<[.
-000005b0: e9af a174 3e2c cff9 3c5f e7b4 cd0b 3343  ...t>,..<_....3C
-000005c0: b772 4bea b694 beb5 2638 4af4 b1cc 704e  .rK.....&8J...pN
-000005d0: 1ecb 0c3b 673c 921d b677 a01d 35fb f65d  ...;g<...w..5..]
-000005e0: 76e4 23a5 3053 9743 b81a 42be 036d ba9d  v.#.0S.C..B..m..
-000005f0: dc3a 389e 9891 b90a d352 906f c3f9 e9c5  .:8......R.o....
-00000600: 781a e239 d904 b97d 9857 6de7 d8d1 d1fb  x..9...}.Wm.....
-00000610: e7c1 51b0 a3ef 3c96 1dc7 88f2 a221 eea1  ..Q...<......!..
-00000620: 8698 cfc3 4387 797b 5f98 6795 c650 3414  ....C.y{_.g..P4.
-00000630: 6d6c ac24 2c46 b760 b8d7 f12c 14e0 6460  ml.$,F.`...,..d`
-00000640: 2da0 0783 af51 02f2 5255 6031 5bc6 032b  -....Q..RU`1[..+
-00000650: 90a2 7c4c 8c45 e870 e797 5c5f e3d1 92e3  ..|L.E.p..\_....
-00000660: dba6 65b5 6eaf 2977 196d 2252 39c2 6998  ..e.n.)w.m"R9.i.
-00000670: 1367 abca de65 b1c1 551d cf55 5bf2 b0be  .g...e..U..U[...
-00000680: 6a3d b415 4ecf fe59 adc8 9f0c 114e 160b  j=..N..Y.....N..
-00000690: 1248 6394 17a6 4aa2 f319 53be e72b 49c4  .Hc...J...S..+I.
-000006a0: 5538 bf45 33b6 1297 18bc e3e6 c771 4e53  U8.E3........qNS
-000006b0: b812 76b6 0f02 32b9 bb39 a97a 6531 67a6  ..v...2..9.ze1g.
-000006c0: f2df 2d0c 092c 5b88 5912 e24d 5ded d5e7  ..-..,[.Y..M]...
-000006d0: 9b9c ae7a 2276 fa97 77c1 60f2 fd70 c947  ...z"v..w.`..p.G
-000006e0: 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa 6e93  ..;._.]C.~....n.
-000006f0: 3b48 4c9c 79c5 1101 7445 0223 951c 0616  ;HL.y...tE.#....
-00000700: 1732 e450 ee92 9006 1301 cd94 c944 f002  .2.P.........D..
-00000710: 8264 a61c 8098 fa0b bdf2 0cb9 2915 cead  .d..........)...
-00000720: 3e39 7f45 2c83 864e 5ed2 2512 148a b00c  >9.E,..N^.%.....
-00000730: 0521 1772 e3ef ef93 6a77 8cd7 fa2c 816d  .!.r....jw...,.m
-00000740: 8454 3264 d517 ca43 89c1 3d33 7243 d854  .T2d...C..=3rC.T
-00000750: 25f3 aeda 260b 85db e254 cdbb 1abe 2660  %...&....T....&`
-00000760: 4bc3 7a6e 9d2d 27ff db5e d43d b417 3d46  K.zn.-'..^.=..=F
-00000770: f3a3 99e0 1eb3 8773 9b7a b8c2 45ac ff58  .......s.z..E..X
-00000780: d61e f932 df39 70db 3ade 035e e613 2c43  ...2.9p.:..^..,C
-00000790: a47e c17d 8a8a 8011 ab62 beba af4f f925  .~.}.....b...O.%
-000007a0: 9c3b b47b f181 209b fcd6 dba4 f6dd e00c  .;.{.. .........
-000007b0: 7cd4 ab5a a564 2b11 3f4b 077c 1f92 0663  |..Z.d+.?K.|...c
-000007c0: 8c5b f434 5f8f 1462 ada6 b1ad c6da 310c  .[.4_..b......1.
-000007d0: 7980 58f3 0ca1 6638 df87 459a 1a33 d58b  y.X...f8..E..3..
-000007e0: ac39 8d0a 6f41 d540 e53f dbd4 0d68 f60d  .9..oA.@.?...h..
-000007f0: 341c 9105 5e31 99b6 36a3 e44e 0a3c dcfe  4...^1..6..N.<..
-00000800: ef0d b0c2 c48e e1ed 8bbf 0150 4b03 0414  ...........PK...
-00000810: 0000 0008 007d 8898 58bb e88b 3838 0100  .....}..X...88..
-00000820: 0011 0200 0018 0000 0078 6c2f 776f 726b  .........xl/work
-00000830: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-00000840: 6c4d 52db 6e83 300c fd95 281f d0d0 49bb  lMR.n.0...(...I.
-00000850: a802 a4b6 d3b4 3d4c aa5a 6d7b 4ec1 40d4  ......=L.Zm{N.@.
-00000860: 2466 893b b6bf 9f03 bd3d 44f8 383e e7d8  $f.;.....=D.8>..
-00000870: 26f9 80e1 103b 0012 bfce fa58 c88e a85f  &....;.....X..._
-00000880: 2815 ab0e 9c8e 33ec c1f3 4d83 c169 6218  (.....3...M..ib.
-00000890: 5a15 fb00 ba1e 49ce aabb 2c7b 504e 1b2f  Z.....I...,{PN./
-000008a0: cb7c cc6d 4299 e391 acf1 b009 221e 9dd3  .|.mB......."...
-000008b0: e16f 0516 8742 cee5 39b1 356d 4763 4295  .o...B..9.5mGcB.
-000008c0: 79af 5bd8 017d f44c 60a8 2e3a b571 e0a3  y.[..}.L`..:.q..
-000008d0: 412f 0234 855c ce17 cb89 3156 7c1a 18e2  A/.4.\....1V|...
-000008e0: 4d2c d230 7bc4 4302 6f75 21b3 d413 58a8  M,.0{.C.ou!...X.
-000008f0: 2849 68fe fcc0 1aac 4d4a dcc9 f749 545e  (Ih.....MJ...IT^
-00000900: 4d13 f336 3ecb bf8c f373 7b7b 1d61 8df6  M..6>....s{{.a..
-00000910: cbd4 d415 f249 8a1a 1a7d b4b4 c5e1 154e  .....I...}.....N
-00000920: 33dd 5f5b 7cd6 a4cb 3ce0 2042 1ab6 ccab  3._[|...<. B....
-00000930: 1424 4b2e 343e 2d69 4781 f386 9da8 3475  .$K.4>-iG.....4u
-00000940: ae88 fd13 5215 1f66 9edb 99a4 d2aa de75  ....R..f.......u
-00000950: 688d 8fc2 42c3 2ad9 ec91 0dc3 e43d 01c2  h...B.*......=..
-00000960: 7e5c ed1e 89d0 8d61 c7bf 0c42 2ae0 fb06  ~\.....a...B*...
-00000970: 912e 20cd 7e79 05e5 3f50 4b03 0414 0000  .. .~y..?PK.....
-00000980: 0008 007d 8898 5833 636f 7aed 0100 0021  ...}..X3coz....!
-00000990: 0400 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
-000009a0: 6565 7473 2f73 6865 6574 322e 786d 6c85  eets/sheet2.xml.
-000009b0: 544d 6fdb 300c fd2b 86ce 4595 f41b 816d  TMo.0..+..E....m
-000009c0: a049 1aac 8702 458b 75c7 40b1 695b 882c  .I....E.u.@.i[.,
-000009d0: ba12 5daf ff7e 949d b8e9 9660 178b a4f8  ..]..~.....`....
-000009e0: 1e49 e9c9 7187 6eeb 2b00 8a7e d7c6 fa44  .I..q.n.+..~...D
-000009f0: 5444 cd4c 4a9f 5550 2b7f 8e0d 58de 29d0  TD.LJ.UP+...X.).
-00000a00: d58a d875 a5f4 8d03 95f7 a0da c88b c9e4  ...u............
-00000a10: 46d6 4a5b 91c6 7dec d9a5 31b6 64b4 8567  F.J[..}...1.d..g
-00000a20: 17f9 b6ae 95fb 9c83 c12e 1153 b10f bce8  ...........S....
-00000a30: b2a2 3e20 d3b8 5125 bc02 fd6c 18c0 ae1c  ..> ..Q%...l....
-00000a40: 7972 5d83 f51a 6de4 a048 c4fd 74b6 1a10  yr]...m..H..t...
-00000a50: 7dc6 9b86 ce1f d851 1866 83b8 0dce 639e  }......Q.f....c.
-00000a60: 8849 e809 0c64 1428 142f 1fb0 0063 0213  .I...d.(./...c..
-00000a70: 77f2 be23 155f 4503 f2d0 ded3 affa f9b9  w..#._E.........
-00000a80: bd8d f2b0 40f3 4be7 5425 e24e 4439 14aa  ....@.K.T%.ND9..
-00000a90: 35f4 82dd 0fd8 cd74 fdd5 e252 914a 6387  5......t...R.Jc.
-00000aa0: 5de4 c2b0 699c 0523 94e4 446d c321 bd92  ]...i..#..Dm.!..
-00000ab0: e3b8 e64a 947a 786f c166 b02e b4e1 4f5f  ...J.zxo.f....O_
-00000ac0: 3496 c41d 857d 99ed f0f3 53f8 1e96 a125  4....}....S....%
-00000ad0: b0c7 708b 5338 fc00 5729 5bae 33a7 b3ed  ..p.S8..W)[.3...
-00000ae0: fab2 717c f047 0896 ff25 e858 2568 4f33  ..q|.G...%.X%hO3
-00000af0: 3c9c 62d0 f991 ecd5 a96c fa6c fe62 977c  <.b......l.l.b.|
-00000b00: c8fb 9b1b 4e3d e7ef 9b32 9a57 be7e 1f65  ....N=...2.W.~.e
-00000b10: d85a 1a6e e1fb d6a8 848b d9fd 7472 7577  .Z.n........truw
-00000b20: 7d7b c3ea a8b0 5b3a 6c96 d8d9 a0a4 3ef0  }{....[:l.....>.
-00000b30: 689b 969e c07b 16ec 187c 700e dd61 5019  h....{...|p..aP.
-00000b40: 16fb dc28 bbed 051e 7a4d 84d1 9eb8 72b8  ...(....zM....r.
-00000b50: d3d6 a869 2a0a e549 9d95 6037 9c78 e6ad  ...i*..I..`7.x..
-00000b60: 6ad8 0611 cb31 2596 dffb fc27 e087 a7f3  j....1%....'....
-00000b70: a45c a979 4003 05cf 3739 bf65 01ba 418b  .\.y@...79.e..A.
-00000b80: 8343 d8f4 9d6c 9008 ebde acf8 0983 0b09  .C...l..........
-00000b90: bc5f 20d2 e884 b730 fe15 d23f 504b 0304  ._ ....0...?PK..
-00000ba0: 1400 0000 0800 7d88 9858 a497 6e89 5601  ......}..X..n.V.
-00000bb0: 0000 a502 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00000bc0: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
-00000bd0: 6d6c 7552 db6e c230 0cfd 952a 1f40 60d2  mluR.n.0...*.@`.
-00000be0: 2e42 6da5 019a b687 4908 b4ed 39b4 2e8d  .Bm.....I...9...
-00000bf0: 48e2 92b8 ebf8 fb39 2d97 6982 a7d8 ce39  H......9-.i....9
-00000c00: c73e 4ed2 0efd 2ed4 0094 fc58 e342 266a  .>N........X.B&j
-00000c10: a266 2a65 286a b02a 8cb0 01c7 3715 7aab  .f*e(j.*....7.z.
-00000c20: 8853 bf95 a1f1 a0ca 9e64 8dbc 1b8f 1fa4  .S.......d......
-00000c30: 55da 893c ed6b 4b9f a7d8 92d1 0e96 3e09  U..<.kK.......>.
-00000c40: adb5 ca1f 6660 b0cb c444 9c0a 2bbd ada9  ....f`...D..+...
-00000c50: 2fc8 3c6d d416 d640 1f0d 1338 9567 9d52  /.<m...@...8.g.R
-00000c60: 5b70 41a3 4b3c 5499 789e 4c17 03a3 477c  [pA.K<T.x.L...G|
-00000c70: 6ae8 c29f 3889 6636 88bb 98bc 9599 18c7  j...8.f6........
-00000c80: 99c0 4041 5142 f1f1 0d73 3026 2af1 24fb  ..@AQB...s0&*.$.
-00000c90: a3a8 b834 8dcc bff1 49fe a5f7 cfe3 6d54  ...4....I.....mT
-00000ca0: 8039 9a2f 5d52 9d89 2791 9450 a9d6 d00a  .9./]R..'..P....
-00000cb0: bb57 387a babf 8cb8 50a4 f2d4 6397 f868  .W8z....P...c..h
-00000cc0: 364f 8b18 c496 0cd4 2e2e 694d 9eeb 9a3b  6O........iM...;
-00000cd0: 51ee 9485 5412 4f10 7359 1cf1 b35b f800  Q...T.O.sY...[..
-00000ce0: fb16 5c71 8d33 bfc5 d1e5 15f4 e216 9a0e  ..\q.3..........
-00000cf0: cd3f 75c9 6e4e 2b1a ecc5 e77b 577e ab5d  .?u.nN+....{W~.]
-00000d00: 480c 54ac 331e 3df2 12fc b08f 2121 6cfa  H.T.3.=.....!!l.
-00000d10: e7de 2011 da3e acf9 1b81 8f00 beaf 10e9  .. ..>..........
-00000d20: 9cc4 f738 ffcc fc17 504b 0304 1400 0000  ...8....PK......
-00000d30: 0800 7d88 9858 32c0 66ed 4c01 0000 4d02  ..}..X2.f.L...M.
-00000d40: 0000 1800 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00000d50: 6574 732f 7368 6565 7434 2e78 6d6c 7552  ets/sheet4.xmluR
-00000d60: db4e c330 0cfd 952a 1f40 3a24 2e9a da4a  .N.0...*.@:$...J
-00000d70: 6c08 c103 d2b4 0978 4459 ebb6 d192 b824  l......xDY.....$
-00000d80: ee0a 7f8f d3ee c603 4fb1 4f7c 8e8f 9d64  ........O.O|...d
-00000d90: 03fa 5d68 0128 f9b6 c685 5cb4 44dd 5cca  ..]h.(....\.D.\.
-00000da0: 50b6 6055 b8c2 0e1c dfd4 e8ad 224e 7d23  P.`U........"N}#
-00000db0: 43e7 4155 23c9 1a79 9da6 b7d2 2aed 4491  C.AU#..y....*.D.
-00000dc0: 8dd8 ca17 19f6 64b4 8395 4f42 6fad f23f  ......d...OBo..?
-00000dd0: 0b30 38e4 6226 8ec0 5a37 2d8d 802c b24e  .08.b&..Z7-..,.N
-00000de0: 35b0 017a eb98 c0a9 3ce9 54da 820b 1a5d  5..z....<.T....]
-00000df0: e2a1 cec5 c36c be98 1863 c5bb 8621 5cc4  .....l...c...!\.
-00000e00: 491c 668b b88b c94b 958b 347a 0203 2545  I.f....K..4z..%E
-00000e10: 09c5 c71e 9660 4c54 6227 5f07 5171 6e1a  .....`LTb'_.Qqn.
-00000e20: 9997 f151 fe69 9c9f ed6d 5580 259a 0f5d  ...Q.i...mU.%..]
-00000e30: 519b 8b7b 9154 50ab ded0 1a87 6738 cc74  Q..{.TP.....g8.t
-00000e40: 73b6 f8a8 4815 99c7 21f1 71d8 222b 6310  s...H...!.q."+c.
-00000e50: 5b72 a176 7149 1bf2 8c6b ee44 45d9 d3e7  [r.vqI...k.DE...
-00000e60: c07b 4697 4962 1f11 95e5 81b5 f88f 857b  .{F.Ib.........{
-00000e70: f0ad 72cd 5f8e e4ae c751 261b 71cd afca  ..r._....Q&.q...
-00000e80: 37da 85c4 40cd 5ae9 d51d 9bf5 93ef 2921  7...@.Z.......)!
-00000e90: ecc6 67d9 2211 da31 6cf9 b9c1 c702 beaf  ..g."..1l.......
-00000ea0: 11e9 94c4 bd9d 7e50 f10b 504b 0304 1400  ......~P..PK....
-00000eb0: 0000 0800 7d88 9858 0840 26f8 5c01 0000  ....}..X.@&.\...
-00000ec0: 8b02 0000 1800 0000 786c 2f77 6f72 6b73  ........xl/works
-00000ed0: 6865 6574 732f 7368 6565 7435 2e78 6d6c  heets/sheet5.xml
-00000ee0: 7552 db4e c330 0cfd 952a 1f40 3624 2e42  uR.N.0...*.@6$.B
-00000ef0: 6d25 3684 e001 6902 018f 286b dd36 5a12  m%6...i...(k.6Z.
-00000f00: 17c7 a38c afc7 e96e 20c1 537c 3bf6 3976  .......n .S|;.9v
-00000f10: f201 6915 3b00 ce3e bd0b b150 1d73 7fa5  ..i.;..>...P.s..
-00000f20: 75ac 3af0 269e 600f 4132 0d92 372c 2eb5  u.:.&.`.A2..7,..
-00000f30: 3af6 04a6 1e41 dee9 d3c9 e45c 7b63 832a  :....A.....\{c.*
-00000f40: f331 b6a0 32c7 353b 1b60 4159 5c7b 6f68  .1..2.5;.`AY\{oh
-00000f50: 3303 8743 a1a6 6a1f 78b4 6dc7 6340 9779  3..C..j.x.m.c@.y
-00000f60: 6f5a 7802 7eee 0520 ae3e f4a9 ad87 102d  oZx.~.. .>.....-
-00000f70: 868c a029 d4f5 f46a be45 8c15 2f16 86f8  ...)...j.E../...
-00000f80: c3ce 9298 25e2 2a39 f775 a126 8913 38a8  ....%.*9.u.&..8.
-00000f90: 38b5 30f2 7cc0 1c9c 4b9d 84c9 fbae a93a  8.0.|...K......:
-00000fa0: 0e4d c89f f6be fded a85f e82d 4d84 39ba  .M......._.-M.9.
-00000fb0: 575b 7357 a84b 95d5 d098 b5e3 471c ee60  W[sW.K......G..`
-00000fc0: a7e9 ec48 f1c6 b029 73c2 21a3 24b6 ccab  ...H...)s.!.$...
-00000fd0: 64a4 9152 6843 5ad2 1393 c4ad 4ce2 9220  d..RhCZ.....L.. 
-00000fe0: 32d9 91ee 1b84 af8d 875c b3f0 4959 5ded  2........\..IY].
-00000ff0: d0b3 ffd0 d59a df06 b912 863f 50f3 ff50  ...........?P..P
-00001000: f801 d499 d0fe c668 e1bc 5fc4 5644 3ad2  .......h.._.VD:.
-00001010: 83a1 d686 9839 68a4 d7e4 e442 a4d2 56f5  .....9h....B..V.
-00001020: d661 ecc7 a32e 9119 fd68 76f2 5980 5281  .a.......hv.Y.R.
-00001030: e41b 443e 3869 eb87 ff57 7e03 504b 0304  ..D>8i...W~.PK..
-00001040: 1400 0000 0800 7d88 9858 c7cf 3958 6801  ......}..X..9Xh.
-00001050: 0000 0e03 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00001060: 6b73 6865 6574 732f 7368 6565 7436 2e78  ksheets/sheet6.x
-00001070: 6d6c 7553 db4e c330 0cfd 952a 1f40 0612  mluS.N.0...*.@..
-00001080: 174d 6d25 b631 c103 d2c4 043c a2ac 75d7  .Mm%.1.....<..u.
-00001090: 68b9 14c7 a5ec ef71 ba2b d2fa 54db f139  h......q.+..T..9
-000010a0: 3ebe 34ed 3c6e 420d 40c9 af35 2e64 a226  >.4.<nB.@..5.d.&
-000010b0: 6ac6 5286 a206 abc2 956f c0f1 4be5 d12a  j.R......o..K..*
-000010c0: 6217 d732 3408 aaec 41d6 c89b d1e8 4e5a  b..24...A.....NZ
-000010d0: a59d c8d3 3eb6 c03c f52d 19ed 6081 4968  ....>..<.-..`.Ih
-000010e0: ad55 b89d 80f1 5d26 aec5 21f0 a6d7 35f5  .U....]&..!...5.
-000010f0: 0199 a78d 5ac3 12e8 bd61 00bb f2c8 536a  ....Z....a....Sj
-00001100: 0b2e 68ef 1284 2a13 8fd7 e3f9 0ed1 677c  ..h...*.......g|
-00001110: 68e8 c299 9dc4 6656 de6f a2f3 5266 6214  h.....fV.o..Rfb.
-00001120: 3581 8182 2285 e2cf 0f4c c198 c8c4 4abe  5..."....L....J.
-00001130: f7a4 e254 3422 cfed 03fd bcef 9fe5 ad54  ...T4".........T
-00001140: 80a9 379f baa4 3a13 0f22 29a1 52ad a137  ..7...:..").R..7
-00001150: df3d c3be a7db 93c4 9922 95a7 e8bb 0463  .=.......".....c
-00001160: b379 5a44 2396 e444 ede2 9096 841c d75c  .yZD#..D.......\
-00001170: 89f2 3600 7e69 d7b4 944a 621d 312a 8b3d  ..6.~i...Jb.1*.=
-00001180: 6a32 842a 3416 ad51 7801 331d c20c 1599  j2.*4..Qx.3.....
-00001190: 0d01 78a5 9711 4f43 08da 3670 217f 3e28  ..x...OC..6p!.>(
-000011a0: a9fc 9f2d 796c 875d ece6 18ef e455 e15a  ...-yl.].....U.Z
-000011b0: bb90 18a8 9865 7475 cfd3 c6dd e077 0ef9  .....etu.....w..
-000011c0: a6bf ab95 27f2 b637 6bbe 57c0 98c0 ef95  ....'..7k.W.....
-000011d0: f774 74e2 e28f bf40 fe07 504b 0304 1400  .tt....@..PK....
-000011e0: 0000 0800 7d88 9858 4409 9006 e701 0000  ....}..XD.......
-000011f0: 3704 0000 1800 0000 786c 2f77 6f72 6b73  7.......xl/works
-00001200: 6865 6574 732f 7368 6565 7437 2e78 6d6c  heets/sheet7.xml
-00001210: 7554 4d6f a330 10fd 2bc8 e7aa 26d5 f643  uTMo.0..+...&..C
-00001220: 1120 3549 dbed a152 d56a db63 e5c0 0056  . 5I...R.j.c...V
-00001230: 8c4d ed61 69ff fd8e 4d42 132d 5cf0 cc78  .M.ai...MB.-\..x
-00001240: decc 1bfb 99a4 3776 e76a 008c be1a a55d  ......7v.j.....]
-00001250: ca6a c476 c9b9 cb6b 6884 3b37 2d68 da29  .j.v...kh.;7-h.)
-00001260: 8d6d 0492 6b2b ee5a 0ba2 08a0 46f1 8b38  .m..k+.Z....F..8
-00001270: bee2 8d90 9a65 4988 3ddb 2c31 1d2a a9e1  .....eI.=.,1.*..
-00001280: d946 ae6b 1a61 bf57 a04c 9fb2 053b 045e  .F.k.a.W.L...;.^
-00001290: 6455 6308 f02c 6945 05af 807f 5a02 90cb  dUc..,iE....Z...
-000012a0: c73a 856c 403b 6974 64a1 4cd9 ed62 f930  .:.l@;itd.L..b.0
-000012b0: 2042 c69b 84de 1dd9 911f 666b ccce 3b8f   B........fk..;.
-000012c0: 45ca 62cf 0914 e4e8 4b08 5afe c21a 94f2  E.b.....K.Z.....
-000012d0: 9588 c9e7 be28 fb69 ea91 c7f6 a1fc 7d98  .....(.i......}.
-000012e0: 9fe8 6d85 83b5 51ef b2c0 3a65 372c 2aa0  ..m...Q...:e7,*.
-000012f0: 149d c217 d3ff 86fd 4c97 3f14 3702 4596  ........L.?.7.E.
-00001300: 58d3 47d6 0f9b 25b9 377c 4b4a 94da 1fd2  X.G...%.7|KJ....
-00001310: 2b5a 8a4b ea84 9983 cf0e 740e 1fa5 54f4  +Z.K......t...T.
-00001320: 094d 138e c4c8 eff3 7c8f 5fcd e103 4c8b  .M......|._...L.
-00001330: 0626 40eb 3990 d405 7c7d 481d 9a4e 0037  .&@.9...|}H..N.7
-00001340: f3c0 b69b a277 3707 2059 4c23 eee7 10f8  .....w7. YL#....
-00001350: dd4e 517a 98a5 549c 6673 3afa c37d 0e77  .NQz..T.fs:..}.w
-00001360: 51d0 f74d 2849 2b89 c245 b9e9 340e 7773  Q..M(I+..E..4.ws
-00001370: ba35 eae3 6279 bb88 7fdd 5c5e 5f91 666a  .5..by....\^_.fj
-00001380: d36f ac69 37a6 d75e 5f21 f0e8 cfe1 099c  .o.i7..^_!......
-00001390: 2319 8fc1 3b6b 8d3d 0e0a 454f 60a5 84de  #...;k.=..EO`...
-000013a0: 05d9 fbc9 52a6 a443 eaec 6fba 5362 91b1  ....R..C..o.Sb..
-000013b0: 5238 1467 15e8 2d25 9e39 2d5a b281 257c  R8.g..-%.9-Z..%|
-000013c0: 4c49 f829 cfff 026e 7850 4fc2 5692 0654  LI.)...nxPO.V..T
-000013d0: 50d2 7cf1 f935 c9d2 0e0a 1d1c 346d 60b2  P.|..5......4m`.
-000013e0: 3588 a609 664d 0f1b ac4f a0fd d218 1c1d  5...fM...O......
-000013f0: ff42 c67f 45f6 0f50 4b03 0414 0000 0008  .B..E..PK.......
-00001400: 007d 8898 5891 c100 8bd2 0100 00f6 0300  .}..X...........
-00001410: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001420: 7473 2f73 6865 6574 382e 786d 6c8d 53db  ts/sheet8.xml.S.
-00001430: 6edb 300c fd15 43cf 43e5 14bd 21b0 0d34  n.0...C.C...!..4
-00001440: 4983 f5a1 40d1 62ed e3a0 d8b4 2d44 165d  I...@.b.....-D.]
-00001450: 899e 97bf 1f65 276e ba25 c05e 24de 0ec5  .....e'n.%.^$...
-00001460: 4352 498f 6eeb 6b00 8a7e 37c6 fa54 d444  CRI.n.k..~7..T.D
-00001470: ed5c 4a9f d7d0 287f 812d 58f6 94e8 1a45  .\J...(..-X....E
-00001480: acba 4afa d681 2a06 5063 e465 1cdf c846  ..J...*.Pc.e...F
-00001490: 692b b264 b03d bb2c c18e 8cb6 f0ec 22df  i+.d.=.,......".
-000014a0: 358d 72bb 0518 ec53 3113 07c3 8bae 6a1a  5.r....S1.....j.
-000014b0: 0c32 4b5a 55c1 2bd0 8f96 01ac ca29 4fa1  .2KZU.+......)O.
-000014c0: 1bb0 5ea3 8d1c 94a9 b89f cdd7 2362 8878  ..^.........#b.x
-000014d0: d3d0 fb23 390a 6436 88db a03c 16a9 8843  ...#9.d6...<...C
-000014e0: 4d60 20a7 9042 f1f5 0b96 604c c8c4 957c  M` ..B....`L...|
-000014f0: ec93 8acf 4703 f258 3ea4 5f0f fcb9 bc8d  ....G..X>._.....
-00001500: f2b0 44f3 ae0b aa53 7127 a202 4ad5 197a  ..D....Sq'..J..z
-00001510: c1fe 3bec 395d 7f96 b852 a4b2 c461 1fb9  ..;.9]...R...a..
-00001520: 4036 4bf2 2084 2739 50db d0a4 5772 6cd7  @6K. .'9P...Wrl.
-00001530: fc12 650e 5af4 9ad0 ed7e 5ad5 4022 898b  ..e.Z....~Z.@"..
-00001540: 092e 99ef a18b ff80 eae2 0470 790e a86d  ...........py..m
-00001550: dbd1 09c0 ea1c 8087 7b1a f170 0e41 bbf6  ........{..p.A..
-00001560: 1497 f5d9 92fe 2220 b981 87a9 8c1d 2df8  ......" ......-.
-00001570: 7c53 46f3 cda3 f551 8e9d a5b1 c35f 5dd3  |SF....Q....._].
-00001580: 942f e7f7 b3f8 eaee faf6 8627 5f63 bf72  ./.........'_c.r
-00001590: d8ae b0b7 614b 06c3 63e8 c313 78cf cb38  ....aK..c...x..8
-000015a0: 191f 9c43 776c 5486 1779 6194 dd0e cb1b  ...CwlT..ya.....
-000015b0: 98a5 c268 4ffc 72f8 249d 51b3 4ca8 a2a8  ...hO.r.$.Q.L...
-000015c0: c0c2 373e 361c 2a12 39f9 12f9 b5c0 7f0c  ..7>6.*.9.......
-000015d0: 7efc 0f4f ca55 9a99 1928 9958 7c71 cb5b  ~..O.U...(.X|q.[
-000015e0: e5c6 051b 15c2 7628 6183 44d8 0c62 cdff  ......v(a.D..b..
-000015f0: 125c 0860 7f89 4893 1216 7cfa ead9 1f50  .\.`..H...|....P
-00001600: 4b03 0414 0000 0008 007d 8898 581a 828f  K........}..X...
-00001610: 869c 0100 001a 0400 0018 0000 0078 6c2f  .............xl/
-00001620: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00001630: 392e 786d 6c7d 94db 4ee4 300c 865f a5ca  9.xml}..N.0.._..
-00001640: 0390 0109 58a1 b6d2 321c 1721 2110 bb97  ....X...2..!!...
-00001650: a34c ebb6 1149 5c12 97ee bcfd 3a9d 0368  .L...I\.....:..h
-00001660: d570 35b6 e3ef cfef ca99 7c44 ff16 3a00  .p5.......|D..:.
-00001670: cafe 5ae3 4221 3aa2 fe42 ca50 7560 5538  ..Z.B!:..B.Pu`U8
-00001680: c21e 1c9f 34e8 ad22 4e7d 2b43 ef41 d513  ....4.."N}+C.A..
-00001690: 648d 3c59 2cce a455 da89 329f 6a4f becc  d.<Y,..U..2.jO..
-000016a0: 7120 a31d 3cf9 2c0c d62a bfb9 0483 6321  q ..<.,..*....c!
-000016b0: 8ec5 bef0 acdb 8ea6 822c f35e b5f0 02f4  .........,.^....
-000016c0: da33 c0a9 3ce8 d4da 820b 1a5d e6a1 29c4  .3..<......]..).
-000016d0: cfe3 8b87 2d31 75fc d630 862f 7116 8759  ....-1u..0./q..Y
-000016e0: 23be c5e4 be2e c422 7a02 0315 4509 c53f  #......"z...E..?
-000016f0: 1fb0 0463 a212 3b79 df89 8acf 4b23 f935  ...c..;y....K#.5
-00001700: decb df4c f3b3 bdb5 0ab0 44f3 47d7 d415  ...L......D.G...
-00001710: e287 c86a 68d4 60e8 19c7 3bd8 cd74 fa69  ...jh.`...;..t.i
-00001720: f14a 912a 738f 63e6 e3b0 655e c520 5ec9  .J.*s.c...e^. ^.
-00001730: 8dda c58f f442 9eeb 9a6f a252 8500 766d  .....B...o.R..vm
-00001740: 362b 5555 10e2 e0b9 24f6 134f 65b5 a32f  6+UU....$..Oe../
-00001750: 5374 80f7 015c 05df d2cb 146d b01a c28a  St...\.....m....
-00001760: 543b 035d a5a0 161c ac74 3d83 5c27 5d92  T;.].....t=.\'].
-00001770: f234 03dc a400 7073 fab7 697d af66 89bb  .4....ps..i}.f..
-00001780: 14a1 5d3f cc39 ba4f 01bc def3 c4af 1441  ..]?.9.O.......A
-00001790: 9b1e 66fa 1f92 96fe 1b40 f20a edf7 72bb  ..f......@....r.
-000017a0: 53f1 cd3c 2adf 6a17 3203 0dab 2c8e ce79  S..<*.j.2...,..y
-000017b0: f3fc 7609 b709 613f bdb1 3512 a19d c28e  ..v...a?..5.....
-000017c0: df2e f8d8 c0e7 0d22 1d92 f808 0e7f 07e5  ......."........
-000017d0: 3f50 4b03 0414 0000 0008 007d 8898 5882  ?PK........}..X.
-000017e0: b2f4 9d67 0100 000f 0300 0019 0000 0078  ...g...........x
-000017f0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00001800: 6574 3130 2e78 6d6c 7553 db4e c330 0cfd  et10.xmluS.N.0..
-00001810: 952a 1f40 3624 2e9a da4a 6c63 8207 a469  .*.@6$...Jlc...i
-00001820: 13f0 88b2 d66d a3e5 46e2 51f6 f738 ed6e  .....m..F.Q..8.n
-00001830: 48eb 536d c7c7 3e3e 76d3 d6fa 6d68 0030  H.Sm..>>v...mh.0
-00001840: f9d5 ca84 8c35 886e c279 281a d022 dc58  .....5.n.y(..".X
-00001850: 0786 5e2a ebb5 4072 7dcd 83f3 20ca 0ea4  ..^*..@r}... ...
-00001860: 15bf 1d8d eeb9 16d2 b03c ed62 4b9f a776  .........<.bK..v
-00001870: 874a 1a58 fa24 ecb4 167e 3f05 65db 8c8d  .J.X.$...~?.e...
-00001880: d931 b092 7583 5d80 e7a9 1335 ac01 df1d  .1..u.]....5....
-00001890: 01c8 e5a7 3aa5 d460 82b4 26f1 5065 ec69  ....:..`..&.Pe.i
-000018a0: 3c59 f488 2ee3 4342 1b2e ec24 0eb3 b176  <Y....CB...$...v
-000018b0: 1b9d d732 63a3 c809 1414 184b 08fa fcc0  ...2c......K....
-000018c0: 0c94 8a95 88c9 f7a1 283b 378d c84b fb58  ........(;7..K.X
-000018d0: 7ed1 cd4f f436 22c0 ccaa 4f59 6293 b147  ~..O.6"...OYb..G
-000018e0: 9694 5089 9dc2 956d 5fe0 30d3 dd99 e25c  ..P....m_.0....\
-000018f0: a0c8 536f dbc4 c761 f3b4 8846 6c49 89d2  ..So...a...FlI..
-00001900: 4491 d6e8 292e a913 e60a 2afc 82b2 8694  D...).....*.....
-00001910: 23d1 8841 5e1c 40d3 2190 8f6d 8750 b321  #..A^.@.!..m.P.!
-00001920: 9434 6e87 5700 f321 00ed f43a e279 0881  .4n.W..!...:.y..
-00001930: 7b77 8dd2 6290 52f9 3f9b 936e c765 f442  {w..b.R.?..n.e.B
-00001940: c643 7913 be96 2624 512b 5af1 cd03 c9ed  .Cy...&$Q+Z.....
-00001950: 7be5 7b07 adeb 0e6b 6311 adee cc86 0e16  {.{....kc.......
-00001960: 7c4c a0f7 ca5a 3c39 71f3 a77f 20ff 0350  |L...Z<9q... ..P
-00001970: 4b03 0414 0000 0008 007d 8898 5882 b2f4  K........}..X...
-00001980: 9d67 0100 000f 0300 0019 0000 0078 6c2f  .g...........xl/
-00001990: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-000019a0: 3131 2e78 6d6c 7553 db4e c330 0cfd 952a  11.xmluS.N.0...*
-000019b0: 1f40 3624 2e9a da4a 6c63 8207 a469 13f0  .@6$...Jlc...i..
-000019c0: 88b2 d66d a3e5 46e2 51f6 f738 ed6e 48eb  ...m..F.Q..8.nH.
-000019d0: 536d c7c7 3e3e 76d3 d6fa 6d68 0030 f9d5  Sm..>>v...mh.0..
-000019e0: ca84 8c35 886e c279 281a d022 dc58 0786  ...5.n.y(..".X..
-000019f0: 5e2a ebb5 4072 7dcd 83f3 20ca 0ea4 15bf  ^*..@r}... .....
-00001a00: 1d8d eeb9 16d2 b03c ed62 4b9f a776 874a  .......<.bK..v.J
-00001a10: 1a58 fa24 ecb4 167e 3f05 65db 8c8d d931  .X.$...~?.e....1
-00001a20: b092 7583 5d80 e7a9 1335 ac01 df1d 01c8  ..u.]....5......
-00001a30: e5a7 3aa5 d460 82b4 26f1 5065 ec69 3c59  ..:..`..&.Pe.i<Y
-00001a40: f488 2ee3 4342 1b2e ec24 0eb3 b176 1b9d  ....CB...$...v..
-00001a50: d732 63a3 c809 1414 184b 08fa fcc0 0c94  .2c......K......
-00001a60: 8a95 88c9 f7a1 283b 378d c84b fb58 7ed1  ......(;7..K.X~.
-00001a70: cd4f f436 22c0 ccaa 4f59 6293 b147 9694  .O.6"...OYb..G..
-00001a80: 5089 9dc2 956d 5fe0 30d3 dd99 e25c a0c8  P....m_.0....\..
-00001a90: 536f dbc4 c761 f3b4 8846 6c49 89d2 4491  So...a...FlI..D.
-00001aa0: d6e8 292e a913 e60a 2afc 82b2 8694 23d1  ..).....*.....#.
-00001ab0: 8841 5e1c 40d3 2190 8f6d 8750 b321 9434  .A^.@.!..m.P.!.4
-00001ac0: 6e87 5700 f321 00ed f43a e279 0881 7b77  n.W..!...:.y..{w
-00001ad0: 8dd2 6290 52f9 3f9b 936e c765 f442 c643  ..b.R.?..n.e.B.C
-00001ae0: 7913 be96 2624 512b 5af1 cd03 c9ed 7be5  y...&$Q+Z.....{.
-00001af0: 7b07 adeb 0e6b 6311 adee cc86 0e16 7c4c  {....kc.......|L
-00001b00: a0f7 ca5a 3c39 71f3 a77f 20ff 0350 4b03  ...Z<9q... ..PK.
-00001b10: 0414 0000 0008 007d 8898 58fb c712 8d4a  .......}..X....J
-00001b20: 0100 0075 0200 0019 0000 0078 6c2f 776f  ...u.......xl/wo
-00001b30: 726b 7368 6565 7473 2f73 6865 6574 3132  rksheets/sheet12
-00001b40: 2e78 6d6c 7552 d94e c330 10fc 95c8 1f50  .xmluR.N.0.....P
-00001b50: a748 1caa 9248 3408 c103 52d5 0a78 7693  .H...H4...R..xv.
-00001b60: 4d62 d5f6 067b 4be0 ef59 273d 10a2 4fde  Mb...{K..Y'=..O.
-00001b70: 6b66 676c 6703 fa5d e800 28f9 b2c6 855c  kfglg..]..(....\
-00001b80: 7444 fd42 ca50 7560 5598 610f 8e3b 0d7a  tD.B.Pu`U.a..;.z
-00001b90: ab88 53df cad0 7b50 f508 b246 5ea5 e98d  ..S...{P...F^...
-00001ba0: b44a 3b51 6463 6de5 8b0c f764 b483 954f  .J;Qdcm....d...O
-00001bb0: c2de 5ae5 bf97 6070 c8c5 5c1c 0b6b dd76  ..Z...`p..\..k.v
-00001bc0: 3416 6491 f5aa 850d d06b cf00 4ee5 89a7  4.d......k..N...
-00001bd0: d616 5cd0 e812 0f4d 2eee e78b 7242 8c13  ..\....M....rB..
-00001be0: 6f1a 86f0 2b4e a299 2de2 2e26 cf75 2ed2  o...+N..-..&.u..
-00001bf0: a809 0c54 1429 141f 9f50 8231 9189 957c  ...T.)...P.1...|
-00001c00: 1c48 c579 6944 fe8e 8ff4 8fa3 7f96 b755  .H.yiD.........U
-00001c10: 014a 34ef baa6 2e17 7722 a9a1 517b 436b  .J4.....w"..Q{Ck
-00001c20: 1c9e e0e0 e9fa 2cf1 4191 2a32 8f43 e2a3  ......,.A.*2.C..
-00001c30: d922 ab62 1057 f2a0 76f1 9236 e4b9 ae79  .".b.W..v..6...y
-00001c40: 1315 8194 a74c 124b 8805 591d 00cb 4b00  .....L.K..Y...K.
-00001c50: 70f5 3fe3 e565 7eaf fe22 24ab 3b5a 9ee4  p.?..e~.."$.;Z..
-00001c60: c6e7 7851 bed5 2e24 061a 664a 67b7 6cca  ..xQ...$..fJg.l.
-00001c70: 4ffe a684 b01f 9f6f 8b44 68c7 b0e3 6f01  O......o.Dh...o.
-00001c80: 3e0e 70bf 41a4 5312 eff7 f4d3 8a1f 504b  >.p.A.S.......PK
-00001c90: 0304 1400 0000 0800 7d88 9858 2751 7b71  ........}..X'Q{q
-00001ca0: 5a01 0000 c902 0000 1900 0000 786c 2f77  Z...........xl/w
-00001cb0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00001cc0: 332e 786d 6c7d 52db 4ec3 300c fd95 2a1f  3.xml}R.N.0...*.
-00001cd0: b06c 485c 84da 4a6c 1382 07a4 6908 7844  .lH\..Jl....i.xD
-00001ce0: 59eb b6d1 92ba 241e 85bf c7ee ae0f 634f  Y.....$.......cO
-00001cf0: f1ed f8f8 d849 7b0c ebd8 0050 f2e3 5d1b  .....I{....P..].
-00001d00: 33d5 1075 f75a c7a2 016f e208 3b68 3953  3..u.Z...o..;h9S
-00001d10: 61f0 86d8 0db5 8e5d 0053 0e20 eff4 d578  a......].S. ...x
-00001d20: 7ca3 bdb1 adca d321 b608 798a 1b72 b685  |......!..y..r..
-00001d30: 4548 e2c6 7b13 7ea7 e0b0 cfd4 44ed 034b  EH..{.~.....D..K
-00001d40: 5b37 3404 749e 76a6 8657 a0b7 8e01 ecea  [74.t.v..W......
-00001d50: 439f d27a 68a3 c536 0950 65ea 6172 3fdf  C..zh..6.Pe.ar?.
-00001d60: 2286 8a77 0b7d 3cb1 1311 b342 5c8b f35c  "..w.}<....B\..\
-00001d70: 666a 2c33 8183 82a4 85e1 e71b 66e0 9c74  fj,3........f..t
-00001d80: e249 be76 4dd5 9154 90a7 f6be fde3 a09f  .I.vM..T........
-00001d90: c75b 9908 3374 1fb6 a426 5377 2a29 a132  .[..3t...&Sw*).2
-00001da0: 1b47 4bec 9f60 a7e9 fa38 e2dc 90c9 d380  .GK..`...8......
-00001db0: 7d12 446c 9e16 6208 2517 da56 96f4 4a81  }.Dl..b.%..V..J.
-00001dc0: e396 9928 7750 d167 154c cdb2 29d5 c4a3  ...(wP.g.L..)...
-00001dd0: 4842 173b e0f4 3f60 10ea 4bc8 d945 4a87  HB.;..?`..K..EJ.
-00001de0: 8591 1d9d 01ce 2f53 9e47 6a56 bc5f e376  ....../S.GjV._.v
-00001df0: 0572 e217 136a dbc6 4428 f938 a35b 5e54  .r...j..D(.8.[^T
-00001e00: d8ee 6ceb 1076 c397 5821 11fa c16c f8ab  ..l..v..X!...l..
-00001e10: 4190 02ce 5788 7470 e466 87df 9bff 0150  A...W.tp.f.....P
-00001e20: 4b03 0414 0000 0008 007d 8898 5844 ff81  K........}..XD..
-00001e30: 0869 0100 000c 0300 0019 0000 0078 6c2f  .i...........xl/
-00001e40: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00001e50: 3134 2e78 6d6c 7553 db6e 8330 0cfd 1594  14.xmluS.n.0....
-00001e60: 0f68 da49 bba8 02a4 b55d b53d 4caa 5a6d  .h.I.....].=L.Zm
-00001e70: 7b0e 604a d45c 5862 c6fa f773 a0b7 49f0  {.`J.\Xb...s..I.
-00001e80: 84ed f81c 1f5f 885b eb0e be02 c0e8 572b  ....._.[......W+
-00001e90: e313 5621 d673 ce7d 5e81 167e 626b 30f4  ..V!.s.}^..~bk0.
-00001ea0: 525a a705 92eb f6dc d70e 44d1 81b4 e277  RZ........D....w
-00001eb0: d3e9 03d7 421a 96c6 5d6c e3d2 d836 a8a4  ....B...]l...6..
-00001ec0: 818d 8b7c a3b5 70c7 0528 db26 6cc6 ce81  ...|..p..(.&l...
-00001ed0: addc 57d8 0578 1ad7 620f 3bc0 8f9a 00e4  ..W..x..b.;.....
-00001ee0: f20b 4f21 3518 2fad 891c 9409 7b9e cdd7  ..O!5./.....{...
-00001ef0: 3da2 cbf8 94d0 fa1b 3b0a cd64 d61e 82f3  =.......;..d....
-00001f00: 5624 6c1a 3481 821c 0385 a0cf 0f2c 41a9  V$l.4........,A.
-00001f10: c044 4abe 4fa4 ec5a 3420 6fed 33fd baeb  .DJ.O..Z4 o.3...
-00001f20: 9fe4 65c2 c3d2 aa2f 5960 95b0 2716 1550  ..e..../Y`..'..P
-00001f30: 8a46 e1d6 b6af 70ea e9fe 2a71 2550 a4b1  .F....p...*q%P..
-00001f40: b36d e442 b369 9c07 2394 a444 69c2 9076  .m.B.i..#..Di..v
-00001f50: e828 2ea9 12a6 b974 79a3 848b 3992 8a10  .(.....ty...9...
-00001f60: e3f9 09b3 18c3 08ef 4167 ea38 8059 8e61  ........Ag.8.Y.a
-00001f70: a4a9 1b1c 00ac c600 b4d0 61c4 cb18 028f  ..........a.....
-00001f80: 350c e4af 4725 15ff b339 0ded bc89 7e8a  5...G%...9....~.
-00001f90: e14a de85 db4b e323 0525 b14c 278f 346b  .J...K.#.%.L'.4k
-00001fa0: d78f bd77 d0d6 dd55 6516 d1ea ceac e85a  ...w...Ue......Z
-00001fb0: c185 047a 2fad c58b 13d6 7ef9 01d2 3f50  ...z/.....~...?P
-00001fc0: 4b03 0414 0000 0008 007d 8898 5811 26ee  K........}..X.&.
-00001fd0: aa80 0100 0080 0300 0019 0000 0078 6c2f  .............xl/
-00001fe0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00001ff0: 3135 2e78 6d6c 7593 594f c330 0c80 ff4a  15.xmlu.YO.0...J
-00002000: 951f 4006 1287 505b 898d 633c 2021 10f0  ..@...P[..c< !..
-00002010: 88b2 d65d 2372 e1b8 94fd 7b9c ee00 a4f6  ...]#r....{.....
-00002020: 29b6 e3cf 47ec e4bd c78f d802 50f6 6d8d  )...G.......P.m.
-00002030: 8b85 6889 c2a5 94b1 6ac1 aa78 e403 38be  ..h.....j..x..8.
-00002040: 693c 5a45 ace2 5ac6 80a0 ea01 b246 9ecc  i<ZE..Z......F..
-00002050: 6667 d22a ed44 990f b647 2c73 df91 d10e  fg.*.D...G,s....
-00002060: 1e31 8b9d b50a 3773 30be 2fc4 b1d8 1b9e  .1....7s0./.....
-00002070: f4ba a5c1 20cb 3ca8 353c 03bd 0406 5895  .... .<.5<....X.
-00002080: 8738 b5b6 e0a2 f62e 4368 0a71 757c b9dc  .8......Ch.qu|..
-00002090: 1283 c7ab 863e fe91 b3d4 ccca fb8f a4dc  .....>..........
-000020a0: d785 98a5 9ac0 4045 2984 e2e3 0b16 604c  ......@E).....`L
-000020b0: 8ac4 957c ee82 8adf a489 fc2b efc3 df0e  ...|.......+....
-000020c0: fd73 792b 1561 e1cd 9bae a92d c485 c86a  .sy+.a.....-...j
-000020d0: 6854 67e8 c9f7 4bd8 f574 fa5b e2b5 2255  hTg...K..t.[.."U
-000020e0: e6e8 fb0c 53b3 655e 2521 a564 47ed d223  ....S.e^%!.dG..#
-000020f0: 3d13 b25d 7326 2af9 997b 85f5 7b40 6e1c  =..]s&*..{..{@n.
-00002100: 7349 5c4b ba91 d58e 9c4f 9108 5f80 11a6  sI\K.....O.._...
-00002110: c9c5 1459 69ac 3aa3 c698 eb29 46c5 0876  ...Yi.:....)F..v
-00002120: 6536 23cc cd14 a35d e868 04b8 9d02 7889  e6#....].h....x.
-00002130: c689 bb29 8236 0146 fc97 9325 d5ff bd25  ...).6.F...%...%
-00002140: 0f6a 3ffd ede4 d266 3e28 5c6b 1733 030d  .j?....f>(\k.3..
-00002150: 4799 1d9d f37c 713b eaad 423e 0c9b bcf2  G....|q;..B>....
-00002160: 44de 0e62 cb3f 0430 39f0 7de3 3d1d 94b4  D..b.?.09.}.=...
-00002170: 6a87 4f57 fe00 504b 0304 1400 0000 0800  j.OW..PK........
-00002180: 7d88 9858 44ff 8108 6901 0000 0c03 0000  }..XD...i.......
-00002190: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-000021a0: 732f 7368 6565 7431 362e 786d 6c75 53db  s/sheet16.xmluS.
-000021b0: 6e83 300c fd15 940f 68da 49bb a802 a4b5  n.0.....h.I.....
-000021c0: 5db5 3d4c aa5a 6d7b 0e60 4ad4 5c58 62c6  ].=L.Zm{.`J.\Xb.
-000021d0: faf7 73a0 b749 f084 edf8 1c1f 5f88 5beb  ..s..I......_.[.
-000021e0: 0ebe 02c0 e857 2be3 1356 21d6 73ce 7d5e  .....W+..V!.s.}^
-000021f0: 8116 7e62 6b30 f452 5aa7 0592 ebf6 dcd7  ..~bk0.RZ.......
-00002200: 0e44 d181 b4e2 77d3 e903 d742 1a96 c65d  .D....w....B...]
-00002210: 6ce3 d2d8 36a8 a481 8d8b 7ca3 b570 c705  l...6.....|..p..
-00002220: 28db 266c c6ce 81ad dc57 d805 781a d762  (.&l.....W..x..b
-00002230: 0f3b c08f 9a00 e4f2 0b4f 2135 182f ad89  .;.......O!5./..
-00002240: 1c94 097b 9ecd d73d a2cb f894 d0fa 1b3b  ...{...=.......;
-00002250: 0acd 64d6 1e82 f356 246c 1a34 8182 1c03  ..d....V$l.4....
-00002260: 85a0 cf0f 2c41 a9c0 444a be4f a4ec 5a34  ....,A..DJ.O..Z4
-00002270: 206f ed33 fdba eb9f e465 c2c3 d2aa 2f59   o.3.....e..../Y
-00002280: 6095 b027 1615 508a 46e1 d6b6 af70 eae9  `..'..P.F....p..
-00002290: fe2a 7125 50a4 b1b3 6de4 42b3 699c 0723  .*q%P...m.B.i..#
-000022a0: 94a4 4469 c290 76e8 282e a912 a6b9 7479  ..Di..v.(.....ty
-000022b0: a384 8b39 928a 10e3 f909 b318 c308 ef41  ...9...........A
-000022c0: 67ea 3880 598e 61a4 a91b 1c00 acc6 00b4  g.8.Y.a.........
-000022d0: d061 c4cb 1802 8f35 0ce4 af47 2515 ffb3  .a.....5...G%...
-000022e0: 390d edbc 897e 8ae1 4ade 85db 4be3 2305  9....~..J...K.#.
-000022f0: 25b1 4c27 8f34 6bd7 8fbd 77d0 d6dd 5565  %.L'.4k...w...Ue
-00002300: 16d1 eace ace8 5ac1 8504 7a2f adc5 8b13  ......Z...z/....
-00002310: d67e f901 d23f 504b 0304 1400 0000 0800  .~...?PK........
-00002320: 7d88 9858 44ff 8108 6901 0000 0c03 0000  }..XD...i.......
-00002330: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00002340: 732f 7368 6565 7431 372e 786d 6c75 53db  s/sheet17.xmluS.
-00002350: 6e83 300c fd15 940f 68da 49bb a802 a4b5  n.0.....h.I.....
-00002360: 5db5 3d4c aa5a 6d7b 0e60 4ad4 5c58 62c6  ].=L.Zm{.`J.\Xb.
-00002370: faf7 73a0 b749 f084 edf8 1c1f 5f88 5beb  ..s..I......_.[.
-00002380: 0ebe 02c0 e857 2be3 1356 21d6 73ce 7d5e  .....W+..V!.s.}^
-00002390: 8116 7e62 6b30 f452 5aa7 0592 ebf6 dcd7  ..~bk0.RZ.......
-000023a0: 0e44 d181 b4e2 77d3 e903 d742 1a96 c65d  .D....w....B...]
-000023b0: 6ce3 d2d8 36a8 a481 8d8b 7ca3 b570 c705  l...6.....|..p..
-000023c0: 28db 266c c6ce 81ad dc57 d805 781a d762  (.&l.....W..x..b
-000023d0: 0f3b c08f 9a00 e4f2 0b4f 2135 182f ad89  .;.......O!5./..
-000023e0: 1c94 097b 9ecd d73d a2cb f894 d0fa 1b3b  ...{...=.......;
-000023f0: 0acd 64d6 1e82 f356 246c 1a34 8182 1c03  ..d....V$l.4....
-00002400: 85a0 cf0f 2c41 a9c0 444a be4f a4ec 5a34  ....,A..DJ.O..Z4
-00002410: 206f ed33 fdba eb9f e465 c2c3 d2aa 2f59   o.3.....e..../Y
-00002420: 6095 b027 1615 508a 46e1 d6b6 af70 eae9  `..'..P.F....p..
-00002430: fe2a 7125 50a4 b1b3 6de4 42b3 699c 0723  .*q%P...m.B.i..#
-00002440: 94a4 4469 c290 76e8 282e a912 a6b9 7479  ..Di..v.(.....ty
-00002450: a384 8b39 928a 10e3 f909 b318 c308 ef41  ...9...........A
-00002460: 67ea 3880 598e 61a4 a91b 1c00 acc6 00b4  g.8.Y.a.........
-00002470: d061 c4cb 1802 8f35 0ce4 af47 2515 ffb3  .a.....5...G%...
-00002480: 390d edbc 897e 8ae1 4ade 85db 4be3 2305  9....~..J...K.#.
-00002490: 25b1 4c27 8f34 6bd7 8fbd 77d0 d6dd 5565  %.L'.4k...w...Ue
-000024a0: 16d1 eace ace8 5ac1 8504 7a2f adc5 8b13  ......Z...z/....
-000024b0: d67e f901 d23f 504b 0304 1400 0000 0800  .~...?PK........
-000024c0: 7d88 9858 44ff 8108 6901 0000 0c03 0000  }..XD...i.......
-000024d0: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-000024e0: 732f 7368 6565 7431 382e 786d 6c75 53db  s/sheet18.xmluS.
-000024f0: 6e83 300c fd15 940f 68da 49bb a802 a4b5  n.0.....h.I.....
-00002500: 5db5 3d4c aa5a 6d7b 0e60 4ad4 5c58 62c6  ].=L.Zm{.`J.\Xb.
-00002510: faf7 73a0 b749 f084 edf8 1c1f 5f88 5beb  ..s..I......_.[.
-00002520: 0ebe 02c0 e857 2be3 1356 21d6 73ce 7d5e  .....W+..V!.s.}^
-00002530: 8116 7e62 6b30 f452 5aa7 0592 ebf6 dcd7  ..~bk0.RZ.......
-00002540: 0e44 d181 b4e2 77d3 e903 d742 1a96 c65d  .D....w....B...]
-00002550: 6ce3 d2d8 36a8 a481 8d8b 7ca3 b570 c705  l...6.....|..p..
-00002560: 28db 266c c6ce 81ad dc57 d805 781a d762  (.&l.....W..x..b
-00002570: 0f3b c08f 9a00 e4f2 0b4f 2135 182f ad89  .;.......O!5./..
-00002580: 1c94 097b 9ecd d73d a2cb f894 d0fa 1b3b  ...{...=.......;
-00002590: 0acd 64d6 1e82 f356 246c 1a34 8182 1c03  ..d....V$l.4....
-000025a0: 85a0 cf0f 2c41 a9c0 444a be4f a4ec 5a34  ....,A..DJ.O..Z4
-000025b0: 206f ed33 fdba eb9f e465 c2c3 d2aa 2f59   o.3.....e..../Y
-000025c0: 6095 b027 1615 508a 46e1 d6b6 af70 eae9  `..'..P.F....p..
-000025d0: fe2a 7125 50a4 b1b3 6de4 42b3 699c 0723  .*q%P...m.B.i..#
-000025e0: 94a4 4469 c290 76e8 282e a912 a6b9 7479  ..Di..v.(.....ty
-000025f0: a384 8b39 928a 10e3 f909 b318 c308 ef41  ...9...........A
-00002600: 67ea 3880 598e 61a4 a91b 1c00 acc6 00b4  g.8.Y.a.........
-00002610: d061 c4cb 1802 8f35 0ce4 af47 2515 ffb3  .a.....5...G%...
-00002620: 390d edbc 897e 8ae1 4ade 85db 4be3 2305  9....~..J...K.#.
-00002630: 25b1 4c27 8f34 6bd7 8fbd 77d0 d6dd 5565  %.L'.4k...w...Ue
-00002640: 16d1 eace ace8 5ac1 8504 7a2f adc5 8b13  ......Z...z/....
-00002650: d67e f901 d23f 504b 0304 1400 0000 0800  .~...?PK........
-00002660: 7d88 9858 19ef 2f38 7b01 0000 4b03 0000  }..X../8{...K...
-00002670: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00002680: 732f 7368 6565 7431 392e 786d 6c75 93db  s/sheet19.xmlu..
-00002690: 4ec3 300c 865f a5ca 0390 81c4 41a8 adc4  N.0.._......A...
-000026a0: 364e 1748 6808 b844 59eb ae11 3914 c7a5  6N.Hh..DY...9...
-000026b0: 8ca7 c7e9 8e48 ed55 6dc7 9ff3 3b76 d3ce  .....H.Um...;v..
-000026c0: e367 a801 28f9 b1c6 854c d444 cdb5 94a1  .g..(....L.D....
-000026d0: a8c1 aa70 e21b 707c 5279 b48a d8c5 950c  ...p..p|Ry......
-000026e0: 0d82 2a7b c81a 7936 995c 48ab b413 79da  ..*{..y6.\H...y.
-000026f0: c79e 314f 7d4b 463b 78c6 24b4 d62a 5c4f  ..1O}KF;x.$..*\O
-00002700: c1f8 2e13 a762 1758 e855 4d7d 40e6 69a3  .....b.X.UM}@.i.
-00002710: 56f0 02f4 da30 c0ae dcd7 29b5 0517 b477  V....0....)....w
-00002720: 0942 9589 9bd3 ebfb 0dd1 67bc 69e8 c291  .B........g.i...
-00002730: 9dc4 6696 de7f 46e7 b1cc c424 6a02 0305  ..f...F....$j...
-00002740: c512 8a3f df30 0363 6225 56f2 b52d 2a0e  ...?.0.cb%V..-*.
-00002750: 9746 f2d8 de95 bfeb fb67 794b 1560 e6cd  .F.......gyK.`..
-00002760: bb2e a9ce c495 484a a854 6b68 e1bb 07d8  ......HJ.Tkh....
-00002770: f674 7e90 3857 a4f2 147d 9760 6c36 4f8b  .t~.8W...}.`l6O.
-00002780: 68c4 2b39 51bb f848 2f84 1cd7 7c13 e508  h.+9Q..H/...|...
-00002790: 8150 f772 3fc0 fdae 2d84 5412 0b8a c7b2  .P.r?...-.T.....
-000027a0: d8e2 d331 bcd0 58b4 46e1 0033 1b63 5408  ...1..X.F..3.cT.
-000027b0: 6097 663d c0cc c718 ed9a 9606 80db 3180  `.f=..........1.
-000027c0: f761 98b8 1b23 68dd c040 fefd a8a4 f27f  .a...#h..@......
-000027d0: b6e4 37df 0d72 3384 b864 4f0a 57da 85c4  ..7..r3..dO.W...
-000027e0: 40c5 5526 2797 3c2a dc4c 6de3 906f faa5  @.U&'.<*.Lm..o..
-000027f0: 5c7a 226f 7bb3 e665 078c 097c 5e79 4f7b  \z"o{..e...|^yO{
-00002800: 276e cdfe ffc9 ff00 504b 0304 1400 0000  'n......PK......
-00002810: 0800 7d88 9858 8b06 3c20 8201 0000 5703  ..}..X..< ....W.
-00002820: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-00002830: 6574 732f 7368 6565 7432 302e 786d 6c75  ets/sheet20.xmlu
-00002840: 53db 6edb 300c fd15 431f 50a5 1bba 0d85  S.n.0...C.P.....
-00002850: 6d60 4d2f dbc3 80a2 c5b6 c740 b169 5b88  m`M/.......@.i[.
-00002860: 246a 145d af7f 3fca b9b4 03e2 2793 14cf  $j.]..?.....'...
-00002870: e1e1 c5e5 84b4 4b03 0017 7fbd 0ba9 5203  ......K.......R.
-00002880: 73bc d63a 3503 7893 2e30 4290 970e c91b  s..:5.x..0B.....
-00002890: 1697 7a9d 2281 6967 9077 fac3 6af5 497b  ..z.".ig.w..j.I{
-000028a0: 6383 aacb 39f6 4875 8923 3b1b e091 8a34  c...9.Hu.#;....4
-000028b0: 7a6f e8f5 061c 4e95 ba54 c7c0 93ed 079e  zo....N..T......
-000028c0: 03ba 2ea3 e9e1 19f8 6714 80b8 fac4 d35a  ........g......Z
-000028d0: 0f21 590c 0541 57a9 af97 d70f 7bc4 9cf1  .!Y..AW.....{...
-000028e0: cbc2 94de d945 6e66 8bb8 cbce f7b6 52ab  .....Enf......R.
-000028f0: ac09 1c34 9c29 8c7c 5e60 0dce 6526 51f2  ...4.).|^`..e&Q.
-00002900: e740 aade 8a66 e47b fb48 7f3f f72f f2b6  .@...f.{.H.?./..
-00002910: 26c1 1add 6fdb f250 a92f aa68 a133 a3e3  &...o..P./.h.3..
-00002920: 279c bec1 a1a7 ab37 89b7 864d 5d12 4e05  '......7...M].N.
-00002930: e566 ebb2 c946 2e29 8936 e421 3d33 49dc  .f...F.).6.!=3I.
-00002940: 4a25 ae65 cc93 a176 83ce f658 6a16 29f9  J%.e...v...Xj.).
-00002950: 4137 07e0 cd12 90e0 0528 c122 70bd 0444  A7.......(."p..D
-00002960: c10d 26f4 9b86 6cb3 db7c 8c24 233f 4370  ..&...l..|.$#?Cp
-00002970: bb44 6043 1cf9 0ce0 6eb1 e2c8 e711 f74b  .D`C....n......K
-00002980: 087e 8de7 243d 2c4a 6aff cfd6 32ff e352  .~..$=,Jj...2..R
-00002990: f70b c907 f7c3 506f 432a 1c74 c2b2 baf8  ......PoC*.t....
-000029a0: 2c6b a3fd 06f7 0e63 9c0f 748b cce8 6773  ,k.....c..t...gs
-000029b0: 90c3 07ca 09f2 de21 f2c9 c917 74fa 97ea  .......!....t...
-000029c0: 7f50 4b03 0414 0000 0008 007d 8898 58a5  .PK........}..X.
-000029d0: 0c76 4f53 0100 00a4 0200 0019 0000 0078  .vOS...........x
-000029e0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-000029f0: 6574 3231 2e78 6d6c 7552 db6a c330 0cfd  et21.xmluR.j.0..
-00002a00: 95e0 0fa8 d3c1 2e94 24b0 b68c ed61 505a  ........$....aPZ
-00002a10: b63d bb89 9298 fa36 5b59 d6bf 9f9c f436  .=.....6[Y.....6
-00002a20: 689f 2cc9 3a47 e7c8 ce7a eb77 a105 c0e4  h.,.:G...z.w....
-00002a30: 572b 1372 d622 ba19 e7a1 6c41 8b30 b10e  W+.r."....lA.0..
-00002a40: 0cdd d4d6 6b81 94fa 8607 e741 5403 482b  ....k......AT.H+
-00002a50: 7e97 a60f 5c0b 6958 910d b595 2f32 dba1  ~...\.iX..../2..
-00002a60: 9206 563e 099d d6c2 efe7 a06c 9fb3 293b  ..V>.......l..);
-00002a70: 16d6 b269 7128 f022 73a2 810d e087 2300  ...iq(."s.....#.
-00002a80: a5fc c453 490d 2648 6b12 0f75 ce9e a7b3  ...SI.&Hk..u....
-00002a90: e588 183a 3e25 f4e1 224e a299 adb5 bb98  ...:>%.."N......
-00002aa0: bc55 394b a326 5050 62a4 1074 fcc0 0294  .U9K.&PPb..t....
-00002ab0: 8a4c a4e4 fb40 cace 4323 f232 3ed2 bf0c  .L...@..C#.2>...
-00002ac0: fe49 de56 0458 58f5 252b 6c73 f6c4 920a  .I.V.XX.%+ls....
-00002ad0: 6ad1 295c dbfe 150e 9eee cf12 9702 4591  j.)\..........E.
-00002ae0: 79db 273e 9a2d b232 0671 2435 4a13 97b4  y.'>.-.2.q$5J...
-00002af0: 414f 7549 93b0 90c6 7598 7124 09b1 c0cb  AOuI....u.q$....
-00002b00: 0360 7e0b 408b be8e 58dc 42e0 dec1 95fe  .`~.@...X.B.....
-00002b10: e54d 49d5 ff6e 4e66 8e1b 1add c5d7 7b17  .MI..nNf......{.
-00002b20: be91 2624 0a6a 6249 278f b403 3fae 634c  ..&$.jbI'...?.cL
-00002b30: d0ba e1b5 b716 d1ea 216c e917 818f 0d74  ........!l.....t
-00002b40: 5f5b 8ba7 243e c7e9 6316 7f50 4b03 0414  _[..$>..c..PK...
-00002b50: 0000 0008 007d 8898 5865 1756 075c 0100  .....}..Xe.V.\..
-00002b60: 00b5 0200 0019 0000 0078 6c2f 776f 726b  .........xl/work
-00002b70: 7368 6565 7473 2f73 6865 6574 3232 2e78  sheets/sheet22.x
-00002b80: 6d6c 7552 db4e c330 0cfd 952a 1fb0 6c48  mluR.N.0...*..lH
-00002b90: 5c84 da4a b009 c103 d204 029e b3d6 5d23  \..J..........]#
-00002ba0: 92b8 735c 0a7f 8fd3 5d91 d853 6c27 e7d8  ..s\....]..Sl'..
-00002bb0: e738 f980 f419 5b00 cebe bd0b b150 2d73  .8....[......P-s
-00002bc0: 77ab 75ac 5af0 264e b083 2037 0d92 372c  w.u.Z.&N.. 7..7,
-00002bd0: 29ad 75ec 084c 3d82 bcd3 17d3 e995 f6c6  ).u..L=.........
-00002be0: 0655 e663 6d49 658e 3d3b 1b60 4959 ecbd  .U.cmIe.=;.`IY..
-00002bf0: 37f4 730f 0e87 42cd d4be f062 d72d 8f05  7.s...B....b.-..
-00002c00: 5de6 9d59 c32b f05b 2700 49f5 81a7 b61e  ]..Y.+.['.I.....
-00002c10: 42b4 1832 82a6 5077 b3db c516 31be 78b7  B..2..Pw....1.x.
-00002c20: 30c4 9338 4b62 5688 9f29 79aa 0b35 4d33  0..8KbV..)y..5M3
-00002c30: 8183 8a13 8591 e30b e6e0 5c62 9249 363b  ..........\b.I6;
-00002c40: 5275 6c9a 90a7 f19e fe61 d42f e3ad 4c84  Rul......a./..L.
-00002c50: 39ba 0f5b 735b a81b 95d5 d098 def1 0b0e  9..[s[..........
-00002c60: 8fb0 d374 791c 7161 d894 39e1 9051 125b  ...ty.qa..9..Q.[
-00002c70: e655 0a52 4b79 6843 32e9 9549 ea56 3a71  .U.RKyhC2..I.V:q
-00002c80: 1961 d343 a820 e69a 658c 54d4 d50e 747f  .a.C. ..e.T...t.
-00002c90: 1684 3dfd 0f99 9f83 7424 c6d2 7f90 c539  ..=.....t$.....9
-00002ca0: 480d b122 db25 27ff c2b4 a8db 5bb6 959b  H..".%'.....[...
-00002cb0: d6f9 6c68 6d43 cc1c 3442 379d 5c8b 29b4  ..lhmC..4B7.\.).
-00002cc0: f567 9b30 76e3 fa57 c88c 7e0c 5bf9 5640  .g.0v..W..~.[.V@
-00002cd0: e981 dc37 887c 48d2 7e0e 3fb5 fc05 504b  ...7.|H.~.?...PK
-00002ce0: 0304 1400 0000 0800 7d88 9858 d205 f146  ........}..X...F
-00002cf0: 5202 0000 470a 0000 0d00 0000 786c 2f73  R...G.......xl/s
-00002d00: 7479 6c65 732e 786d 6cdd 56db 8adb 3010  tyles.xml.V...0.
-00002d10: fd15 e30f a893 989a b824 79a8 2150 68cb  .........$y.!Ph.
-00002d20: c2ee 435f e558 4e04 bab8 b2bc 24fd fa6a  ..C_.XN.....$..j
-00002d30: 24e7 b69b e352 fa56 9be0 9939 3a33 67a4  $....R.V...9:3g.
-00002d40: 31ce aa77 27c9 9f0f 9cbb e4a8 a4ee d7e9  1..w'...........
-00002d50: c1b9 ee53 96f5 bb03 57ac ff60 3aae 3dd2  ...S....W..`:.=.
-00002d60: 1aab 98f3 aedd 677d 6739 6b7a 2229 992d  ......g}g9kz").-
-00002d70: 66b3 2253 4ce8 74b3 d283 da2a d727 3b33  f."SL.t....*.';3
-00002d80: 68b7 4e67 6992 6d56 add1 d7d0 3c8d 01bf  h.Ngi.mV....<...
-00002d90: 9629 9ebc 32b9 4e2b 2645 6d45 5ccc 9490  .)..2.N+&EmE\...
-00002da0: a718 5f84 c8ce 4863 13e7 d570 a253 a8ff  .._...Hc...p.S..
-00002db0: 1517 cc47 97a4 8eb9 94d0 c686 6816 cb84  ...G........h...
-00002dc0: 47ef 130b 292f 2a16 690c 6c56 1d73 8e5b  G...)/*.i.lV.s.[
-00002dd0: bdf5 4e24 85e8 7b6c b45f 4e9d 57b1 b7ec  ..N$..{l._N.W...
-00002de0: 345f 7c4c 6f18 e1e1 cbd4 c636 dcde b51b  4_|Lo......6....
-00002df0: 439b 95e4 ad23 8615 fb43 309c e9e8 511b  C....#...C0...Q.
-00002e00: e78c 22ab 116c 6f34 8b4a ceb4 d1f0 b977  .."..lo4.J.....w
-00002e10: 5cca 673a af1f ed5d 8163 9bc4 8dff d284  \.g:...].c......
-00002e20: 3da7 8ecf a657 359a 31cd e850 81db 7431  =....W5.1..P..t1
-00002e30: f9bf e7ed c4ab 719f 07df 900e fecf c138  ......q........8
-00002e40: fe64 792b 8ec1 3fb6 6f04 5c6a 0725 77e5  .dy+..?.o.\j.%w.
-00002e50: 2fd1 8446 659d 7ea7 1194 3739 ea41 4827  /..Fe.~...79.AH'
-00002e60: f4e8 1d44 d370 fdbe 3b9f dfb1 da0f f95d  ...D.p..;......]
-00002e70: 01bf aae1 2d1b a47b b980 ebf4 6a7f e38d  ....-..{....j...
-00002e80: 1854 7959 f544 8d8d abae f657 3aca 7971  .TyY.D.....W:.yq
-00002e90: 9d53 5f4c e886 1f79 538d aedd d7c1 4cbc  .S_L...yS.....L.
-00002ea0: e1cb 8e57 60bc 85b6 e102 1064 4510 4004  ...W`......dE.@.
-00002eb0: c25a 5006 6445 1eac f53f f6b5 c47d 4510  .ZP.dE...?...}E.
-00002ec0: 2a5c 3e86 9698 b5c4 acc8 7b08 55e1 86b5  *\>.......{.U...
-00002ed0: 00ab f417 68b9 2cf3 bc28 e0f6 56d5 6319  ....h.,..(..V.c.
-00002ee0: 15dc c3a2 a01f 4808 1512 07d6 a26a 7fbb  ......H......j..
-00002ef0: f313 0330 3136 7f98 0d78 ca93 6303 5b9e  ...016...x..c.[.
-00002f00: 1851 d8f2 c4ce 1304 f690 3865 0906 00d6  .Q........8e....
-00002f10: 220e 3c14 3851 2402 d4a2 5103 ac3c a773  ".<.8Q$...Q..<.s
-00002f20: 860a e16b 3e01 9525 8468 48c1 f416 05da  ...k>..%.hH.....
-00002f30: a882 6e70 5ef0 25ca f3b2 0410 8140 469e  ..np^.%......@F.
-00002f40: 4388 5ed8 0908 ca20 2110 caf3 f821 7df3  C.^.... !....!}.
-00002f50: 3dcb cedf b9ec fad7 71f3 1b50 4b03 0414  =.......q..PK...
-00002f60: 0000 0008 007d 8898 58b7 47eb 8ac0 0000  .....}..X.G.....
-00002f70: 0016 0200 000b 0000 005f 7265 6c73 2f2e  ........._rels/.
-00002f80: 7265 6c73 9d92 4b6e 0231 0c40 af12 655f  rels..Kn.1.@..e_
-00002f90: 4ca9 c402 31ac d8b0 4388 0bb8 89e7 a399  L...1...C.......
-00002fa0: c491 63c4 f4f6 8dd8 c020 6811 4bff 9e9e  ..c...... h.K...
-00002fb0: 2daf 0f34 a076 1c73 dba5 6cc6 30c4 5cd9  -..4.v.s..l.0.\.
-00002fc0: 5635 ad00 b26b 2960 9e71 a258 2a35 4b40  V5...k)`.q.X*5K@
-00002fd0: 2da1 3490 d0f5 d810 2ce6 f325 c82d c36e  -.4.....,..%.-.n
-00002fe0: d6b7 4c73 fc49 f40a 91eb ba73 b465 770a  ..Ls.I.....s.ew.
-00002ff0: 14f5 01f8 aec3 9a23 4a43 5ad9 7180 334b  .......#JCZ.q.3K
-00003000: ffcd dccf 0ad4 9a9d afac ecfc a735 f0a6  .............5..
-00003010: ccf3 f520 90a2 4745 702c f491 a44c 8b76  ... ..GEp,...L.v
-00003020: 94af 3e9e ddbe a4f3 a563 62b4 78df e8ff  ..>......cb.x...
-00003030: f3d0 a814 3df9 bf9d 30a5 89d2 d745 0926  ....=...0....E.&
-00003040: 6fb0 f905 504b 0304 1400 0000 0800 7d88  o...PK........}.
-00003050: 9858 10a8 bdb2 7a02 0000 7e08 0000 0f00  .X....z...~.....
-00003060: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
-00003070: 6c8d 956f 6fda 3010 c6bf 0aca 0758 08a5  l..oo.0......X..
-00003080: f48f 4aa5 8a76 d0a9 5b11 b0be 77e2 239c  ..J..v..[...w.#.
-00003090: 6afb 32db 691b 3efd ec44 b4e9 4cad bd21  j.2.i.>..D..L..!
-000030a0: f86c ff72 673f 4fee ea95 f473 4ef4 3c78  .l.rg?O....sN.<x
-000030b0: 9342 994b 3d4d 76d6 5697 696a 8a1d 4866  .B.K=Mv.V.ij..Hf
-000030c0: be51 05ca cd6d 494b 66dd 5097 296d b758  .Q...mIKf.P.)m.X
-000030d0: c02d 15b5 0465 d3d1 7038 4935 0866 9194  .-...e..p8I5.f..
-000030e0: d961 6592 8ef6 3f2c 5369 60dc ec00 ac14  .ae...?,Si`.....
-000030f0: 1d4a 3254 c9f5 d521 b3a5 1ea4 fd11 5928  .J2T...!......Y(
-00003100: fc9b 7cd4 479e 105e cdc7 023f 1cbc a0c1  ..|.G..^...?....
-00003110: 1c05 da66 9ab4 ff05 2403 890a 25ee 814f  ...f....$...%..O
-00003120: 9361 3230 3b7a 5d90 c63d 29cb c4ba d024  .a20;z]..=)....$
-00003130: c434 c9ba 8927 d016 8b20 bcf6 696e 586e  .4...'... ..inXn
-00003140: da88 65f9 cad7 3c4d 2643 07dc a236 b65d  ..e...<M&C...6.]
-00003150: d1f2 994b f205 dce2 6e54 5bfa 8ec2 82be  ...K....nT[.....
-00003160: 6516 e69a ea0a 55d9 625c 1969 af8e f628  e.....U.b\.i...(
-00003170: 0ecf 8162 12a6 c92f f7cb 373b b7c3 e7e1  ...b.../..7;....
-00003180: e2f7 bccb c93a 58af 427d 896e 42df f30e  .....:X.B}.nB...
-00003190: db47 6ce0 cdba 0460 0d7f 6a50 05f4 40a3  .Gl....`..jP..@.
-000031a0: 0868 1480 961a 25e8 def6 93c8 f693 60fb  .h....%.......`.
-000031b0: e1fd b3da f618 e308 631c 3056 60ac c656  ........c.0V`..V
-000031c0: 04c7 71a7 11dc 6980 fbc9 54cd 8468 364d  ..q...i...T..h6M
-000031d0: 057c 4db5 fe74 3a93 086b 12b0 7e57 8218  .|M..t:..k..~W..
-000031e0: 07de 1ef5 bfa8 b308 eaec 4895 1519 b4a4  ..........H.....
-000031f0: 9bfb 30ab f308 ea3c 40cd 4191 8419 91e6  ..0....<@.A.....
-00003200: a8dc 2e13 f02e 22bc 8bd8 2506 a46c 18d3  ......"...%..l..
-00003210: e530 7699 776a df48 b8c5 d285 fcdd 06e8  .0v.wj.H........
-00003220: a8e4 43cd af51 561f 8a7f a0a2 fd42 f581  ..C..QV......B..
-00003230: 31e9 67a1 f66f 8c01 998b e607 e127 4ccc  1.g..o.......'L.
-00003240: 0259 e881 0326 2c30 e683 2c34 c272 b60a  .Y...&,0..,4.r..
-00003250: 1931 f167 a1fa 1fb0 64c7 4f3b a6fc 2c94  .1.g....d.O;..,.
-00003260: fe82 2409 2aa9 362b 2848 e65e 6947 b931  ..$.*.6+(H.^iG.1
-00003270: 1b64 a10f e698 1b52 5f9f 59cc 0a59 e885  .d.....R_.Y..Y..
-00003280: 9ede 6e14 ffba fa98 23b2 d012 8f02 4b5a  ..n.....#.....KZ
-00003290: 34b9 468e fbe3 c851 cc19 a3d0 194b 12ce  4.F....Q.....K..
-000032a0: 0e9a 19b8 7bb3 a0cc 5166 cc12 a3d0 1233  ....{...Qf.....3
-000032b0: 41ca b591 b5d5 6e4f d9f4 49d1 36d0 7921  A.....nO..I.6.y!
-000032c0: 3d34 270e 5b54 c07d 5f32 7ec2 b5ca c2f5  =4'.[T.}_2~.....
-000032d0: 69ff e87c 353e f567 b4ad 8598 b9d8 a37a  i..|5>.g.......z
-000032e0: 705f c5f7 6e77 68d5 d77f 0150 4b03 0414  p_..nwh....PK...
-000032f0: 0000 0008 007d 8898 5800 5845 5b2c 0100  .....}..X.XE[,..
-00003300: 0011 0e00 001a 0000 0078 6c2f 5f72 656c  .........xl/_rel
-00003310: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-00003320: 656c 73cd d741 8e82 3014 c6f1 ab90 1ec0  els..A..0.......
-00003330: f2aa a24e c495 1bb7 132f d0e0 1388 4049  ...N...../....@I
-00003340: dbc9 e8ed 87c8 023f 328b d998 792b d212  .......?2...y+..
-00003350: 1eff a4c9 2fb0 ffe4 c6c6 da75 a1aa fb90  ..../......u....
-00003360: dcdb a60b b9aa 62ec 3fb4 0e45 c5ad 0d0b  ......b.?..E....
-00003370: d773 37dc b93a dfda 382c 7da9 7b5b dc6c  .s7..:..8,}.{[.l
-00003380: c9da a469 a6fd eb0c 75d8 bfce 4cce 8f9e  ...i....u...L...
-00003390: ff32 d15d af75 c147 577c b5dc c55f 06eb  .2.].u.GW|..._..
-000033a0: 6fe7 6fa1 628e 2a39 5b5f 72cc 95be 37d3  o.o.b.*9[_r...7.
-000033b0: 76d0 cf0b 2d86 c92a 395d 72e5 4f17 5289  v...-..*9]r.O.R.
-000033c0: feef 2203 4546 40d1 128a 9602 8a56 50b4  ..".EF@......VP.
-000033d0: 1250 b486 a2b5 80a2 0c8a 3201 451b 28da  .P........2.E.(.
-000033e0: 0828 da42 d156 40d1 0e8a 7602 8a28 4522  .(.B.V@...v..(E"
-000033f0: 5309 4d33 b625 b84d 0837 4990 9b90 6e92  S.M3.%.M.7I...n.
-00003400: 6037 21de 2441 6f42 be49 82df 8480 9304  `7!.$AoB.I......
-00003410: c109 0927 0986 1322 4e12 1427 649c 2438  ...'..."N..'d.$8
-00003420: 6ed0 7123 c171 838e 1b09 8e9b d907 f85b  n.q#.q.........[
-00003430: 1d0f f1d1 7098 82c6 3506 bc15 ed38 3ccb  ....p...5....8<.
-00003440: d3fb 9fcb 7173 7634 23d3 1afe 000f 3f50  ....qsv4#.....?P
-00003450: 4b03 0414 0000 0008 007d 8898 589b b2a7  K........}..X...
-00003460: be69 0100 0021 0f00 0013 0000 005b 436f  .i...!.......[Co
-00003470: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00003480: cd97 cb6e c230 1045 7f25 ca16 11e3 b4a5  ...n.0.E.%......
-00003490: 0f01 9bb6 db96 457f c04d 2624 c22f 790c  ......E..M&$./y.
-000034a0: 85bf ef24 14a4 5694 87a8 d4d9 c44a 3c73  ...$..V......J<s
-000034b0: efb1 47ba 5246 6f6b 0f98 ac8c b638 4eeb  ..G.RFok.....8N.
-000034c0: 18fd 8310 58d4 6014 66ce 83a5 9dca 05a3  ....X.`.f.......
-000034d0: 22bd 8699 f0aa 98ab 1988 7c30 188a c2d9  ".........|0....
-000034e0: 0836 f663 ab91 4e46 4f50 a985 8ec9 f38a  .6.c..NFOP......
-000034f0: 3e63 e3ec 380d a031 4d1e 3785 add7 3855  >c..8..1M.7...8U
-00003500: deeb a650 91f6 c5d2 963f 5cfa 5f0e 1975  ...P.....?\._..u
-00003510: 7635 5837 1e7b 5490 2662 af45 b7f5 abc3  v5X7.{T.&b.E....
-00003520: b6f1 7509 2134 2524 5315 e28b 3254 2656  ..u.!4%$S...2T&V
-00003530: 5a60 5c6b c0ec b0c6 1e4a 5755 4d01 a52b  Z`\k.....JWUM..+
-00003540: 1686 5a32 f401 5489 3540 343a db88 f68e  ..Z2..T.5@4:....
-00003550: 5847 ba64 d83c e5c5 009d cc41 472a 9d06  XG.d.<.....AG*..
-00003560: e791 a616 e07c bfed 58da eebe 2721 08b1  .....|..X...'!..
-00003570: 3972 c89d 2569 5f7c 4268 275e 4279 aa39  9r..%i_|Bh'^By.9
-00003580: ddf0 870b f36e 2628 bae5 f26b fe3e e79d  .....n&(...k.>..
-00003590: feb9 2039 1790 2b2e 20d7 5c40 6eb8 800c  .. 9..+. .\@n...
-000035a0: b980 dc72 01b9 e302 72cf 0544 0ed8 90b0  ...r....r..D....
-000035b0: c956 c926 5c25 9b74 956c e255 b2c9 57c9  .V.&\%.t.l.U..W.
-000035c0: 2660 259b 8495 6c22 56b2 c9d8 9c4d c6e6  &`%...l"V....M..
-000035d0: 6c32 36ff d78c 7d77 6efe d77f 6ced 9a19  l26...}wn...l...
-000035e0: d5d8 1d80 e8fe 8c27 9f50 4b01 0214 0314  .......'.PK.....
-000035f0: 0000 0008 007d 8898 5846 5ac1 0c82 0000  .....}..XFZ.....
-00003600: 00b1 0000 0010 0000 0000 0000 0000 0000  ................
-00003610: 0080 0100 0000 0064 6f63 5072 6f70 732f  .......docProps/
-00003620: 6170 702e 786d 6c50 4b01 0214 0314 0000  app.xmlPK.......
-00003630: 0008 007d 8898 5892 2b0a b7eb 0000 00cb  ...}..X.+.......
-00003640: 0100 0011 0000 0000 0000 0000 0000 0080  ................
-00003650: 01b0 0000 0064 6f63 5072 6f70 732f 636f  .....docProps/co
-00003660: 7265 2e78 6d6c 504b 0102 1403 1400 0000  re.xmlPK........
-00003670: 0800 7d88 9858 995c 9c23 1006 0000 9c27  ..}..X.\.#.....'
-00003680: 0000 1300 0000 0000 0000 0000 0000 8001  ................
-00003690: ca01 0000 786c 2f74 6865 6d65 2f74 6865  ....xl/theme/the
-000036a0: 6d65 312e 786d 6c50 4b01 0214 0314 0000  me1.xmlPK.......
-000036b0: 0008 007d 8898 58bb e88b 3838 0100 0011  ...}..X...88....
-000036c0: 0200 0018 0000 0000 0000 0000 0000 0080  ................
-000036d0: 810b 0800 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000036e0: 7473 2f73 6865 6574 312e 786d 6c50 4b01  ts/sheet1.xmlPK.
-000036f0: 0214 0314 0000 0008 007d 8898 5833 636f  .........}..X3co
-00003700: 7aed 0100 0021 0400 0018 0000 0000 0000  z....!..........
-00003710: 0000 0000 0080 8179 0900 0078 6c2f 776f  .......y...xl/wo
-00003720: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
-00003730: 786d 6c50 4b01 0214 0314 0000 0008 007d  xmlPK..........}
-00003740: 8898 58a4 976e 8956 0100 00a5 0200 0018  ..X..n.V........
-00003750: 0000 0000 0000 0000 0000 0080 819c 0b00  ................
-00003760: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003770: 6865 6574 332e 786d 6c50 4b01 0214 0314  heet3.xmlPK.....
-00003780: 0000 0008 007d 8898 5832 c066 ed4c 0100  .....}..X2.f.L..
-00003790: 004d 0200 0018 0000 0000 0000 0000 0000  .M..............
-000037a0: 0080 8128 0d00 0078 6c2f 776f 726b 7368  ...(...xl/worksh
-000037b0: 6565 7473 2f73 6865 6574 342e 786d 6c50  eets/sheet4.xmlP
-000037c0: 4b01 0214 0314 0000 0008 007d 8898 5808  K..........}..X.
-000037d0: 4026 f85c 0100 008b 0200 0018 0000 0000  @&.\............
-000037e0: 0000 0000 0000 0080 81aa 0e00 0078 6c2f  .............xl/
-000037f0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00003800: 352e 786d 6c50 4b01 0214 0314 0000 0008  5.xmlPK.........
-00003810: 007d 8898 58c7 cf39 5868 0100 000e 0300  .}..X..9Xh......
-00003820: 0018 0000 0000 0000 0000 0000 0080 813c  ...............<
-00003830: 1000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00003840: 2f73 6865 6574 362e 786d 6c50 4b01 0214  /sheet6.xmlPK...
-00003850: 0314 0000 0008 007d 8898 5844 0990 06e7  .......}..XD....
-00003860: 0100 0037 0400 0018 0000 0000 0000 0000  ...7............
-00003870: 0000 0080 81da 1100 0078 6c2f 776f 726b  .........xl/work
-00003880: 7368 6565 7473 2f73 6865 6574 372e 786d  sheets/sheet7.xm
-00003890: 6c50 4b01 0214 0314 0000 0008 007d 8898  lPK..........}..
-000038a0: 5891 c100 8bd2 0100 00f6 0300 0018 0000  X...............
-000038b0: 0000 0000 0000 0000 0080 81f7 1300 0078  ...............x
-000038c0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-000038d0: 6574 382e 786d 6c50 4b01 0214 0314 0000  et8.xmlPK.......
-000038e0: 0008 007d 8898 581a 828f 869c 0100 001a  ...}..X.........
-000038f0: 0400 0018 0000 0000 0000 0000 0000 0080  ................
-00003900: 81ff 1500 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00003910: 7473 2f73 6865 6574 392e 786d 6c50 4b01  ts/sheet9.xmlPK.
-00003920: 0214 0314 0000 0008 007d 8898 5882 b2f4  .........}..X...
-00003930: 9d67 0100 000f 0300 0019 0000 0000 0000  .g..............
-00003940: 0000 0000 0080 81d1 1700 0078 6c2f 776f  ...........xl/wo
-00003950: 726b 7368 6565 7473 2f73 6865 6574 3130  rksheets/sheet10
-00003960: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00003970: 7d88 9858 82b2 f49d 6701 0000 0f03 0000  }..X....g.......
-00003980: 1900 0000 0000 0000 0000 0000 8081 6f19  ..............o.
-00003990: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000039a0: 7368 6565 7431 312e 786d 6c50 4b01 0214  sheet11.xmlPK...
-000039b0: 0314 0000 0008 007d 8898 58fb c712 8d4a  .......}..X....J
-000039c0: 0100 0075 0200 0019 0000 0000 0000 0000  ...u............
-000039d0: 0000 0080 810d 1b00 0078 6c2f 776f 726b  .........xl/work
-000039e0: 7368 6565 7473 2f73 6865 6574 3132 2e78  sheets/sheet12.x
-000039f0: 6d6c 504b 0102 1403 1400 0000 0800 7d88  mlPK..........}.
-00003a00: 9858 2751 7b71 5a01 0000 c902 0000 1900  .X'Q{qZ.........
-00003a10: 0000 0000 0000 0000 0000 8081 8e1c 0000  ................
-00003a20: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00003a30: 6565 7431 332e 786d 6c50 4b01 0214 0314  eet13.xmlPK.....
-00003a40: 0000 0008 007d 8898 5844 ff81 0869 0100  .....}..XD...i..
-00003a50: 000c 0300 0019 0000 0000 0000 0000 0000  ................
-00003a60: 0080 811f 1e00 0078 6c2f 776f 726b 7368  .......xl/worksh
-00003a70: 6565 7473 2f73 6865 6574 3134 2e78 6d6c  eets/sheet14.xml
-00003a80: 504b 0102 1403 1400 0000 0800 7d88 9858  PK..........}..X
-00003a90: 1126 eeaa 8001 0000 8003 0000 1900 0000  .&..............
-00003aa0: 0000 0000 0000 0000 8081 bf1f 0000 786c  ..............xl
-00003ab0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00003ac0: 7431 352e 786d 6c50 4b01 0214 0314 0000  t15.xmlPK.......
-00003ad0: 0008 007d 8898 5844 ff81 0869 0100 000c  ...}..XD...i....
-00003ae0: 0300 0019 0000 0000 0000 0000 0000 0080  ................
-00003af0: 8176 2100 0078 6c2f 776f 726b 7368 6565  .v!..xl/workshee
-00003b00: 7473 2f73 6865 6574 3136 2e78 6d6c 504b  ts/sheet16.xmlPK
-00003b10: 0102 1403 1400 0000 0800 7d88 9858 44ff  ..........}..XD.
-00003b20: 8108 6901 0000 0c03 0000 1900 0000 0000  ..i.............
-00003b30: 0000 0000 0000 8081 1623 0000 786c 2f77  .........#..xl/w
-00003b40: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00003b50: 372e 786d 6c50 4b01 0214 0314 0000 0008  7.xmlPK.........
-00003b60: 007d 8898 5844 ff81 0869 0100 000c 0300  .}..XD...i......
-00003b70: 0019 0000 0000 0000 0000 0000 0080 81b6  ................
-00003b80: 2400 0078 6c2f 776f 726b 7368 6565 7473  $..xl/worksheets
-00003b90: 2f73 6865 6574 3138 2e78 6d6c 504b 0102  /sheet18.xmlPK..
-00003ba0: 1403 1400 0000 0800 7d88 9858 19ef 2f38  ........}..X../8
-00003bb0: 7b01 0000 4b03 0000 1900 0000 0000 0000  {...K...........
-00003bc0: 0000 0000 8081 5626 0000 786c 2f77 6f72  ......V&..xl/wor
-00003bd0: 6b73 6865 6574 732f 7368 6565 7431 392e  ksheets/sheet19.
-00003be0: 786d 6c50 4b01 0214 0314 0000 0008 007d  xmlPK..........}
-00003bf0: 8898 588b 063c 2082 0100 0057 0300 0019  ..X..< ....W....
-00003c00: 0000 0000 0000 0000 0000 0080 8108 2800  ..............(.
-00003c10: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00003c20: 6865 6574 3230 2e78 6d6c 504b 0102 1403  heet20.xmlPK....
-00003c30: 1400 0000 0800 7d88 9858 a50c 764f 5301  ......}..X..vOS.
-00003c40: 0000 a402 0000 1900 0000 0000 0000 0000  ................
-00003c50: 0000 8081 c129 0000 786c 2f77 6f72 6b73  .....)..xl/works
-00003c60: 6865 6574 732f 7368 6565 7432 312e 786d  heets/sheet21.xm
-00003c70: 6c50 4b01 0214 0314 0000 0008 007d 8898  lPK..........}..
-00003c80: 5865 1756 075c 0100 00b5 0200 0019 0000  Xe.V.\..........
-00003c90: 0000 0000 0000 0000 0080 814b 2b00 0078  ...........K+..x
-00003ca0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00003cb0: 6574 3232 2e78 6d6c 504b 0102 1403 1400  et22.xmlPK......
-00003cc0: 0000 0800 7d88 9858 d205 f146 5202 0000  ....}..X...FR...
-00003cd0: 470a 0000 0d00 0000 0000 0000 0000 0000  G...............
-00003ce0: 8001 de2c 0000 786c 2f73 7479 6c65 732e  ...,..xl/styles.
-00003cf0: 786d 6c50 4b01 0214 0314 0000 0008 007d  xmlPK..........}
-00003d00: 8898 58b7 47eb 8ac0 0000 0016 0200 000b  ..X.G...........
-00003d10: 0000 0000 0000 0000 0000 0080 015b 2f00  .............[/.
-00003d20: 005f 7265 6c73 2f2e 7265 6c73 504b 0102  ._rels/.relsPK..
-00003d30: 1403 1400 0000 0800 7d88 9858 10a8 bdb2  ........}..X....
-00003d40: 7a02 0000 7e08 0000 0f00 0000 0000 0000  z...~...........
-00003d50: 0000 0000 8001 4430 0000 786c 2f77 6f72  ......D0..xl/wor
-00003d60: 6b62 6f6f 6b2e 786d 6c50 4b01 0214 0314  kbook.xmlPK.....
-00003d70: 0000 0008 007d 8898 5800 5845 5b2c 0100  .....}..X.XE[,..
-00003d80: 0011 0e00 001a 0000 0000 0000 0000 0000  ................
-00003d90: 0080 01eb 3200 0078 6c2f 5f72 656c 732f  ....2..xl/_rels/
-00003da0: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00003db0: 7350 4b01 0214 0314 0000 0008 007d 8898  sPK..........}..
-00003dc0: 589b b2a7 be69 0100 0021 0f00 0013 0000  X....i...!......
-00003dd0: 0000 0000 0000 0000 0080 014f 3400 005b  ...........O4..[
-00003de0: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
-00003df0: 6d6c 504b 0506 0000 0000 1e00 1e00 0908  mlPK............
-00003e00: 0000 e935 0000 0000                      ...5....
+000000b0: 504b 0304 1400 0000 0800 d050 a858 150f  PK.........P.X..
+000000c0: 74b6 ee00 0000 cb01 0000 1100 0000 646f  t.............do
+000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
+000000e0: 914d 4fc3 300c 86ff ca94 7beb b41d 1344  .MO.0.....{....D
+000000f0: 5d2f a09d 4042 6212 885b 9478 5b44 f3a1  ]/..@Bb..[.x[D..
+00000100: c4a8 ddbf a72d 5b37 0417 8ef1 fbf8 b1ad  .....-[7........
+00000110: d42a 08e5 233e 471f 3092 c1b4 e86d eb92  .*..#>G.0....m..
+00000120: 5061 cd0e 4441 0024 7540 2b53 3e10 6e08  Pa..DA.$u@+S>.n.
+00000130: 773e 5a49 c333 ee21 48f5 21f7 0825 e72b  w>ZI.3.!H.!..%.+
+00000140: b048 524b 9230 0ab3 301b d949 a9d5 ac0c  .HRK.0..0..I....
+00000150: 9fb1 9d04 5a01 b668 d151 8222 2fe0 c212  ....Z..h.Q."/...
+00000160: 469b fe6c 9892 99ec 9399 a9ae ebf2 ae9a  F..l............
+00000170: b861 a302 de9e 1e5f a6e5 33e3 1249 a790  .a....._..3..I..
+00000180: 35b5 5642 4594 e463 335e 148e 7d5b c355  5.VBE..c3^..}[.U
+00000190: b13e cdfe 2ea0 5e0c 1304 1d03 aed9 3979  .>....^.......9y
+000001a0: adee 1fb6 1bd6 94bc 5c66 fc26 e3b7 5b7e  ........\f.&..[~
+000001b0: 27f8 4a54 c5fb e8fa d17f 115a afcd cefc  '.JT.......Z....
+000001c0: d358 5d19 cf82 a686 5fff d67c 0150 4b03  .X]....._..|.PK.
+000001d0: 0414 0000 0008 00d0 50a8 5899 5c9c 2310  ........P.X.\.#.
+000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
+000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
+00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
+00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
+00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
+00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
+00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
+00000250: b72f dee0 5732 2411 4130 19a7 aff0 c00a  ./..W2$.A0......
+00000260: a54c 5eb5 5a69 00c3 387d c913 12c3 dc82  .L^.Zi..8}......
+00000270: 8b08 4b78 14cb d65c e05b 1a2f 23d6 eab4  ..Kx...\.[./#...
+00000280: dbdd 5684 696c a118 4764 607d 5e2c 6840  ..V.il..Gd`}^,h@
+00000290: d054 515a 6f5f 20b4 e51f 33f8 15cb 548d  .TQZo_ ...3...T.
+000002a0: 65a3 0113 5741 26b9 88b4 f2f9 6cc5 fcda  e...WA&.....l...
+000002b0: de3e 65cf e93a 1d32 816e 301b 5820 7fce  .>e..:.2.n0.X ..
+000002c0: 6fa7 e44e 5a88 e154 c2c4 c06a 673f 566b  o..NZ..T...jg?Vk
+000002d0: c7d1 d248 8082 c97d 9405 ba49 f6a3 d315  ...H...}...I....
+000002e0: 0832 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca  .2.;:.X.v|......
+000002f0: da74 346d 1ae0 e3f1 7838 b6cb d28b 701c  .t4m....x8....p.
+00000300: 04e0 51bb 9ec2 9df4 6cbf a441 09b4 a369  ..Q.....l..A...i
+00000310: d064 d8f6 daae 91a6 aa8d 534f d3f7 7ddf  .d........SO..}.
+00000320: eb9b 689c 0a8d 5b4f d36b 77dd d38e 89c6  ..h...[O.kw.....
+00000330: add0 780d bef1 4f87 c3ae 89c6 abd0 74eb  ..x...O.......t.
+00000340: 6926 27fd ae6b a4e9 1668 4246 e3eb 7a12  i&'..k...hBF..z.
+00000350: 15b5 e540 d320 0058 7076 d6cc d203 965e  ...@. .Xpv.....^
+00000360: 29fa 7594 1ad9 1dbb dd41 5cf0 58ee 3989  ).u......A\.X.9.
+00000370: 11fe c6c5 04d6 69d2 1996 3446 729d 9005  ......i...4Fr...
+00000380: 0e00 37c4 d14c 507c af41 b68a e0c2 92d2  ..7..LP|.A......
+00000390: 5c90 d6cf 29b5 501a 089a c881 f547 8221  \...).P......G.!
+000003a0: c5dc affd f597 bbc9 a433 7a9d 7d3a ce6b  .........3z.}:.k
+000003b0: 947f 69ab 01a7 edbb 9bcf 93fc 73e8 e49f  ..i.........s...
+000003c0: a793 d74d 42ce 70bc 2c09 f1fb 235b 6187  ...MB.p.,...#[a.
+000003d0: 276e 3b13 723a 1c67 427c cff6 f691 a525  'n;.r:.gB|.....%
+000003e0: 32cf eff9 0aeb 4e3c 671f 5696 b05d cfcf  2.....N<g.V..]..
+000003f0: e49e 8c72 23bb ddf6 587d f64f 476e 23d7  ...r#...X}.OGn#.
+00000400: a9c0 b322 d794 4624 459f c82d bae4 1138  ..."..F$E..-...8
+00000410: b549 0d32 133f 089d 8698 6a50 1c02 a409  .I.2.?....jP....
+00000420: 3196 a186 f8b4 c6ac 11e0 137d b7be 08c8  1..........}....
+00000430: df8d 88f7 ab6f 9a3d 57a1 5849 da84 f810  .....o.=W.XI....
+00000440: 461a e29c 73e6 73d1 6cfb 07a5 46d1 f655  F...s.s.l...F..U
+00000450: bcdc a397 5815 0197 18df 34aa 352c c5d6  ....X.....4.5,..
+00000460: 7895 c0f1 ad9c 3c1d 1312 cd94 0b06 4186  x.....<.......A.
+00000470: 9724 2612 a939 7e4d 4813 fe2b a5da fe9c  .$&..9~MH..+....
+00000480: d340 f094 2f24 fa4a 918f 69b3 23a7 7426  .@../$.J..i.#.t&
+00000490: cde8 331a c146 af1b 7587 68d2 3c7a fe05  ..3..F..u.h.<z..
+000004a0: f99c 350a 1c91 1b1d 0267 1bb3 4621 8469  ..5......g..F!.i
+000004b0: bbf0 1eaf 248e 9aad c211 2b42 3e62 1936  ....$.....+B>b.6
+000004c0: 1a72 b516 81b6 71a9 8460 5a12 c6d1 784e  .r....q..`Z...xN
+000004d0: d2b4 11fc 59ac 3593 3e60 c8ec cd91 75ce  ....Y.5.>`....u.
+000004e0: d691 0e11 925e 3742 3e62 ce8b 9011 bf1e  .....^7B>b......
+000004f0: 8638 4a9a eda2 7158 04fd 9e5e c349 c1e8  .8J...qX...^.I..
+00000500: 82cb 66fd b87e 86d5 336c 2c8e f747 d417  ..f..~..3l,..G..
+00000510: 4ae4 0f26 a73f e932 3407 a39a 5909 bd84  J..&.?.24...Y...
+00000520: 566a 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e  Vj...4>..2.....>
+00000530: e57a 780a 3796 c6bc 50ae 827b 01ff d1da  .zx.7...P..{....
+00000540: 37c2 abf8 82c0 397f 2e7d cfa5 efb9 f43d  7.....9..}.....=
+00000550: a1d2 b737 237d 67c1 d38b 5bde 466e 5bc4  ...7#}g...[.Fn[.
+00000560: fbae 31da d734 2e28 6357 72cd c8c7 54af  ..1..4.(cWr...T.
+00000570: 9329 d839 9fc0 ecfd 683e 9ef1 edfa d924  .).9....h>.....$
+00000580: 84af 9a59 2d23 1690 4b81 b341 24b8 fc8b  ...Y-#..K..A$...
+00000590: caf0 2ac4 09e8 645b 2509 cb54 d365 378a  ..*...d[%..T.e7.
+000005a0: 129e 421b 6ee9 53f5 4a95 d7e5 afb9 28b8  ..B.n.S.J.....(.
+000005b0: 3c5b e4e9 afa1 743e 2ccf f93c 5fe7 b4cd  <[....t>,..<_...
+000005c0: 0b33 43b7 724b eab6 94be b526 384a f4b1  .3C.rK.....&8J..
+000005d0: cc70 4e1e cb0c 3b67 3c92 1db6 77a0 1d35  .pN...;g<...w..5
+000005e0: fbf6 5d76 e423 a530 5397 43b8 1a42 be03  ..]v.#.0S.C..B..
+000005f0: 6dba 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3  m...:8......R.o.
+00000600: f9e9 c578 1ae2 39d9 04b9 7d98 576d e7d8  ...x..9...}.Wm..
+00000610: d1d1 fbe7 c151 b0a3 ef3c 961d c788 f2a2  .....Q...<......
+00000620: 21ee a186 98cf c343 8779 7b5f 9867 95c6  !......C.y{_.g..
+00000630: 5034 146d 6cac 242c 46b7 60b8 d7f1 2c14  P4.ml.$,F.`...,.
+00000640: e064 602d a007 83af 5102 f252 5560 315b  .d`-....Q..RU`1[
+00000650: c603 2b90 a27c 4c8c 45e8 70e7 975c 5fe3  ..+..|L.E.p..\_.
+00000660: d192 e3db a665 b56e af29 7719 6d22 5239  .....e.n.)w.m"R9
+00000670: c269 9813 67ab cade 65b1 c155 1dcf 555b  .i..g...e..U..U[
+00000680: f2b0 be6a 3db4 154e cffe 59ad c89f 0c11  ...j=..N..Y.....
+00000690: 4e16 0b12 4863 9417 a64a a2f3 1953 bee7  N...Hc...J...S..
+000006a0: 2b49 c455 38bf 4533 b612 9718 bce3 e6c7  +I.U8.E3........
+000006b0: 714e 53b8 1276 b60f 0232 b9bb 39a9 7a65  qNS..v...2..9.ze
+000006c0: 3167 a6f2 df2d 0c09 2c5b 8859 12e2 4d5d  1g...-..,[.Y..M]
+000006d0: edd5 e79b 9cae 7a22 76fa 9777 c160 f2fd  ......z"v..w.`..
+000006e0: 70c9 470f e53b e75f f45d 43ae 7ef6 dde3  p.G..;._.]C.~...
+000006f0: fa6e 933b 484c 9c79 c511 0174 4502 2395  .n.;HL.y...tE.#.
+00000700: 1c06 1617 32e4 50ee 9290 0613 01cd 94c9  ....2.P.........
+00000710: 44f0 0282 64a6 1c80 98fa 0bbd f20c b929  D...d..........)
+00000720: 15ce ad3e 397f 452c 8386 4e5e d225 1214  ...>9.E,..N^.%..
+00000730: 8ab0 0c05 2117 72e3 efef 936a 778c d7fa  ....!.r....jw...
+00000740: 2c81 6d84 5432 64d5 17ca 4389 c13d 3372  ,.m.T2d...C..=3r
+00000750: 43d8 5425 f3ae da26 0b85 dbe2 54cd bb1a  C.T%...&....T...
+00000760: be26 604b c37a 6e9d 2d27 ffdb 5ed4 3db4  .&`K.zn.-'..^.=.
+00000770: 173d 46f3 a399 e01e b387 739b 7ab8 c245  .=F.......s.z..E
+00000780: acff 58d6 1ef9 32df 3970 db3a de03 5ee6  ..X...2.9p.:..^.
+00000790: 132c 43a4 7ec1 7d8a 8a80 11ab 62be baaf  .,C.~.}.....b...
+000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
+000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
+000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
+000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
+000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
+000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
+00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
+00000810: 0304 1400 0000 0800 d050 a858 bbe8 8b38  .........P.X...8
+00000820: 3801 0000 1102 0000 1800 0000 786c 2f77  8...........xl/w
+00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00000840: 2e78 6d6c 4d52 db6e 8330 0cfd 9528 1fd0  .xmlMR.n.0...(..
+00000850: d049 bba8 02a4 b6d3 b43d 4caa 5a6d 7b4e  .I.......=L.Zm{N
+00000860: c140 d424 6689 3bb6 bf9f 03bd 3d44 f838  .@.$f.;.....=D.8
+00000870: 3ee7 d826 f980 e110 3b00 12bf cefa 58c8  >..&....;.....X.
+00000880: 8ea8 5f28 15ab 0e9c 8e33 ecc1 f34d 83c1  .._(.....3...M..
+00000890: 6962 185a 15fb 00ba 1e49 ceaa bb2c 7b50  ib.Z.....I...,{P
+000008a0: 4e1b 2fcb 7ccc 6d42 99e3 91ac f1b0 0922  N./.|.mB......."
+000008b0: 1e9d d3e1 6f05 1687 42ce e539 b135 6d47  ....o...B..9.5mG
+000008c0: 6342 9579 af5b d801 7df4 4c60 a82e 3ab5  cB.y.[..}.L`..:.
+000008d0: 71e0 a341 2f02 3485 5cce 17cb 8931 567c  q..A/.4.\....1V|
+000008e0: 1a18 e24d 2cd2 307b c443 026f 7521 b3d4  ...M,.0{.C.ou!..
+000008f0: 1358 a828 4968 fefc c01a ac4d 4adc c9f7  .X.(Ih.....MJ...
+00000900: 4954 5e4d 13f3 363e cbbf 8cf3 737b 7b1d  IT^M..6>....s{{.
+00000910: 618d f6cb d4d4 15f2 498a 1a1a 7db4 b4c5  a.......I...}...
+00000920: e115 4e33 dd5f 5b7c d6a4 cb3c e020 421a  ..N3._[|...<. B.
+00000930: b6cc ab14 244b 2e34 3e2d 6947 81f3 869d  ....$K.4>-iG....
+00000940: a834 75ae 88fd 1352 151f 669e db99 a4d2  .4u....R..f.....
+00000950: aade 7568 8d8f c242 c32a d9ec 910d c3e4  ..uh...B.*......
+00000960: 3d01 c27e 5ced 1e89 d08d 61c7 bf0c 422a  =..~\.....a...B*
+00000970: e0fb 0691 2e20 cd7e 7905 e53f 504b 0304  ..... .~y..?PK..
+00000980: 1400 0000 0800 d050 a858 0712 deaa ee01  .......P.X......
+00000990: 0000 2104 0000 1800 0000 786c 2f77 6f72  ..!.......xl/wor
+000009a0: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
+000009b0: 6d6c 8554 db6e db30 0cfd 1543 cf45 95f4  ml.T.n.0...C.E..
+000009c0: 8ec0 36d0 240d d687 0245 8b75 8f81 62d3  ..6.$....E.u..b.
+000009d0: b610 5974 25ba 5eff 7e94 9db8 e996 602f  ..Yt%.^.~.....`/
+000009e0: 1649 9187 8717 39ee d06d 7d05 40d1 efda  .I....9..m}.@...
+000009f0: 589f 888a a899 49e9 b30a 6ae5 cfb1 01cb  X.....I...j.....
+00000a00: 3705 ba5a 11ab ae94 be71 a0f2 3ea8 36f2  7..Z.....q..>.6.
+00000a10: 6232 b991 b5d2 56a4 716f 7b76 698c 2d19  b2....V.qo{vi.-.
+00000a20: 6de1 d945 bead 6be5 3ee7 60b0 4bc4 54ec  m..E..k.>.`.K.T.
+00000a30: 0d2f baac a837 c834 6e54 09af 403f 1b0e  ./...7.4nT..@?..
+00000a40: 6055 8e38 b9ae c17a 8d36 7250 24e2 7e3a  `U.8...z.6rP$.~:
+00000a50: 5b0d 11bd c79b 86ce 1fc8 5128 6683 b80d  [.........Q(f...
+00000a60: ca63 9e88 49e0 0406 320a 108a 8f0f 5880  .c..I...2.....X.
+00000a70: 3101 8999 bcef 40c5 57d2 1079 28ef e157  1.....@.W..y(..W
+00000a80: 7dfd 4c6f a33c 2cd0 fcd2 3955 89b8 1351  }.Lo.<,...9U...Q
+00000a90: 0e85 6a0d bd60 f703 7635 5d7f 515c 2a52  ..j..`..v5].Q\*R
+00000aa0: 69ec b08b 5c28 368d b320 8494 eca8 6d68  i...\(6.. ....mh
+00000ab0: d22b 39b6 6bce 44a9 87f7 166c 06eb 421b  .+9.k.D....l..B.
+00000ac0: fef4 4963 49cc 28dc cb6c 173f 3f15 8f1f  ..IcI.(..l.??...
+00000ad0: e02a 65cb 75e6 74b6 5d5f 368e 1b78 0460  .*e.u.t.]_6..x.`
+00000ae0: f15f 808e a78d f634 c2f2 1442 cf3c 434b  ._.....4...B.<CK
+00000af0: 608f 517f 3815 a7f3 23de ab53 def4 d9fc  `.Q.8...#..S....
+00000b00: c54a 7293 f793 1bba 9ef3 f74d 19cd 278f  .Jr........M..'.
+00000b10: df47 19b6 9686 297c bf1a 37e1 6276 3f9d  .G....)|..7.bv?.
+00000b20: 5cdd 5ddf def0 7654 d82d 1d36 4bec 6cd8  \.]...vT.-.6K.l.
+00000b30: a4de f068 9b96 9ec0 7b5e d8d1 f8e0 1cba  ...h....{^......
+00000b40: 43a3 32bc ec73 a3ec b65f f0c0 3511 467b  C.2..s..._..5.F{
+00000b50: e2cc 61a6 ad51 d354 14ca 933a 2bc1 6ed8  ..a..Q.T...:+.n.
+00000b60: f1cc 5bd5 b00c 2296 a34b 2cbf f3fc c7e0  ..[..."..K,.....
+00000b70: 87a7 f3a4 5ca9 b940 0305 d737 39bf e505  ....\..@...79...
+00000b80: 74c3 2e0e 0a61 d333 d920 11d6 bd58 f113  t....a.3. ...X..
+00000b90: 0617 1cf8 be40 a451 096f 61fc 2ba4 7f00  .....@.Q.oa.+...
+00000ba0: 504b 0304 1400 0000 0800 d050 a858 a497  PK.........P.X..
+00000bb0: 6e89 5601 0000 a502 0000 1800 0000 786c  n.V...........xl
+00000bc0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00000bd0: 7433 2e78 6d6c 7552 db6e c230 0cfd 952a  t3.xmluR.n.0...*
+00000be0: 1f40 60d2 2e42 6da5 019a b687 4908 b4ed  .@`..Bm.....I...
+00000bf0: 39b4 2e8d 48e2 92b8 ebf8 fb39 2d97 6982  9...H......9-.i.
+00000c00: a7d8 ce39 c73e 4ed2 0efd 2ed4 0094 fc58  ...9.>N........X
+00000c10: e342 266a a266 2a65 286a b02a 8cb0 01c7  .B&j.f*e(j.*....
+00000c20: 3715 7aab 8853 bf95 a1f1 a0ca 9e64 8dbc  7.z..S.......d..
+00000c30: 1b8f 1fa4 55da 893c ed6b 4b9f a7d8 92d1  ....U..<.kK.....
+00000c40: 0e96 3e09 adb5 ca1f 6660 b0cb c444 9c0a  ..>.....f`...D..
+00000c50: 2bbd ada9 2fc8 3c6d d416 d640 1f0d 1338  +.../.<m...@...8
+00000c60: 9567 9d52 5b70 41a3 4b3c 5499 789e 4c17  .g.R[pA.K<T.x.L.
+00000c70: 03a3 477c 6ae8 c29f 3889 6636 88bb 98bc  ..G|j...8.f6....
+00000c80: 9599 18c7 99c0 4041 5142 f1f1 0d73 3026  ......@AQB...s0&
+00000c90: 2af1 24fb a3a8 b834 8dcc bff1 49fe a5f7  *.$....4....I...
+00000ca0: cfe3 6d54 8039 9a2f 5d52 9d89 2791 9450  ..mT.9./]R..'..P
+00000cb0: a9d6 d00a bb57 387a babf 8cb8 50a4 f2d4  .....W8z....P...
+00000cc0: 6397 f868 364f 8b18 c496 0cd4 2e2e 694d  c..h6O........iM
+00000cd0: 9eeb 9a3b 51ee 9485 5412 4f10 7359 1cf1  ...;Q...T.O.sY..
+00000ce0: b35b f800 fb16 5c71 8d33 bfc5 d1e5 15f4  .[....\q.3......
+00000cf0: e216 9a0e cd3f 75c9 6e4e 2b1a ecc5 e77b  .....?u.nN+....{
+00000d00: 577e ab5d 480c 54ac 331e 3df2 12fc b08f  W~.]H.T.3.=.....
+00000d10: 2121 6cfa e7de 2011 da3e acf9 1b81 8f00  !!l... ..>......
+00000d20: beaf 10e9 9cc4 f738 ffcc fc17 504b 0304  .......8....PK..
+00000d30: 1400 0000 0800 d050 a858 32c0 66ed 4c01  .......P.X2.f.L.
+00000d40: 0000 4d02 0000 1800 0000 786c 2f77 6f72  ..M.......xl/wor
+00000d50: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
+00000d60: 6d6c 7552 db4e c330 0cfd 952a 1f40 3a24  mluR.N.0...*.@:$
+00000d70: 2e9a da4a 6c08 c103 d2b4 0978 4459 ebb6  ...Jl......xDY..
+00000d80: d192 b824 ee0a 7f8f d3ee c603 4fb1 4f7c  ...$........O.O|
+00000d90: 8e8f 9d64 03fa 5d68 0128 f9b6 c685 5cb4  ...d..]h.(....\.
+00000da0: 44dd 5cca 50b6 6055 b8c2 0e1c dfd4 e8ad  D.\.P.`U........
+00000db0: 224e 7d23 43e7 4155 23c9 1a79 9da6 b7d2  "N}#C.AU#..y....
+00000dc0: 2aed 4491 8dd8 ca17 19f6 64b4 8395 4f42  *.D.......d...OB
+00000dd0: 6fad f23f 0b30 38e4 6226 8ec0 5a37 2d8d  o..?.08.b&..Z7-.
+00000de0: 802c b24e 35b0 017a eb98 c0a9 3ce9 54da  .,.N5..z....<.T.
+00000df0: 820b 1a5d e2a1 cec5 c36c be98 1863 c5bb  ...].....l...c..
+00000e00: 8621 5cc4 491c 668b b88b c94b 958b 347a  .!\.I.f....K..4z
+00000e10: 0203 2545 09c5 c71e 9660 4c54 6227 5f07  ..%E.....`LTb'_.
+00000e20: 5171 6e1a 9997 f151 fe69 9c9f ed6d 5580  Qqn....Q.i...mU.
+00000e30: 259a 0f5d 519b 8b7b 9154 50ab ded0 1a87  %..]Q..{.TP.....
+00000e40: 6738 cc74 73b6 f8a8 4815 99c7 21f1 71d8  g8.ts...H...!.q.
+00000e50: 222b 6310 5b72 a176 7149 1bf2 8c6b ee44  "+c.[r.vqI...k.D
+00000e60: 45d9 d3e7 c07b 4697 4962 1f11 95e5 81b5  E....{F.Ib......
+00000e70: f88f 857b f0ad 72cd 5f8e e4ae c751 261b  ...{..r._....Q&.
+00000e80: 71cd afca 37da 85c4 40cd 5ae9 d51d 9bf5  q...7...@.Z.....
+00000e90: 93ef 2921 ecc6 67d9 2211 da31 6cf9 b9c1  ..)!..g."..1l...
+00000ea0: c702 beaf 11e9 94c4 bd9d 7e50 f10b 504b  ..........~P..PK
+00000eb0: 0304 1400 0000 0800 d050 a858 0840 26f8  .........P.X.@&.
+00000ec0: 5c01 0000 8b02 0000 1800 0000 786c 2f77  \...........xl/w
+00000ed0: 6f72 6b73 6865 6574 732f 7368 6565 7435  orksheets/sheet5
+00000ee0: 2e78 6d6c 7552 db4e c330 0cfd 952a 1f40  .xmluR.N.0...*.@
+00000ef0: 3624 2e42 6d25 3684 e001 6902 018f 286b  6$.Bm%6...i...(k
+00000f00: dd36 5a12 17c7 a38c afc7 e96e 20c1 537c  .6Z........n .S|
+00000f10: 3bf6 3976 f201 6915 3b00 ce3e bd0b b150  ;.9v..i.;..>...P
+00000f20: 1d73 7fa5 75ac 3af0 269e 600f 4132 0d92  .s..u.:.&.`.A2..
+00000f30: 372c 2eb5 3af6 04a6 1e41 dee9 d3c9 e45c  7,..:....A.....\
+00000f40: 7b63 832a f331 b6a0 32c7 353b 1b60 4159  {c.*.1..2.5;.`AY
+00000f50: 5c7b 6f68 3303 8743 a1a6 6a1f 78b4 6dc7  \{oh3..C..j.x.m.
+00000f60: 6340 9779 6f5a 7802 7eee 0520 ae3e f4a9  c@.yoZx.~.. .>..
+00000f70: ad87 102d 868c a029 d4f5 f46a be45 8c15  ...-...)...j.E..
+00000f80: 2f16 86f8 c3ce 9298 25e2 2a39 f775 a126  /.......%.*9.u.&
+00000f90: 8913 38a8 38b5 30f2 7cc0 1c9c 4b9d 84c9  ..8.8.0.|...K...
+00000fa0: fbae a93a 0e4d c89f f6be fded a85f e82d  ...:.M......._.-
+00000fb0: 4d84 39ba 575b 7357 a84b 95d5 d098 b5e3  M.9.W[sW.K......
+00000fc0: 471c ee60 a7e9 ec48 f1c6 b029 73c2 21a3  G..`...H...)s.!.
+00000fd0: 24b6 ccab 64a4 9152 6843 5ad2 1393 c4ad  $...d..RhCZ.....
+00000fe0: 4ce2 9220 32d9 91ee 1b84 af8d 875c b3f0  L.. 2........\..
+00000ff0: 4959 5ded d0b3 ffd0 d59a df06 b912 863f  IY]............?
+00001000: 50f3 ff50 f801 d499 d0fe c668 e1bc 5fc4  P..P.......h.._.
+00001010: 5644 3ad2 83a1 d686 9839 68a4 d7e4 e442  VD:......9h....B
+00001020: a4d2 56f5 d661 ecc7 a32e 9119 fd68 76f2  ..V..a.......hv.
+00001030: 5980 5281 e41b 443e 3869 eb87 ff57 7e03  Y.R...D>8i...W~.
+00001040: 504b 0304 1400 0000 0800 d050 a858 4ec7  PK.........P.XN.
+00001050: 5d80 8a01 0000 9103 0000 1800 0000 786c  ].............xl
+00001060: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00001070: 7436 2e78 6d6c 8553 6d4f dc30 0cfe 2b55  t6.xml.SmO.0..+U
+00001080: 7e00 3986 3626 d456 8263 ecf6 6112 026d  ~.9.6&.V.c..a..m
+00001090: 7c3c e55a b78d 2e8d 83e3 d2f1 efe7 f45e  |<.Z...........^
+000010a0: 00e9 2a3e c576 fc3c 7e1c 3bf9 88b4 8d1d  ..*>.v.<~.;.....
+000010b0: 0067 ff7a e763 a13a e670 a575 ac3a e84d  .g.z.c.:.p.u.:.M
+000010c0: 3cc3 005e 6e1a a4de b0b8 d4ea 1808 4c3d  <..^n.........L=
+000010d0: 817a a7bf 2c16 df74 6fac 5765 3ec5 eea9  .z..,..to.We>...
+000010e0: cc71 6067 3ddc 5316 87be 37f4 7a03 0ec7  .q`g=.S...7.z...
+000010f0: 429d ab43 e0c1 b61d 4f01 5de6 c1b4 f008  B..C....O.].....
+00001100: fc27 0840 5c7d e4a9 6d0f 3e5a f419 4153  .'.@\}..m.>Z..AS
+00001110: a8eb f3ab d50e 3165 fcb5 30c6 7776 969a  ......1e..0.wv..
+00001120: d920 6e93 f3ab 2ed4 2269 0207 1527 0a23  . n....."i...'.#
+00001130: c70b 2cc1 b9c4 244a 9ef7 a4ea ad68 42be  ..,...$J.....hB.
+00001140: b70f f477 53ff 226f 6322 2cd1 3dd9 9abb  ...wS."oc",.=...
+00001150: 427d 5759 0d8d 191c 3fe0 b882 7d4f 5fdf  B}WY....?...}O_.
+00001160: 24de 1a36 654e 3866 949a 2df3 2a19 a9a4  $..6eN8f..-.*...
+00001170: 245a 9f1e e991 49e2 562a 7189 2f40 9df1  $Z....I.V*q./@..
+00001180: edba 225b 6dd7 1781 e401 72cd 2229 25e8  .."[m.....r.")%.
+00001190: 6a4f 70f3 29c1 28d3 423f cfb0 9c63 1822  jOp.).(.B?...c."
+000011a0: d0da fa30 f009 d4ed 1caa b254 0dce d009  ...0.......T....
+000011b0: cc8f 39cc 5c91 bbd9 e606 3e8d f839 87e0  ..9.\.....>..9..
+000011c0: d770 aaf9 d5ac a4fa 63b6 96c9 1dd6 6137  .p......c.....a7
+000011d0: cab4 aabf 0db5 d6c7 cc41 232c 8bb3 4b19  .........A#,..K.
+000011e0: 38ed 66bf 7318 c3b4 da1b 64c6 7e32 3bf9  8.f.s.....d.~2;.
+000011f0: 3240 2941 ee1b 443e 3a69 f78e bfb0 fc0f  2@)A..D>:i......
+00001200: 504b 0304 1400 0000 0800 d050 a858 4409  PK.........P.XD.
+00001210: 9006 e701 0000 3704 0000 1800 0000 786c  ......7.......xl
+00001220: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00001230: 7437 2e78 6d6c 7554 4d6f a330 10fd 2bc8  t7.xmluTMo.0..+.
+00001240: e7aa 26d5 f643 1120 3549 dbed a152 d56a  ..&..C. 5I...R.j
+00001250: db63 e5c0 0056 8c4d ed61 69ff fd8e 4d42  .c...V.M.ai...MB
+00001260: 132d 5cf0 cc78 decc 1bfb 99a4 3776 e76a  .-\..x......7v.j
+00001270: 008c be1a a55d ca6a c476 c9b9 cb6b 6884  .....].j.v...kh.
+00001280: 3b37 2d68 da29 8d6d 0492 6b2b ee5a 0ba2  ;7-h.).m..k+.Z..
+00001290: 08a0 46f1 8b38 bee2 8d90 9a65 4988 3ddb  ..F..8.....eI.=.
+000012a0: 2c31 1d2a a9e1 d946 ae6b 1a61 bf57 a04c  ,1.*...F.k.a.W.L
+000012b0: 9fb2 053b 045e 6455 6308 f02c 6945 05af  ...;.^dUc..,iE..
+000012c0: 807f 5a02 90cb c73a 856c 403b 6974 64a1  ..Z....:.l@;itd.
+000012d0: 4cd9 ed62 f930 2042 c69b 84de 1dd9 911f  L..b.0 B........
+000012e0: 666b ccce 3b8f 45ca 62cf 0914 e4e8 4b08  fk..;.E.b.....K.
+000012f0: 5afe c21a 94f2 9588 c9e7 be28 fb69 ea91  Z..........(.i..
+00001300: c7f6 a1fc 7d98 9fe8 6d85 83b5 51ef b2c0  ....}...m...Q...
+00001310: 3a65 372c 2aa0 149d c217 d3ff 86fd 4c97  :e7,*.........L.
+00001320: 3f14 3702 4596 58d3 47d6 0f9b 25b9 377c  ?.7.E.X.G...%.7|
+00001330: 4b4a 94da 1fd2 2b5a 8a4b ea84 9983 cf0e  KJ....+Z.K......
+00001340: 740e 1fa5 54f4 094d 138e c4c8 eff3 7c8f  t...T..M......|.
+00001350: 5fcd e103 4c8b 0626 40eb 3990 d405 7c7d  _...L..&@.9...|}
+00001360: 481d 9a4e 0037 f3c0 b69b a277 3707 2059  H..N.7.....w7. Y
+00001370: 4c23 eee7 10f8 dd4e 517a 98a5 549c 6673  L#.....NQz..T.fs
+00001380: 3afa c37d 0e77 51d0 f74d 2849 2b89 c245  :..}.wQ..M(I+..E
+00001390: b9e9 340e 7773 ba35 eae3 6279 bb88 7fdd  ..4.ws.5..by....
+000013a0: 5c5e 5f91 666a d36f ac69 37a6 d75e 5f21  \^_.fj.o.i7..^_!
+000013b0: f0e8 cfe1 099c 2319 8fc1 3b6b 8d3d 0e0a  ......#...;k.=..
+000013c0: 454f 60a5 84de 05d9 fbc9 52a6 a443 eaec  EO`.......R..C..
+000013d0: 6fba 5362 91b1 5238 1467 15e8 2d25 9e39  o.Sb..R8.g..-%.9
+000013e0: 2d5a b281 257c 4c49 f829 cfff 026e 7850  -Z..%|LI.)...nxP
+000013f0: 4fc2 5692 0654 50d2 7cf1 f935 c9d2 0e0a  O.V..TP.|..5....
+00001400: 1d1c 346d 60b2 3588 a609 664d 0f1b ac4f  ..4m`.5...fM...O
+00001410: a0fd d218 1c1d ff42 c67f 45f6 0f50 4b03  .......B..E..PK.
+00001420: 0414 0000 0008 00d0 50a8 5891 c100 8bd2  ........P.X.....
+00001430: 0100 00f6 0300 0018 0000 0078 6c2f 776f  ...........xl/wo
+00001440: 726b 7368 6565 7473 2f73 6865 6574 382e  rksheets/sheet8.
+00001450: 786d 6c8d 53db 6edb 300c fd15 43cf 43e5  xml.S.n.0...C.C.
+00001460: 14bd 21b0 0d34 4983 f5a1 40d1 62ed e3a0  ..!..4I...@.b...
+00001470: d8b4 2d44 165d 899e 97bf 1f65 276e ba25  ..-D.].....e'n.%
+00001480: c05e 24de 0ec5 4352 498f 6eeb 6b00 8a7e  .^$...CRI.n.k..~
+00001490: 37c6 fa54 d444 ed5c 4a9f d7d0 287f 812d  7..T.D.\J...(..-
+000014a0: 58f6 94e8 1a45 acba 4afa d681 2a06 5063  X....E..J...*.Pc
+000014b0: e465 1cdf c846 692b b264 b03d bb2c c18e  .e...Fi+.d.=.,..
+000014c0: 8cb6 f0ec 22df 358d 72bb 0518 ec53 3113  ....".5.r....S1.
+000014d0: 07c3 8bae 6a1a 0c32 4b5a 55c1 2bd0 8f96  ....j..2KZU.+...
+000014e0: 01ac ca29 4fa1 1bb0 5ea3 8d1c 94a9 b89f  ...)O...^.......
+000014f0: cdd7 2362 8878 d3d0 fb23 390a 6436 88db  ..#b.x...#9.d6..
+00001500: a03c 16a9 8843 4d60 20a7 9042 f1f5 0b96  .<...CM` ..B....
+00001510: 604c c8c4 957c ec93 8acf 4703 f258 3ea4  `L...|....G..X>.
+00001520: 5f0f fcb9 bc8d f2b0 44f3 ae0b aa53 7127  _.......D....Sq'
+00001530: a202 4ad5 197a c1fe 3bec 395d 7f96 b852  ..J..z..;.9]...R
+00001540: a4b2 c461 1fb9 4036 4bf2 2084 2739 50db  ...a..@6K. .'9P.
+00001550: d0a4 5772 6cd7 fc12 650e 5af4 9ad0 ed7e  ..Wrl...e.Z....~
+00001560: 5ad5 4022 898b 092e 99ef a18b ff80 eae2  Z.@"............
+00001570: 0470 790e a86d dbd1 09c0 ea1c 8087 7b1a  .py..m........{.
+00001580: f170 0e41 bbf6 1497 f5d9 92fe 2220 b981  .p.A........" ..
+00001590: 87a9 8c1d 2df8 7c53 46f3 cda3 f551 8e9d  ....-.|SF....Q..
+000015a0: a5b1 c35f 5dd3 942f e7f7 b3f8 eaee faf6  ..._]../........
+000015b0: 8627 5f63 bf72 d8ae b0b7 614b 06c3 63e8  .'_c.r....aK..c.
+000015c0: c313 78cf cb38 191f 9c43 776c 5486 1779  ..x..8...CwlT..y
+000015d0: 6194 dd0e cb1b 98a5 c268 4ffc 72f8 249d  a........hO.r.$.
+000015e0: 51b3 4ca8 a2a8 c0c2 373e 361c 2a12 39f9  Q.L.....7>6.*.9.
+000015f0: 12f9 b5c0 7f0c 7efc 0f4f ca55 9a99 1928  ......~..O.U...(
+00001600: 9958 7c71 cb5b e5c6 051b 15c2 7628 6183  .X|q.[......v(a.
+00001610: 44d8 0c62 cdff 125c 0860 7f89 4893 1216  D..b...\.`..H...
+00001620: 7cfa ead9 1f50 4b03 0414 0000 0008 00d0  |....PK.........
+00001630: 50a8 58d3 d762 9c0b 0200 0031 0500 0018  P.X..b.....1....
+00001640: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00001650: 2f73 6865 6574 392e 786d 6cbd 544d 6fdb  /sheet9.xml.TMo.
+00001660: 300c fd2b 86ce 5d95 04eb 0702 dbc0 92b4  0..+..].........
+00001670: 4b0f 058a 16ed 8e81 62d3 b110 5974 257a  K.......b...Yt%z
+00001680: 5eff fd28 2771 b320 1e76 dac5 1629 bea7  ^..('q. .v...)..
+00001690: 4791 54dc a2db fa12 80a2 5f95 b13e 1125  G.T......._..>.%
+000016a0: 513d 95d2 6725 54ca 5f62 0d96 770a 7495  Q=..g%T._b..w.t.
+000016b0: 2236 dd46 fada 81ca 3b50 65e4 6434 ba96  "6.F....;Pe.d4..
+000016c0: 95d2 56a4 71e7 7b72 698c 0d19 6de1 c945  ..V.q.{ri...m..E
+000016d0: bea9 2ae5 3e66 60b0 4dc4 581c 1ccf 7a53  ..*.>f`.M.X...zS
+000016e0: 52e7 9069 5cab 0dbc 00bd d60c 6053 f63c  R..i\.......`S.<
+000016f0: b9ae c07a 8d36 7250 24e2 db78 badc 21ba  ...z.6rP$..x..!.
+00001700: 8837 0dad 3f5a 4721 9935 e236 180f 7922  .7..?ZG!.5.6..y"
+00001710: 4641 1318 c828 5028 fefd 8439 1813 9858  FA...(P(...9...X
+00001720: c9fb 9e54 7c1e 1a90 c7eb 03fd 7d97 3fcb  ...T|.......}.?.
+00001730: 5b2b 0f73 343f 744e 6522 6e45 9443 a11a  [+.s4?tNe"nE.C..
+00001740: 43cf d82e 619f d3d5 a7c4 8522 95c6 0edb  C...a......"....
+00001750: c885 64d3 380b 8b70 2407 6a1b 2ee9 851c  ..d.8..p$.j.....
+00001760: fb35 9f44 a987 f706 6c06 ab42 1b58 35ce  .5.D....l..B.X5.
+00001770: c492 584e d894 d91e 3c1b 02ab 3cdf 8085  ..XN....<...<...
+00001780: 554f 421f 359c 2198 0f11 38a8 d16b 42f7  UOB.5.!...8..kB.
+00001790: b1b2 aa3a 075d fc03 54e7 6780 7743 406d  ...:.]..T.g.wC@m
+000017a0: eb86 ce00 ee87 00dc 5ae7 11df 8710 03d7  ........Z.......
+000017b0: b01c 9474 9280 e4f2 1d7a 6257 cf9c bf6f  ...t.....zbW...o
+000017c0: ca68 fe73 63f9 28c3 c632 d544 9c6e 1d7a  .h.sc.(..2.D.n.z
+000017d0: 6c36 99ce c6a3 afb7 5737 d7dc 7725 b60b  l6......W7..w%..
+000017e0: 87f5 025b 1b7a b473 3c84 7b78 04ef 7914  ...[.z.s<.{x..y.
+000017f0: 7ae7 9d73 e88e 9dca f018 cd8c b2db 6e74  z..s..........nt
+00001800: 4266 8930 da13 9f1c 46b4 316a 9c8a fc50  Bf.0....F.1j...P
+00001810: 8c2f 4563 ccc5 be2f 3a43 c4b2 8f8b e59f  ./Ec.../:C......
+00001820: 6287 c4cf 27d3 f9ff 13bf 577b c19f 3587  b...'.....W{..5.
+00001830: fe5d f089 c3ef 9e92 47e5 369a cb62 a0e0  .]......G.6..b..
+00001840: aa8c 2e6f 7820 dd6e 3677 0661 dd49 5823  ...ox .n6w.a.IX#
+00001850: 1156 ddb2 e427 0d5c 08e0 fd02 917a 23bc  .V...'.\.....z#.
+00001860: 0dfd 2b99 fe06 504b 0304 1400 0000 0800  ..+...PK........
+00001870: d050 a858 1a82 8f86 9c01 0000 1a04 0000  .P.X............
+00001880: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00001890: 732f 7368 6565 7431 302e 786d 6c7d 94db  s/sheet10.xml}..
+000018a0: 4ee4 300c 865f a5ca 0390 0109 58a1 b6d2  N.0.._......X...
+000018b0: 321c 1721 2110 bb97 a34c ebb6 1149 5c12  2..!!....L...I\.
+000018c0: 97ee bcfd 3a9d 0368 d570 35b6 e3ef cfef  ....:..h.p5.....
+000018d0: ca99 7c44 ff16 3a00 cafe 5ae3 4221 3aa2  ..|D..:...Z.B!:.
+000018e0: fe42 ca50 7560 5538 c21e 1c9f 34e8 ad22  .B.Pu`U8....4.."
+000018f0: 4e7d 2b43 ef41 d513 648d 3c59 2cce a455  N}+C.A..d.<Y,..U
+00001900: da89 329f 6a4f becc 7120 a31d 3cf9 2c0c  ..2.jO..q ..<.,.
+00001910: d62a bfb9 0483 6321 8ec5 bef0 acdb 8ea6  .*....c!........
+00001920: 822c f35e b5f0 02f4 da33 c0a9 3ce8 d4da  .,.^.....3..<...
+00001930: 820b 1a5d e6a1 29c4 cfe3 8b87 2d31 75fc  ...]..).....-1u.
+00001940: d630 862f 7116 8759 23be c5e4 be2e c422  .0./q..Y#......"
+00001950: 7a02 0315 4509 c53f 1fb0 0463 a212 3b79  z...E..?...c..;y
+00001960: df89 8acf 4b23 f935 decb df4c f3b3 bdb5  ....K#.5...L....
+00001970: 0ab0 44f3 47d7 d415 e287 c86a 68d4 60e8  ..D.G......jh.`.
+00001980: 19c7 3bd8 cd74 fa69 f14a 912a 738f 63e6  ..;..t.i.J.*s.c.
+00001990: e3b0 655e c520 5ec9 8dda c58f f442 9eeb  ..e^. ^......B..
+000019a0: 9a6f a252 8500 766d 362b 5555 10e2 e0b9  .o.R..vm6+UU....
+000019b0: 24f6 134f 65b5 a32f 5374 80f7 015c 05df  $..Oe../St...\..
+000019c0: d2cb 146d b01a c28a 543b 035d a5a0 161c  ...m....T;.]....
+000019d0: ac74 3d83 5c27 5d92 f234 03dc a400 7073  .t=.\']..4....ps
+000019e0: fab7 697d af66 89bb 14a1 5d3f cc39 ba4f  ..i}.f....]?.9.O
+000019f0: 01bc def3 c4af 1441 9b1e 66fa 1f92 96fe  .......A..f.....
+00001a00: 1b40 f20a edf7 72bb 53f1 cd3c 2adf 6a17  .@....r.S..<*.j.
+00001a10: 3203 0dab 2c8e ce79 f3fc 7609 b709 613f  2...,..y..v...a?
+00001a20: bdb1 3512 a19d c28e df2e f8d8 c0e7 0d22  ..5............"
+00001a30: 1d92 f808 0e7f 07e5 3f50 4b03 0414 0000  ........?PK.....
+00001a40: 0008 00d0 50a8 5882 b2f4 9d67 0100 000f  ....P.X....g....
+00001a50: 0300 0019 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
+00001a60: 6565 7473 2f73 6865 6574 3131 2e78 6d6c  eets/sheet11.xml
+00001a70: 7553 db4e c330 0cfd 952a 1f40 3624 2e9a  uS.N.0...*.@6$..
+00001a80: da4a 6c63 8207 a469 13f0 88b2 d66d a3e5  .Jlc...i.....m..
+00001a90: 46e2 51f6 f738 ed6e 48eb 536d c7c7 3e3e  F.Q..8.nH.Sm..>>
+00001aa0: 76d3 d6fa 6d68 0030 f9d5 ca84 8c35 886e  v...mh.0.....5.n
+00001ab0: c279 281a d022 dc58 0786 5e2a ebb5 4072  .y(..".X..^*..@r
+00001ac0: 7dcd 83f3 20ca 0ea4 15bf 1d8d eeb9 16d2  }... ...........
+00001ad0: b03c ed62 4b9f a776 874a 1a58 fa24 ecb4  .<.bK..v.J.X.$..
+00001ae0: 167e 3f05 65db 8c8d d931 b092 7583 5d80  .~?.e....1..u.].
+00001af0: e7a9 1335 ac01 df1d 01c8 e5a7 3aa5 d460  ...5........:..`
+00001b00: 82b4 26f1 5065 ec69 3c59 f488 2ee3 4342  ..&.Pe.i<Y....CB
+00001b10: 1b2e ec24 0eb3 b176 1b9d d732 63a3 c809  ...$...v...2c...
+00001b20: 1414 184b 08fa fcc0 0c94 8a95 88c9 f7a1  ...K............
+00001b30: 283b 378d c84b fb58 7ed1 cd4f f436 22c0  (;7..K.X~..O.6".
+00001b40: ccaa 4f59 6293 b147 9694 5089 9dc2 956d  ..OYb..G..P....m
+00001b50: 5fe0 30d3 dd99 e25c a0c8 536f dbc4 c761  _.0....\..So...a
+00001b60: f3b4 8846 6c49 89d2 4491 d6e8 292e a913  ...FlI..D...)...
+00001b70: e60a 2afc 82b2 8694 23d1 8841 5e1c 40d3  ..*.....#..A^.@.
+00001b80: 2190 8f6d 8750 b321 9434 6e87 5700 f321  !..m.P.!.4n.W..!
+00001b90: 00ed f43a e279 0881 7b77 8dd2 6290 52f9  ...:.y..{w..b.R.
+00001ba0: 3f9b 936e c765 f442 c643 7913 be96 2624  ?..n.e.B.Cy...&$
+00001bb0: 512b 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b  Q+Z.....{.{....k
+00001bc0: 6311 adee cc86 0e16 7c4c a0f7 ca5a 3c39  c.......|L...Z<9
+00001bd0: 71f3 a77f 20ff 0350 4b03 0414 0000 0008  q... ..PK.......
+00001be0: 00d0 50a8 5882 b2f4 9d67 0100 000f 0300  ..P.X....g......
+00001bf0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00001c00: 7473 2f73 6865 6574 3132 2e78 6d6c 7553  ts/sheet12.xmluS
+00001c10: db4e c330 0cfd 952a 1f40 3624 2e9a da4a  .N.0...*.@6$...J
+00001c20: 6c63 8207 a469 13f0 88b2 d66d a3e5 46e2  lc...i.....m..F.
+00001c30: 51f6 f738 ed6e 48eb 536d c7c7 3e3e 76d3  Q..8.nH.Sm..>>v.
+00001c40: d6fa 6d68 0030 f9d5 ca84 8c35 886e c279  ..mh.0.....5.n.y
+00001c50: 281a d022 dc58 0786 5e2a ebb5 4072 7dcd  (..".X..^*..@r}.
+00001c60: 83f3 20ca 0ea4 15bf 1d8d eeb9 16d2 b03c  .. ............<
+00001c70: ed62 4b9f a776 874a 1a58 fa24 ecb4 167e  .bK..v.J.X.$...~
+00001c80: 3f05 65db 8c8d d931 b092 7583 5d80 e7a9  ?.e....1..u.]...
+00001c90: 1335 ac01 df1d 01c8 e5a7 3aa5 d460 82b4  .5........:..`..
+00001ca0: 26f1 5065 ec69 3c59 f488 2ee3 4342 1b2e  &.Pe.i<Y....CB..
+00001cb0: ec24 0eb3 b176 1b9d d732 63a3 c809 1414  .$...v...2c.....
+00001cc0: 184b 08fa fcc0 0c94 8a95 88c9 f7a1 283b  .K............(;
+00001cd0: 378d c84b fb58 7ed1 cd4f f436 22c0 ccaa  7..K.X~..O.6"...
+00001ce0: 4f59 6293 b147 9694 5089 9dc2 956d 5fe0  OYb..G..P....m_.
+00001cf0: 30d3 dd99 e25c a0c8 536f dbc4 c761 f3b4  0....\..So...a..
+00001d00: 8846 6c49 89d2 4491 d6e8 292e a913 e60a  .FlI..D...).....
+00001d10: 2afc 82b2 8694 23d1 8841 5e1c 40d3 2190  *.....#..A^.@.!.
+00001d20: 8f6d 8750 b321 9434 6e87 5700 f321 00ed  .m.P.!.4n.W..!..
+00001d30: f43a e279 0881 7b77 8dd2 6290 52f9 3f9b  .:.y..{w..b.R.?.
+00001d40: 936e c765 f442 c643 7913 be96 2624 512b  .n.e.B.Cy...&$Q+
+00001d50: 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b 6311  Z.....{.{....kc.
+00001d60: adee cc86 0e16 7c4c a0f7 ca5a 3c39 71f3  ......|L...Z<9q.
+00001d70: a77f 20ff 0350 4b03 0414 0000 0008 00d0  .. ..PK.........
+00001d80: 50a8 58fb c712 8d4a 0100 0075 0200 0019  P.X....J...u....
+00001d90: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00001da0: 2f73 6865 6574 3133 2e78 6d6c 7552 d94e  /sheet13.xmluR.N
+00001db0: c330 10fc 95c8 1f50 a748 1caa 9248 3408  .0.....P.H...H4.
+00001dc0: c103 52d5 0a78 7693 4d62 d5f6 067b 4be0  ..R..xv.Mb...{K.
+00001dd0: ef59 273d 10a2 4fde 6b66 676c 6703 fa5d  .Y'=..O.kfglg..]
+00001de0: e800 28f9 b2c6 855c 7444 fd42 ca50 7560  ..(....\tD.B.Pu`
+00001df0: 5598 610f 8e3b 0d7a ab88 53df cad0 7b50  U.a..;.z..S...{P
+00001e00: f508 b246 5ea5 e98d b44a 3b51 6463 6de5  ...F^....J;Qdcm.
+00001e10: 8b0c f764 b483 954f c2de 5ae5 bf97 6070  ...d...O..Z...`p
+00001e20: c8c5 5c1c 0b6b dd76 3416 6491 f5aa 850d  ..\..k.v4.d.....
+00001e30: d06b cf00 4ee5 89a7 d616 5cd0 e812 0f4d  .k..N.....\....M
+00001e40: 2eee e78b 7242 8c13 6f1a 86f0 2b4e a299  ....rB..o...+N..
+00001e50: 2de2 2e26 cf75 2ed2 a809 0c54 1429 141f  -..&.u.....T.)..
+00001e60: 9f50 8231 9189 957c 1c48 c579 6944 fe8e  .P.1...|.H.yiD..
+00001e70: 8ff4 8fa3 7f96 b755 014a 34ef baa6 2e17  .......U.J4.....
+00001e80: 7722 a9a1 517b 436b 1c9e e0e0 e9fa 2cf1  w"..Q{Ck......,.
+00001e90: 4191 2a32 8f43 e2a3 d922 ab62 1057 f2a0  A.*2.C...".b.W..
+00001ea0: 76f1 9236 e4b9 ae79 1315 8194 a74c 124b  v..6...y.....L.K
+00001eb0: 8805 591d 00cb 4b00 70f5 3fe3 e565 7eaf  ..Y...K.p.?..e~.
+00001ec0: fe22 24ab 3b5a 9ee4 c6e7 7851 bed5 2e24  ."$.;Z....xQ...$
+00001ed0: 061a 664a 67b7 6cca 4ffe a684 b01f 9f6f  ..fJg.l.O......o
+00001ee0: 8b44 68c7 b0e3 6f01 3e0e 70bf 41a4 5312  .Dh...o.>.p.A.S.
+00001ef0: eff7 f4d3 8a1f 504b 0304 1400 0000 0800  ......PK........
+00001f00: d050 a858 2751 7b71 5a01 0000 c902 0000  .P.X'Q{qZ.......
+00001f10: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00001f20: 732f 7368 6565 7431 342e 786d 6c7d 52db  s/sheet14.xml}R.
+00001f30: 4ec3 300c fd95 2a1f b06c 485c 84da 4a6c  N.0...*..lH\..Jl
+00001f40: 1382 07a4 6908 7844 59eb b6d1 92ba 241e  ....i.xDY.....$.
+00001f50: 85bf c7ee ae0f 634f f1ed f8f8 d849 7b0c  ......cO.....I{.
+00001f60: ebd8 0050 f2e3 5d1b 33d5 1075 f75a c7a2  ...P..].3..u.Z..
+00001f70: 016f e208 3b68 3953 61f0 86d8 0db5 8e5d  .o..;h9Sa......]
+00001f80: 0053 0e20 eff4 d578 7ca3 bdb1 adca d321  .S. ...x|......!
+00001f90: b608 798a 1b72 b685 4548 e2c6 7b13 7ea7  ..y..r..EH..{.~.
+00001fa0: e0b0 cfd4 44ed 034b 5b37 3404 749e 76a6  ....D..K[74.t.v.
+00001fb0: 8657 a0b7 8e01 ecea 439f d27a 68a3 c536  .W......C..zh..6
+00001fc0: 0950 65ea 6172 3fdf 2286 8a77 0b7d 3cb1  .Pe.ar?."..w.}<.
+00001fd0: 1311 b342 5c8b f35c 666a 2c33 8183 82a4  ...B\..\fj,3....
+00001fe0: 85e1 e71b 66e0 9c74 e249 be76 4dd5 9154  ....f..t.I.vM..T
+00001ff0: 90a7 f6be fde3 a09f c75b 9908 3374 1fb6  .........[..3t..
+00002000: a426 5377 2a29 a132 1b47 4bec 9f60 a7e9  .&Sw*).2.GK..`..
+00002010: fa38 e2dc 90c9 d380 7d12 446c 9e16 6208  .8......}.Dl..b.
+00002020: 2517 da56 96f4 4a81 e396 9928 7750 d167  %..V..J....(wP.g
+00002030: 154c cdb2 29d5 c4a3 4842 173b e0f4 3f60  .L..)...HB.;..?`
+00002040: 10ea 4bc8 d945 4a87 8591 1d9d 01ce 2f53  ..K..EJ......./S
+00002050: 9e47 6a56 bc5f e376 0572 e217 136a dbc6  .GjV._.v.r...j..
+00002060: 4428 f938 a35b 5e54 d8ee 6ceb 1076 c397  D(.8.[^T..l..v..
+00002070: 5821 11fa c16c f8ab 4190 02ce 5788 7470  X!...l..A...W.tp
+00002080: e466 87df 9bff 0150 4b03 0414 0000 0008  .f.....PK.......
+00002090: 00d0 50a8 5844 ff81 0869 0100 000c 0300  ..P.XD...i......
+000020a0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+000020b0: 7473 2f73 6865 6574 3135 2e78 6d6c 7553  ts/sheet15.xmluS
+000020c0: db6e 8330 0cfd 1594 0f68 da49 bba8 02a4  .n.0.....h.I....
+000020d0: b55d b53d 4caa 5a6d 7b0e 604a d45c 5862  .].=L.Zm{.`J.\Xb
+000020e0: c6fa f773 a0b7 49f0 84ed f81c 1f5f 885b  ...s..I......_.[
+000020f0: eb0e be02 c0e8 572b e313 5621 d673 ce7d  ......W+..V!.s.}
+00002100: 5e81 167e 626b 30f4 525a a705 92eb f6dc  ^..~bk0.RZ......
+00002110: d70e 44d1 81b4 e277 d3e9 03d7 421a 96c6  ..D....w....B...
+00002120: 5d6c e3d2 d836 a8a4 818d 8b7c a3b5 70c7  ]l...6.....|..p.
+00002130: 0528 db26 6cc6 ce81 addc 57d8 0578 1ad7  .(.&l.....W..x..
+00002140: 620f 3bc0 8f9a 00e4 f20b 4f21 3518 2fad  b.;.......O!5./.
+00002150: 891c 9409 7b9e cdd7 3da2 cbf8 94d0 fa1b  ....{...=.......
+00002160: 3b0a cd64 d61e 82f3 5624 6c1a 3481 821c  ;..d....V$l.4...
+00002170: 0385 a0cf 0f2c 41a9 c044 4abe 4fa4 ec5a  .....,A..DJ.O..Z
+00002180: 3420 6fed 33fd baeb 9fe4 65c2 c3d2 aa2f  4 o.3.....e..../
+00002190: 5960 95b0 2716 1550 8a46 e1d6 b6af 70ea  Y`..'..P.F....p.
+000021a0: e9fe 2a71 2550 a4b1 b36d e442 b369 9c07  ..*q%P...m.B.i..
+000021b0: 2394 a444 69c2 9076 e828 2ea9 12a6 b974  #..Di..v.(.....t
+000021c0: 79a3 848b 3992 8a10 e3f9 09b3 18c3 08ef  y...9...........
+000021d0: 4167 ea38 8059 8e61 a4a9 1b1c 00ac c600  Ag.8.Y.a........
+000021e0: b4d0 61c4 cb18 028f 350c e4af 4725 15ff  ..a.....5...G%..
+000021f0: b339 0ded bc89 7e8a e14a de85 db4b e323  .9....~..J...K.#
+00002200: 0525 b14c 278f 346b d78f bd77 d0d6 dd55  .%.L'.4k...w...U
+00002210: 6516 d1ea ceac e85a c185 047a 2fad c58b  e......Z...z/...
+00002220: 13d6 7ef9 01d2 3f50 4b03 0414 0000 0008  ..~...?PK.......
+00002230: 00d0 50a8 5811 26ee aa80 0100 0080 0300  ..P.X.&.........
+00002240: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00002250: 7473 2f73 6865 6574 3136 2e78 6d6c 7593  ts/sheet16.xmlu.
+00002260: 594f c330 0c80 ff4a 951f 4006 1287 505b  YO.0...J..@...P[
+00002270: 898d 633c 2021 10f0 88b2 d65d 2372 e1b8  ..c< !.....]#r..
+00002280: 94fd 7b9c ee00 a4f6 29b6 e3cf 47ec e4bd  ..{.....)...G...
+00002290: c78f d802 50f6 6d8d 8b85 6889 c2a5 94b1  ....P.m...h.....
+000022a0: 6ac1 aa78 e403 38be 693c 5a45 ace2 5ac6  j..x..8.i<ZE..Z.
+000022b0: 80a0 ea01 b246 9ecc 6667 d22a ed44 990f  .....F..fg.*.D..
+000022c0: b647 2c73 df91 d10e 1e31 8b9d b50a 3773  .G,s.....1....7s
+000022d0: 30be 2fc4 b1d8 1b9e f4ba a5c1 20cb 3ca8  0./......... .<.
+000022e0: 353c 03bd 0406 5895 8738 b5b6 e0a2 f62e  5<....X..8......
+000022f0: 4368 0a71 757c b9dc 1283 c7ab 863e fe91  Ch.qu|.......>..
+00002300: b3d4 ccca fb8f a4dc d785 98a5 9ac0 4045  ..............@E
+00002310: 2984 e2e3 0b16 604c 8ac4 957c ee82 8adf  ).....`L...|....
+00002320: a489 fc2b efc3 df0e fd73 792b 1561 e1cd  ...+.....sy+.a..
+00002330: 9bae a92d c485 c86a 6854 67e8 c9f7 4bd8  ...-...jhTg...K.
+00002340: f574 fa5b e2b5 2255 e6e8 fb0c 53b3 655e  .t.[.."U....S.e^
+00002350: 2521 a564 47ed d223 3d13 b25d 7326 2af9  %!.dG..#=..]s&*.
+00002360: 997b 85f5 7b40 6e1c 7349 5c4b ba91 d58e  .{..{@n.sI\K....
+00002370: 9c4f 9108 5f80 11a6 c9c5 1459 69ac 3aa3  .O.._......Yi.:.
+00002380: c698 eb29 46c5 0876 6536 23cc cd14 a35d  ...)F..ve6#....]
+00002390: e868 04b8 9d02 7889 c689 bb29 8236 0146  .h....x....).6.F
+000023a0: fc97 9325 d5ff bd25 0f6a 3ffd ede4 d266  ...%...%.j?....f
+000023b0: 3e28 5c6b 1733 030d 4799 1d9d f37c 713b  >(\k.3..G....|q;
+000023c0: eaad 423e 0c9b bcf2 44de 0e62 cb3f 0430  ..B>....D..b.?.0
+000023d0: 39f0 7de3 3d1d 94b4 6a87 4f57 fe00 504b  9.}.=...j.OW..PK
+000023e0: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
+000023f0: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
+00002400: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00002410: 372e 786d 6c75 53db 6e83 300c fd15 940f  7.xmluS.n.0.....
+00002420: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
+00002430: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
+00002440: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
+00002450: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
+00002460: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
+00002470: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
+00002480: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
+00002490: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
+000024a0: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
+000024b0: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
+000024c0: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
+000024d0: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
+000024e0: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
+000024f0: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
+00002500: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
+00002510: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
+00002520: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
+00002530: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
+00002540: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
+00002550: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
+00002560: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
+00002570: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
+00002580: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
+00002590: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
+000025a0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+000025b0: 382e 786d 6c75 53db 6e83 300c fd15 940f  8.xmluS.n.0.....
+000025c0: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
+000025d0: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
+000025e0: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
+000025f0: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
+00002600: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
+00002610: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
+00002620: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
+00002630: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
+00002640: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
+00002650: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
+00002660: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
+00002670: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
+00002680: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
+00002690: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
+000026a0: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
+000026b0: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
+000026c0: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
+000026d0: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
+000026e0: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
+000026f0: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
+00002700: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
+00002710: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
+00002720: 0304 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
+00002730: 6901 0000 0c03 0000 1900 0000 786c 2f77  i...........xl/w
+00002740: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00002750: 392e 786d 6c75 53db 6e83 300c fd15 940f  9.xmluS.n.0.....
+00002760: 68da 49bb a802 a4b5 5db5 3d4c aa5a 6d7b  h.I.....].=L.Zm{
+00002770: 0e60 4ad4 5c58 62c6 faf7 73a0 b749 f084  .`J.\Xb...s..I..
+00002780: edf8 1c1f 5f88 5beb 0ebe 02c0 e857 2be3  ...._.[......W+.
+00002790: 1356 21d6 73ce 7d5e 8116 7e62 6b30 f452  .V!.s.}^..~bk0.R
+000027a0: 5aa7 0592 ebf6 dcd7 0e44 d181 b4e2 77d3  Z........D....w.
+000027b0: e903 d742 1a96 c65d 6ce3 d2d8 36a8 a481  ...B...]l...6...
+000027c0: 8d8b 7ca3 b570 c705 28db 266c c6ce 81ad  ..|..p..(.&l....
+000027d0: dc57 d805 781a d762 0f3b c08f 9a00 e4f2  .W..x..b.;......
+000027e0: 0b4f 2135 182f ad89 1c94 097b 9ecd d73d  .O!5./.....{...=
+000027f0: a2cb f894 d0fa 1b3b 0acd 64d6 1e82 f356  .......;..d....V
+00002800: 246c 1a34 8182 1c03 85a0 cf0f 2c41 a9c0  $l.4........,A..
+00002810: 444a be4f a4ec 5a34 206f ed33 fdba eb9f  DJ.O..Z4 o.3....
+00002820: e465 c2c3 d2aa 2f59 6095 b027 1615 508a  .e..../Y`..'..P.
+00002830: 46e1 d6b6 af70 eae9 fe2a 7125 50a4 b1b3  F....p...*q%P...
+00002840: 6de4 42b3 699c 0723 94a4 4469 c290 76e8  m.B.i..#..Di..v.
+00002850: 282e a912 a6b9 7479 a384 8b39 928a 10e3  (.....ty...9....
+00002860: f909 b318 c308 ef41 67ea 3880 598e 61a4  .......Ag.8.Y.a.
+00002870: a91b 1c00 acc6 00b4 d061 c4cb 1802 8f35  .........a.....5
+00002880: 0ce4 af47 2515 ffb3 390d edbc 897e 8ae1  ...G%...9....~..
+00002890: 4ade 85db 4be3 2305 25b1 4c27 8f34 6bd7  J...K.#.%.L'.4k.
+000028a0: 8fbd 77d0 d6dd 5565 16d1 eace ace8 5ac1  ..w...Ue......Z.
+000028b0: 8504 7a2f adc5 8b13 d67e f901 d23f 504b  ..z/.....~...?PK
+000028c0: 0304 1400 0000 0800 d050 a858 19ef 2f38  .........P.X../8
+000028d0: 7b01 0000 4b03 0000 1900 0000 786c 2f77  {...K.......xl/w
+000028e0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+000028f0: 302e 786d 6c75 93db 4ec3 300c 865f a5ca  0.xmlu..N.0.._..
+00002900: 0390 81c4 41a8 adc4 364e 1748 6808 b844  ....A...6N.Hh..D
+00002910: 59eb ae11 3914 c7a5 8ca7 c7e9 8e48 ed55  Y...9........H.U
+00002920: 6dc7 9ff3 3b76 d3ce e367 a801 28f9 b1c6  m...;v...g..(...
+00002930: 854c d444 cdb5 94a1 a8c1 aa70 e21b 707c  .L.D.......p..p|
+00002940: 5279 b48a d8c5 950c 0d82 2a7b c81a 7936  Ry........*{..y6
+00002950: 995c 48ab b413 79da c79e 314f 7d4b 463b  .\H...y...1O}KF;
+00002960: 78c6 24b4 d62a 5c4f c1f8 2e13 a762 1758  x.$..*\O.....b.X
+00002970: e855 4d7d 40e6 69a3 56f0 02f4 da30 c0ae  .UM}@.i.V....0..
+00002980: dcd7 29b5 0517 b477 0942 9589 9bd3 ebfb  ..)....w.B......
+00002990: 0dd1 67bc 69e8 c291 9dc4 6696 de7f 46e7  ..g.i.....f...F.
+000029a0: b1cc c424 6a02 0305 c512 8a3f df30 0363  ...$j......?.0.c
+000029b0: 6225 56f2 b52d 2a0e 9746 f2d8 de95 bfeb  b%V..-*..F......
+000029c0: fb67 794b 1560 e6cd bb2e a9ce c495 484a  .gyK.`........HJ
+000029d0: a854 6b68 e1bb 07d8 f674 7e90 3857 a4f2  .Tkh.....t~.8W..
+000029e0: 147d 9760 6c36 4f8b 68c4 2b39 51bb f848  .}.`l6O.h.+9Q..H
+000029f0: 2f84 1cd7 7c13 e508 8150 f772 3fc0 fdae  /...|....P.r?...
+00002a00: 2d84 5412 0b8a c7b2 d8e2 d331 bcd0 58b4  -.T........1..X.
+00002a10: 46e1 0033 1b63 5408 6097 663d c0cc c718  F..3.cT.`.f=....
+00002a20: ed9a 9606 80db 3180 f761 98b8 1b23 68dd  ......1..a...#h.
+00002a30: c040 fefd a8a4 f27f b6e4 37df 0d72 3384  .@........7..r3.
+00002a40: b864 4f0a 57da 85c4 40c5 5526 2797 3c2a  .dO.W...@.U&'.<*
+00002a50: dc4c 6de3 906f faa5 5c7a 226f 7bb3 e665  .Lm..o..\z"o{..e
+00002a60: 078c 097c 5e79 4f7b 276e cdfe ffc9 ff00  ...|^yO{'n......
+00002a70: 504b 0304 1400 0000 0800 d050 a858 caac  PK.........P.X..
+00002a80: fec0 7101 0000 3e03 0000 1900 0000 786c  ..q...>.......xl
+00002a90: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00002aa0: 7432 312e 786d 6c75 93db 6e83 300c 407f  t21.xmlu..n.0.@.
+00002ab0: 05e5 039a 76d2 2eaa 0069 6dd7 6e0f 93aa  ....v....im.n...
+00002ac0: 56db 9e53 3010 3517 9698 b1fe fd1c 7a9d  V..S0.5.......z.
+00002ad0: 044f d88e 8fef c4ad 757b 5f01 60f4 ab95  .O......u{_.`...
+00002ae0: f109 ab10 eb29 e73e ab40 0b3f b235 187a  .....).>.@.?.5.z
+00002af0: 29ac d302 4975 25f7 b503 9177 9056 fc6e  )...Iu%....w.V.n
+00002b00: 3c7e e05a 48c3 d2b8 b3ad 5d1a db06 9534  <~.ZH.....]....4
+00002b10: b076 916f b416 ee30 0365 db84 4dd8 d9b0  .v.o...0.e..M...
+00002b20: 9165 859d 81a7 712d 4ad8 027e d404 90ca  .e....q-J..~....
+00002b30: 2f71 72a9 c178 694d e4a0 48d8 f364 ba3a  /qr..xiM..H..d.:
+00002b40: 129d c7a7 84d6 dfc8 5168 6667 ed3e 286f  ........Qhfg.>(o
+00002b50: 79c2 c6a1 2650 9061 0821 e8f3 0373 502a  y...&P.a.!...sP*
+00002b60: 44a2 4abe 4f41 d935 6920 6fe5 73f8 65d7  D.J.OA.5i o.s.e.
+00002b70: 3f95 b713 1ee6 567d c91c ab84 3db1 2887  ?.....V}....=.(.
+00002b80: 4234 0a37 b67d 8553 4ff7 d712 1702 451a  B4.7.}.SO.....E.
+00002b90: 3bdb 462e 349b c659 1042 4a72 9426 0c69  ;.F.4..Y.BJr.&.i
+00002ba0: 8b8e ec92 3261 5a36 3207 1f73 a41a 8285  ....2aZ62..s....
+00002bb0: 6727 6236 4464 d265 8d12 ae87 990f 31c2  g'b6Dd.e......1.
+00002bc0: 7bd0 3b75 e861 1643 8c34 7583 3dc0 cb10  {.;u.a.C.4u.=...
+00002bd0: 4027 d04f 2c87 083c d4d0 e3bf 1a2c 29ff  @'.O,..<.....,).
+00002be0: efcd 69cc e7dd 1de7 1eee ea5d b852 1a1f  ..i........].R..
+00002bf0: 2928 28ca 78f4 48db 71c7 451d 15b4 7577  )((.x.H.q.E...uw
+00002c00: 873b 8b68 7527 5674 dfe0 8203 bd17 d6e2  .;.hu'Vt........
+00002c10: 4509 8772 f965 d23f 504b 0304 1400 0000  E..r.e.?PK......
+00002c20: 0800 d050 a858 2513 3651 8301 0000 5703  ...P.X%.6Q....W.
+00002c30: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00002c40: 6574 732f 7368 6565 7432 322e 786d 6c75  ets/sheet22.xmlu
+00002c50: 53db 6edb 300c fd15 431f 50a5 1bba 0d85  S.n.0...C.P.....
+00002c60: 6d60 4d2f dbc3 80a2 c5b6 c740 b169 5b88  m`M/.......@.i[.
+00002c70: 246a 145d af7f 3fca b9b4 03e2 2793 14cf  $j.]..?.....'...
+00002c80: e1e1 c5e5 84b4 4b03 0017 7fbd 0ba9 5203  ......K.......R.
+00002c90: 73bc d63a 3503 7893 2e30 4290 970e c91b  s..:5.x..0B.....
+00002ca0: 1697 7a9d 2281 6967 9077 fac3 6af5 497b  ..z.".ig.w..j.I{
+00002cb0: 6383 aacb 39f6 4875 8923 3b1b e091 8a34  c...9.Hu.#;....4
+00002cc0: 7a6f e8f5 061c 4e95 ba54 c7c0 93ed 079e  zo....N..T......
+00002cd0: 03ba 2ea3 e9e1 19f8 6714 80b8 fac4 d35a  ........g......Z
+00002ce0: 0f21 590c 0541 57a9 af97 d70f 7bc4 9cf1  .!Y..AW.....{...
+00002cf0: cbc2 94de d945 6e66 8bb8 cbce f7b6 52ab  .....Enf......R.
+00002d00: ac09 1c34 9c29 8c7c 5e60 0dce 6526 51f2  ...4.).|^`..e&Q.
+00002d10: e740 aade 8a66 e47b fb48 7f3f f72f f2b6  .@...f.{.H.?./..
+00002d20: 26c1 1add 6fdb f250 a92f aa68 a133 a3e3  &...o..P./.h.3..
+00002d30: 279c bec1 a1a7 ab37 89b7 864d 5d12 4e05  '......7...M].N.
+00002d40: e566 ebb2 c946 2e29 8936 e421 3d33 49dc  .f...F.).6.!=3I.
+00002d50: 4a25 aef1 0568 30a1 df34 649b dde6 6324  J%...h0..4d...c$
+00002d60: 1940 a959 24e5 04dd 1c08 6e96 0864 4f93  .@.Y$.....n..dO.
+00002d70: a176 83ce f678 06b8 5e02 1248 e904 8bc0  .v...x..^..H....
+00002d80: db25 a00d 71e4 3380 bbc5 1e47 3e8f b85f  .%..q.3....G>.._
+00002d90: 42f0 6b3c 3784 8745 49ed ffd9 5ae6 7f5c  B.k<7..EI...Z..\
+00002da0: ea7e 21f9 e07e 18ea 6d48 8583 4e58 5617  .~!..~..mH..NXV.
+00002db0: 9f65 6db4 dfe0 de61 8cf3 816e 9119 fd6c  .em....a...n...l
+00002dc0: 0e72 f840 3941 de3b 443e 39f9 824e ff52  .r.@9A.;D>9..N.R
+00002dd0: fd0f 504b 0304 1400 0000 0800 d050 a858  ..PK.........P.X
+00002de0: a50c 764f 5301 0000 a402 0000 1900 0000  ..vOS...........
+00002df0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00002e00: 6565 7432 332e 786d 6c75 52db 6ac3 300c  eet23.xmluR.j.0.
+00002e10: fd95 e00f a8d3 c12e 9424 b0b6 8ced 6150  .........$....aP
+00002e20: 5ab6 3dbb 8992 98fa 365b 59d6 bf9f 9cf4  Z.=.....6[Y.....
+00002e30: 3668 9f2c c93a 47e7 c8ce 7aeb 77a1 05c0  6h.,.:G...z.w...
+00002e40: e457 2b13 72d6 22ba 19e7 a16c 418b 30b1  .W+.r."....lA.0.
+00002e50: 0e0c ddd4 d66b 8194 fa86 07e7 4154 0348  .....k......AT.H
+00002e60: 2b7e 97a6 0f5c 0b69 5891 0db5 952f 32db  +~...\.iX..../2.
+00002e70: a192 0656 3e09 9dd6 c2ef e7a0 6c9f b329  ...V>.......l..)
+00002e80: 3b16 d6b2 6971 28f0 2273 a281 0de0 8723  ;...iq(."s.....#
+00002e90: 00a5 fcc4 5349 0d26 486b 120f 75ce 9ea7  ....SI.&Hk..u...
+00002ea0: b3e5 8818 3a3e 25f4 e122 4ea2 99ad b5bb  ....:>%.."N.....
+00002eb0: 98bc 5539 4ba3 2650 5062 a410 74fc c002  ..U9K.&PPb..t...
+00002ec0: 948a 4ca4 e4fb 40ca ce43 23f2 323e d2bf  ..L...@..C#.2>..
+00002ed0: 0cfe 49de 5604 5858 f525 2b6c 73f6 c492  ..I.V.XX.%+ls...
+00002ee0: 0a6a d129 5cdb fe15 0e9e eecf 1297 0245  .j.)\..........E
+00002ef0: 9179 db27 3e9a 2db2 3206 7124 354a 1397  .y.'>.-.2.q$5J..
+00002f00: b441 4f75 4993 b090 c675 9871 2409 b1c0  .AOuI....u.q$...
+00002f10: cb03 607e 0b40 8bbe 8e58 dc42 e0de c195  ..`~.@...X.B....
+00002f20: fee5 4d49 d5ff 6e4e 668e 1b1a ddc5 d77b  ..MI..nNf......{
+00002f30: 17be 9126 240a 6a62 4927 8fb4 033f ae63  ...&$.jbI'...?.c
+00002f40: 4cd0 bae1 b5b7 16d1 ea21 6ce9 1781 8f0d  L........!l.....
+00002f50: 745f 5b8b a724 3ec7 e963 167f 504b 0304  t_[..$>..c..PK..
+00002f60: 1400 0000 0800 d050 a858 6517 5607 5c01  .......P.Xe.V.\.
+00002f70: 0000 b502 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
+00002f80: 6b73 6865 6574 732f 7368 6565 7432 342e  ksheets/sheet24.
+00002f90: 786d 6c75 52db 4ec3 300c fd95 2a1f b06c  xmluR.N.0...*..l
+00002fa0: 485c 84da 4ab0 09c1 03d2 0402 9eb3 d65d  H\..J..........]
+00002fb0: 2392 b873 5c0a 7f8f d35d 91d8 536c 27e7  #..s\....]..Sl'.
+00002fc0: d8e7 38f9 80f4 195b 00ce bebd 0bb1 502d  ..8....[......P-
+00002fd0: 7377 ab75 ac5a f026 4eb0 8320 370d 9237  sw.u.Z.&N.. 7..7
+00002fe0: 2c29 ad75 ec08 4c3d 82bc d317 d3e9 95f6  ,).u..L=........
+00002ff0: c606 55e6 636d 4965 8e3d 3b1b 6049 59ec  ..U.cmIe.=;.`IY.
+00003000: bd37 f473 0f0e 8742 cdd4 bef0 62d7 2d8f  .7.s...B....b.-.
+00003010: 055d e69d 59c3 2bf0 5b27 0049 f581 a7b6  .]..Y.+.['.I....
+00003020: 1e42 b418 3282 a650 77b3 dbc5 1631 be78  .B..2..Pw....1.x
+00003030: b730 c493 384b 6256 889f 2979 aa0b 354d  .0..8KbV..)y..5M
+00003040: 3381 838a 1385 91e3 0be6 e05c 6292 4936  3..........\b.I6
+00003050: 3b52 756c 9a90 a7f1 9efe 61d4 2fe3 ad4c  ;Rul......a./..L
+00003060: 8439 ba0f 5b73 5ba8 1b95 d5d0 98de f10b  .9..[s[.........
+00003070: 0e8f b0d3 7479 1c71 61d8 9439 e190 5112  ....ty.qa..9..Q.
+00003080: 5be6 550a 524b 7968 4332 e995 49ea 563a  [.U.RKyhC2..I.V:
+00003090: 7119 61d3 43a8 20e6 9a65 8c54 d4d5 0e74  q.a.C. ..e.T...t
+000030a0: 7f16 843d fd0f 999f 8374 24c6 d27f 90c5  ...=.....t$.....
+000030b0: 3948 0db1 22db 2527 ffc2 b4a8 db5b b695  9H..".%'.....[..
+000030c0: 9bd6 f96c 686d 43cc 1c34 4237 9d5c 8b29  ...lhmC..4B7.\.)
+000030d0: b4f5 679b 3076 e3fa 57c8 8c7e 0c5b f956  ..g.0v..W..~.[.V
+000030e0: 40e9 81dc 3788 7c48 d27e 0e3f b5fc 0550  @...7.|H.~.?...P
+000030f0: 4b03 0414 0000 0008 00d0 50a8 58d2 05f1  K.........P.X...
+00003100: 4652 0200 0047 0a00 000d 0000 0078 6c2f  FR...G.......xl/
+00003110: 7374 796c 6573 2e78 6d6c dd56 db8a db30  styles.xml.V...0
+00003120: 10fd 15e3 0fa8 9398 9ab8 2479 a821 5068  ..........$y.!Ph
+00003130: cbc2 ee43 5fe5 584e 04ba b8b2 bc24 fdfa  ...C_.XN.....$..
+00003140: 6a24 e7b6 9be3 52fa 569b e099 393a 3367  j$....R.V...9:3g
+00003150: a431 ceaa 7727 c99f 0f9c bbe4 a8a4 eed7  .1..w'..........
+00003160: e9c1 b9ee 5396 f5bb 0357 acff 603a ae3d  ....S....W..`:.=
+00003170: d21a ab98 f3ae dd67 7d67 396b 7a22 2999  .......g}g9kz").
+00003180: 2d66 b322 534c e874 b3d2 83da 2ad7 273b  -f."SL.t....*.';
+00003190: 3368 b74e 6769 926d 56ad d1d7 d03c 8d01  3h.Ngi.mV....<..
+000031a0: bf96 299e bc32 b94e 2b26 456d 455c cc94  ..)..2.N+&EmE\..
+000031b0: 90a7 185f 84c8 ce48 6313 e7d5 70a2 53a8  ..._...Hc...p.S.
+000031c0: ff15 17cc 4797 a48e b994 d0c6 8668 16cb  ....G........h..
+000031d0: 8447 ef13 0b29 2f2a 1669 0c6c 561d 738e  .G...)/*.i.lV.s.
+000031e0: 5bbd f54e 2485 e87b 6cb4 5f4e 9d57 b1b7  [..N$..{l._N.W..
+000031f0: ec34 5f7c 4c6f 18e1 e1cb d4c6 36dc deb5  .4_|Lo......6...
+00003200: 1b43 9b95 e4ad 2386 15fb 4330 9ce9 e851  .C....#...C0...Q
+00003210: 1be7 8c22 ab11 6c6f 348b 4ace b4d1 f0b9  ..."..lo4.J.....
+00003220: 775c ca67 3aaf 1fed 5d81 639b c48d ffd2  w\.g:...].c.....
+00003230: 843d a78e cfa6 5735 9a31 cde8 5081 db74  .=....W5.1..P..t
+00003240: 31f9 bfe7 edc4 ab71 9f07 df90 0efe cfc1  1......q........
+00003250: 38fe 6479 2b8e c13f b66f 045c 6a07 2577  8.dy+..?.o.\j.%w
+00003260: e52f d184 4665 9d7e a711 9437 39ea 4148  ./..Fe.~...79.AH
+00003270: 27f4 e81d 44d3 70fd be3b 9fdf b1da 0ff9  '...D.p..;......
+00003280: 5d01 bfaa e12d 1ba4 7bb9 80eb f46a 7fe3  ]....-..{....j..
+00003290: 8d18 5479 59f5 448d 8dab aef6 573a ca79  ..TyY.D.....W:.y
+000032a0: 719d 535f 4ce8 861f 7953 8dae ddd7 c14c  q.S_L...yS.....L
+000032b0: bce1 cb8e 5760 bc85 b6e1 0210 6445 1040  ....W`......dE.@
+000032c0: 04c2 5a50 0664 451e acf5 3ff6 b5c4 7d45  ..ZP.dE...?...}E
+000032d0: 102a 5c3e 8696 98b5 c4ac c87b 0855 e186  .*\>.......{.U..
+000032e0: b500 abf4 1768 b92c f3bc 28e0 f656 d563  .....h.,..(..V.c
+000032f0: 1915 dcc3 a2a0 1f48 0815 1207 d6a2 6a7f  .......H......j.
+00003300: bbf3 1303 3031 367f 980d 78ca 9363 035b  ....016...x..c.[
+00003310: 9e18 51d8 f2c4 ce13 04f6 9038 6509 0600  ..Q........8e...
+00003320: d622 0e3c 1438 5124 02d4 a251 03ac 3ca7  .".<.8Q$...Q..<.
+00003330: 7386 0ae1 6b3e 0195 2584 6848 c1f4 1605  s...k>..%.hH....
+00003340: daa8 826e 705e f025 caf3 b204 1081 4046  ...np^.%......@F
+00003350: 9e43 885e d809 08ca 2021 10ca f3f8 217d  .C.^.... !....!}
+00003360: f33d cbce dfb9 ecfa d771 f31b 504b 0304  .=.......q..PK..
+00003370: 1400 0000 0800 d050 a858 b747 eb8a c000  .......P.X.G....
+00003380: 0000 1602 0000 0b00 0000 5f72 656c 732f  .........._rels/
+00003390: 2e72 656c 739d 924b 6e02 310c 40af 1265  .rels..Kn.1.@..e
+000033a0: 5f4c a9c4 0231 acd8 b043 880b b889 e7a3  _L...1...C......
+000033b0: 99c4 9163 c4f4 f68d d8c0 2068 114b ff9e  ...c...... h.K..
+000033c0: 9e2d af0f 34a0 761c 73db a56c c630 c45c  .-..4.v.s..l.0.\
+000033d0: d956 35ad 00b2 6b29 609e 71a2 582a 354b  .V5...k)`.q.X*5K
+000033e0: 402d a134 90d0 f5d8 102c e6f3 25c8 2dc3  @-.4.....,..%.-.
+000033f0: 6ed6 b74c 73fc 49f4 0a91 ebba 73b4 6577  n..Ls.I.....s.ew
+00003400: 0a14 f501 f8ae c39a 234a 435a d971 8033  ........#JCZ.q.3
+00003410: 4bff cddc cf0a d49a 9daf acec fca7 35f0  K.............5.
+00003420: a6cc f3f5 2090 a247 4570 2cf4 91a4 4c8b  .... ..GEp,...L.
+00003430: 7694 af3e 9edd bea4 f3a5 6362 b478 dfe8  v..>......cb.x..
+00003440: fff3 d0a8 143d f9bf 9d30 a589 d2d7 4509  .....=...0....E.
+00003450: 266f b0f9 0550 4b03 0414 0000 0008 00d0  &o...PK.........
+00003460: 50a8 58dc 9a46 7c94 0200 000f 0900 000f  P.X..F|.........
+00003470: 0000 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
+00003480: 6d6c 8d96 6f53 a330 10c6 bf4a 870f 7014  ml..oS.0...J..p.
+00003490: d4fa 67ac 334e f5b4 37de d929 3ddf 07b2  ..g.3N..7..)=...
+000034a0: a53b 2659 2e09 2afd f417 60aa 78c1 ccbd  .;&Y..*...`.x...
+000034b0: 29cd 86fd b11b 9e27 e1f2 95f4 734e f43c  )......'....sN.<
+000034c0: 7993 4299 0b3d 8f76 d656 1771 6c8a 1d48  y.B..=.v.V.ql..H
+000034d0: 66be 5105 cacd 6d49 4b66 dd50 9731 6db7  f.Q...mIKf.P.1m.
+000034e0: 58c0 0d15 b504 65e3 743a 9dc5 1a04 b348  X.....e.t:.....H
+000034f0: caec b032 514f fb1f 96a9 3430 6e76 0056  ...2QO....40nv.V
+00003500: 8a1e 2519 aae8 eaf2 50d9 4a4f e2e1 882c  ..%.....P.JO...,
+00003510: 14ed 93da 681b 7942 7835 1f37 b4c3 c90b  ....h.yBx5.7....
+00003520: 1acc 51a0 6de6 51f7 5f40 3491 a850 e21e  ..Q.m.Q._@4..P..
+00003530: f83c 9a46 13b3 a3d7 7bd2 b827 6599 c80a  .<.F....{..'e...
+00003540: 4d42 cca3 a49f 7802 6db1 f0c2 595b e686  MB....x.m...Y[..
+00003550: e5a6 8b58 96af db9e e7d1 6cea 805b d4c6  ...X......l..[..
+00003560: 7677 747c e68a 7c01 7773 3faa 2d7d 4761  vwt|..|.ws?.-}Ga
+00003570: 41df 300b 779a ea0a 55d9 615c 1bf1 a08f  A.0.w...U.a\....
+00003580: 6e29 0ed7 8962 12e6 d12f f7cb 373b 97d1  n)...b.../..7;..
+00003590: d6e1 e24b ded7 641d 6cd0 a1be 4037 a197  ...K..d.l...@7..
+000035a0: bcc7 0e11 1b78 b3ae 00c8 e04f 0daa 8001  .....x.....O....
+000035b0: 280d 8052 0fb4 d228 410f d28f 02e9 475e  (..R...(A.....G^
+000035c0: fae1 f98b da0e 18c7 01c6 b1c7 5883 b11a  ............X...
+000035d0: 3b11 8ce3 4e02 b813 0ff7 93a9 9a09 d16c  ;...N..........l
+000035e0: 9a0a 7846 b5fe b43a b300 6be6 b17e 5782  ..xF...:..k..~W.
+000035f0: 1807 de2d f5bf a8d3 00ea 74a4 cb8a 0c5a  ...-......t....Z
+00003600: d2cd d2af ea2c 803a f350 d79c df81 8211  .....,.:.P......
+00003610: ce79 8073 ee71 1c84 242c 8834 47e5 b28c  .y.s.q..$,.4G...
+00003620: c74b a621 554e 4372 f059 4185 fb12 1fc8  .K.!UNCr.YA.....
+00003630: e256 ed1b 0937 58ba 50ab 120f 1dd2 7ce2  .V...7X.P.....|.
+00003640: 8b3e 4359 7d78 e781 8a6e af1b 0243 2e48  .>CY}x...n...C.H
+00003650: 7c1b 5c1b 0332 17cd 0fc2 4f98 9011 12df  |.\..2....O.....
+00003660: 0907 8cdf 60c8 0289 ef81 d562 ed33 42d2  ....`......b.3B.
+00003670: 4f7c ed3f 60c9 c657 3b24 fcc4 57fe 3d49  O|.?`..W;$..W.=I
+00003680: 1254 526d d650 90cc 5bad 8d72 432e 487c  .TRm.P..[..rC.H|
+00003690: 1bdc 616e 487d bd66 2133 24be 1b06 7abb  ..anH}.f!3$...z.
+000036a0: 56fc cbee d390 2552 df12 8bf5 325b f96f  V.....%R....2[.o
+000036b0: 230d b921 f5dd f028 b0a4 fb26 d7c8 71ff  #..!...(...&..q.
+000036c0: 4565 c19d 7f64 eb27 e15c a599 81db 370b  Ee...d.'.\....7.
+000036d0: ca8c 3243 4648 7d23 2c04 2977 ae65 56bb  ..2CFH}#,.)w.eV.
+000036e0: 9cb2 1992 425e 487b 2fc4 87d3 92c3 1615  ....B^H{/.......
+000036f0: f0f6 a034 ed84 3bbb 0bf7 e1d0 5e7a bf1f  ...4..;.....^z..
+00003700: 9fb4 6f70 5b0b b170 b147 f5e0 b6e9 f7e3  ..op[..p.G......
+00003710: f7f0 ed70 f517 504b 0304 1400 0000 0800  ...p..PK........
+00003720: d050 a858 7296 7e91 3701 0000 390f 0000  .P.Xr.~.7...9...
+00003730: 1a00 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00003740: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 cdd7  kbook.xml.rels..
+00003750: 418e 8230 14c6 f1ab 901e c0f2 aaa2 4ec4  A..0..........N.
+00003760: 951b b713 2fd0 e013 8840 49db c9e8 ed87  ..../....@I.....
+00003770: c802 3f32 8bd9 9879 2bd2 121e ff45 f30b  ..?2...y+....E..
+00003780: ec3f b9b1 b176 5da8 ea3e 24f7 b6e9 42ae  .?...v]..>$...B.
+00003790: aa18 fb0f ad43 5171 6bc3 c2f5 dc0d 77ae  .....CQqk.....w.
+000037a0: ceb7 360e 4b5f eade 1637 5bb2 3669 9a69  ..6.K_...7[.6i.i
+000037b0: ff3a 431d f6af 3393 f3a3 e7bf 4c74 d76b  .:C...3.....Lt.k
+000037c0: 5df0 d115 5f2d 77f1 97c1 fadb f95b a898  ]..._-w......[..
+000037d0: a34a ced6 971c 73a5 efcd b41d f4f3 428b  .J....s.......B.
+000037e0: 61b2 4a4e 975c f9d3 8554 a2ff bbc8 4091  a.JN.\...T....@.
+000037f0: 1150 b484 a2a5 80a2 1514 ad04 14ad a168  .P.............h
+00003800: 2da0 2883 a24c 40d1 068a 3602 8ab6 50b4  -.(..L@...6...P.
+00003810: 1550 b483 a29d 8022 4a91 c854 42d3 8c6d  .P....."J..TB..m
+00003820: 096e 13c2 4d12 e426 a49b 24d8 4d88 3749  .n..M..&..$.M.7I
+00003830: d09b 906f 92e0 3721 e024 4170 42c2 4982  ...o..7!.$ApB.I.
+00003840: e184 8893 04c5 0919 2709 8e1b 74dc 4870  ........'...t.Hp
+00003850: dca0 e346 82e3 66f6 012e c171 838e 1b09  ...F..f....q....
+00003860: 8e1b 74dc bcd5 f110 1f0d 8729 685c 63c0  ..t........)h\c.
+00003870: 5bd1 8ec3 b33c bdff b91c 3767 4778 645a  [....<....7gGxdZ
+00003880: c39f f2e1 0750 4b03 0414 0000 0008 00d0  .....PK.........
+00003890: 50a8 588b 1ae4 a471 0100 0035 1000 0013  P.X....q...5....
+000038a0: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
+000038b0: 735d 2e78 6d6c cd98 cb6e c230 1045 7f25  s].xml...n.0.E.%
+000038c0: ca16 1163 b7a5 0f01 9bb6 db96 457f c04d  ...c........E..M
+000038d0: 26c4 c22f 790c 85bf af13 0a52 2bca 4354  &../y......R+.CT
+000038e0: ea6c 6225 9eb9 f7c6 231d 2919 bdad 3d60  .lb%....#.)...=`
+000038f0: b632 dae2 386f 62f4 0f8c 61d9 8091 5838  .2..8ob...a...X8
+00003900: 0f36 edd4 2e18 19d3 6d98 312f cbb9 9c01  .6......m.1/....
+00003910: 1383 c190 95ce 46b0 b11f 5b8d 7c32 7a82  ......F...[.|2z.
+00003920: 5a2e 74cc 9e57 e931 2a67 c779 008d 79f6  Z.t..W.1*g.y..y.
+00003930: b829 6cbd c6b9 f45e ab52 c6b4 cf96 b6fa  .)l....^.R......
+00003940: e1d2 ff72 2852 6757 838d f2d8 4b05 79c6  ...r(RgW....K.y.
+00003950: f65a 745b bf3a 6c1b 5f97 1082 aa20 9bca  .Zt[.:l._.... ..
+00003960: 105f a449 656c a519 c6b5 062c 0e6b ec49  ._.Iel.....,.k.I
+00003970: e9ea 5a95 50b9 7261 524b 813e 80ac b001  ..Z.P.raRK.>....
+00003980: 8846 171b d1de 11eb 980e 1936 577e 7180  .F.........6W~q.
+00003990: 4ee6 a063 2a9d 06e7 314d 2dc0 f97e dbb1  N..c*...1M-..~..
+000039a0: b4dd 7d9f 8420 4475 e425 7796 49fb e237  ..}.. Du.%w.I..7
+000039b0: 8476 e215 54a7 9aa7 13fe 7061 decd 0459  .v..T.....pa...Y
+000039c0: b75c 7ecc dfe7 bcd3 3f37 88a0 12e4 8a4a  .\~.....?7.....J
+000039d0: 906b 2a41 6ea8 0419 5209 724b 25c8 1d95  .k*An...R.rK%...
+000039e0: 20f7 5482 f001 9924 64d8 cac9 c095 93a1   .T....$d.......
+000039f0: 2b27 8357 4e86 af9c 0c60 3919 c272 3288  +'.WN....`9..r2.
+00003a00: e564 182b c830 5690 61ac 20c3 5841 86b1  .d.+.0V.a. .XA..
+00003a10: e25f 19fb eedc fcaf bf62 dbb5 3052 d95d  ._.......b..0R.]
+00003a20: 00d6 fd2d 987c 0250 4b01 0214 0314 0000  ...-.|.PK.......
+00003a30: 0008 00d0 50a8 5846 5ac1 0c82 0000 00b1  ....P.XFZ.......
+00003a40: 0000 0010 0000 0000 0000 0000 0000 0080  ................
+00003a50: 0100 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
+00003a60: 702e 786d 6c50 4b01 0214 0314 0000 0008  p.xmlPK.........
+00003a70: 00d0 50a8 5815 0f74 b6ee 0000 00cb 0100  ..P.X..t........
+00003a80: 0011 0000 0000 0000 0000 0000 0080 01b0  ................
+00003a90: 0000 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
+00003aa0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00003ab0: d050 a858 995c 9c23 1006 0000 9c27 0000  .P.X.\.#.....'..
+00003ac0: 1300 0000 0000 0000 0000 0000 8001 cd01  ................
+00003ad0: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00003ae0: 312e 786d 6c50 4b01 0214 0314 0000 0008  1.xmlPK.........
+00003af0: 00d0 50a8 58bb e88b 3838 0100 0011 0200  ..P.X...88......
+00003b00: 0018 0000 0000 0000 0000 0000 0080 810e  ................
+00003b10: 0800 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00003b20: 2f73 6865 6574 312e 786d 6c50 4b01 0214  /sheet1.xmlPK...
+00003b30: 0314 0000 0008 00d0 50a8 5807 12de aaee  ........P.X.....
+00003b40: 0100 0021 0400 0018 0000 0000 0000 0000  ...!............
+00003b50: 0000 0080 817c 0900 0078 6c2f 776f 726b  .....|...xl/work
+00003b60: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
+00003b70: 6c50 4b01 0214 0314 0000 0008 00d0 50a8  lPK...........P.
+00003b80: 58a4 976e 8956 0100 00a5 0200 0018 0000  X..n.V..........
+00003b90: 0000 0000 0000 0000 0080 81a0 0b00 0078  ...............x
+00003ba0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00003bb0: 6574 332e 786d 6c50 4b01 0214 0314 0000  et3.xmlPK.......
+00003bc0: 0008 00d0 50a8 5832 c066 ed4c 0100 004d  ....P.X2.f.L...M
+00003bd0: 0200 0018 0000 0000 0000 0000 0000 0080  ................
+00003be0: 812c 0d00 0078 6c2f 776f 726b 7368 6565  .,...xl/workshee
+00003bf0: 7473 2f73 6865 6574 342e 786d 6c50 4b01  ts/sheet4.xmlPK.
+00003c00: 0214 0314 0000 0008 00d0 50a8 5808 4026  ..........P.X.@&
+00003c10: f85c 0100 008b 0200 0018 0000 0000 0000  .\..............
+00003c20: 0000 0000 0080 81ae 0e00 0078 6c2f 776f  ...........xl/wo
+00003c30: 726b 7368 6565 7473 2f73 6865 6574 352e  rksheets/sheet5.
+00003c40: 786d 6c50 4b01 0214 0314 0000 0008 00d0  xmlPK...........
+00003c50: 50a8 584e c75d 808a 0100 0091 0300 0018  P.XN.]..........
+00003c60: 0000 0000 0000 0000 0000 0080 8140 1000  .............@..
+00003c70: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00003c80: 6865 6574 362e 786d 6c50 4b01 0214 0314  heet6.xmlPK.....
+00003c90: 0000 0008 00d0 50a8 5844 0990 06e7 0100  ......P.XD......
+00003ca0: 0037 0400 0018 0000 0000 0000 0000 0000  .7..............
+00003cb0: 0080 8100 1200 0078 6c2f 776f 726b 7368  .......xl/worksh
+00003cc0: 6565 7473 2f73 6865 6574 372e 786d 6c50  eets/sheet7.xmlP
+00003cd0: 4b01 0214 0314 0000 0008 00d0 50a8 5891  K...........P.X.
+00003ce0: c100 8bd2 0100 00f6 0300 0018 0000 0000  ................
+00003cf0: 0000 0000 0000 0080 811d 1400 0078 6c2f  .............xl/
+00003d00: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00003d10: 382e 786d 6c50 4b01 0214 0314 0000 0008  8.xmlPK.........
+00003d20: 00d0 50a8 58d3 d762 9c0b 0200 0031 0500  ..P.X..b.....1..
+00003d30: 0018 0000 0000 0000 0000 0000 0080 8125  ...............%
+00003d40: 1600 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00003d50: 2f73 6865 6574 392e 786d 6c50 4b01 0214  /sheet9.xmlPK...
+00003d60: 0314 0000 0008 00d0 50a8 581a 828f 869c  ........P.X.....
+00003d70: 0100 001a 0400 0019 0000 0000 0000 0000  ................
+00003d80: 0000 0080 8166 1800 0078 6c2f 776f 726b  .....f...xl/work
+00003d90: 7368 6565 7473 2f73 6865 6574 3130 2e78  sheets/sheet10.x
+00003da0: 6d6c 504b 0102 1403 1400 0000 0800 d050  mlPK...........P
+00003db0: a858 82b2 f49d 6701 0000 0f03 0000 1900  .X....g.........
+00003dc0: 0000 0000 0000 0000 0000 8081 391a 0000  ............9...
+00003dd0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00003de0: 6565 7431 312e 786d 6c50 4b01 0214 0314  eet11.xmlPK.....
+00003df0: 0000 0008 00d0 50a8 5882 b2f4 9d67 0100  ......P.X....g..
+00003e00: 000f 0300 0019 0000 0000 0000 0000 0000  ................
+00003e10: 0080 81d7 1b00 0078 6c2f 776f 726b 7368  .......xl/worksh
+00003e20: 6565 7473 2f73 6865 6574 3132 2e78 6d6c  eets/sheet12.xml
+00003e30: 504b 0102 1403 1400 0000 0800 d050 a858  PK...........P.X
+00003e40: fbc7 128d 4a01 0000 7502 0000 1900 0000  ....J...u.......
+00003e50: 0000 0000 0000 0000 8081 751d 0000 786c  ..........u...xl
+00003e60: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00003e70: 7431 332e 786d 6c50 4b01 0214 0314 0000  t13.xmlPK.......
+00003e80: 0008 00d0 50a8 5827 517b 715a 0100 00c9  ....P.X'Q{qZ....
+00003e90: 0200 0019 0000 0000 0000 0000 0000 0080  ................
+00003ea0: 81f6 1e00 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00003eb0: 7473 2f73 6865 6574 3134 2e78 6d6c 504b  ts/sheet14.xmlPK
+00003ec0: 0102 1403 1400 0000 0800 d050 a858 44ff  ...........P.XD.
+00003ed0: 8108 6901 0000 0c03 0000 1900 0000 0000  ..i.............
+00003ee0: 0000 0000 0000 8081 8720 0000 786c 2f77  ......... ..xl/w
+00003ef0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00003f00: 352e 786d 6c50 4b01 0214 0314 0000 0008  5.xmlPK.........
+00003f10: 00d0 50a8 5811 26ee aa80 0100 0080 0300  ..P.X.&.........
+00003f20: 0019 0000 0000 0000 0000 0000 0080 8127  ...............'
+00003f30: 2200 0078 6c2f 776f 726b 7368 6565 7473  "..xl/worksheets
+00003f40: 2f73 6865 6574 3136 2e78 6d6c 504b 0102  /sheet16.xmlPK..
+00003f50: 1403 1400 0000 0800 d050 a858 44ff 8108  .........P.XD...
+00003f60: 6901 0000 0c03 0000 1900 0000 0000 0000  i...............
+00003f70: 0000 0000 8081 de23 0000 786c 2f77 6f72  .......#..xl/wor
+00003f80: 6b73 6865 6574 732f 7368 6565 7431 372e  ksheets/sheet17.
+00003f90: 786d 6c50 4b01 0214 0314 0000 0008 00d0  xmlPK...........
+00003fa0: 50a8 5844 ff81 0869 0100 000c 0300 0019  P.XD...i........
+00003fb0: 0000 0000 0000 0000 0000 0080 817e 2500  .............~%.
+00003fc0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00003fd0: 6865 6574 3138 2e78 6d6c 504b 0102 1403  heet18.xmlPK....
+00003fe0: 1400 0000 0800 d050 a858 44ff 8108 6901  .......P.XD...i.
+00003ff0: 0000 0c03 0000 1900 0000 0000 0000 0000  ................
+00004000: 0000 8081 1e27 0000 786c 2f77 6f72 6b73  .....'..xl/works
+00004010: 6865 6574 732f 7368 6565 7431 392e 786d  heets/sheet19.xm
+00004020: 6c50 4b01 0214 0314 0000 0008 00d0 50a8  lPK...........P.
+00004030: 5819 ef2f 387b 0100 004b 0300 0019 0000  X../8{...K......
+00004040: 0000 0000 0000 0000 0080 81be 2800 0078  ............(..x
+00004050: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00004060: 6574 3230 2e78 6d6c 504b 0102 1403 1400  et20.xmlPK......
+00004070: 0000 0800 d050 a858 caac fec0 7101 0000  .....P.X....q...
+00004080: 3e03 0000 1900 0000 0000 0000 0000 0000  >...............
+00004090: 8081 702a 0000 786c 2f77 6f72 6b73 6865  ..p*..xl/workshe
+000040a0: 6574 732f 7368 6565 7432 312e 786d 6c50  ets/sheet21.xmlP
+000040b0: 4b01 0214 0314 0000 0008 00d0 50a8 5825  K...........P.X%
+000040c0: 1336 5183 0100 0057 0300 0019 0000 0000  .6Q....W........
+000040d0: 0000 0000 0000 0080 8118 2c00 0078 6c2f  ..........,..xl/
+000040e0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+000040f0: 3232 2e78 6d6c 504b 0102 1403 1400 0000  22.xmlPK........
+00004100: 0800 d050 a858 a50c 764f 5301 0000 a402  ...P.X..vOS.....
+00004110: 0000 1900 0000 0000 0000 0000 0000 8081  ................
+00004120: d22d 0000 786c 2f77 6f72 6b73 6865 6574  .-..xl/worksheet
+00004130: 732f 7368 6565 7432 332e 786d 6c50 4b01  s/sheet23.xmlPK.
+00004140: 0214 0314 0000 0008 00d0 50a8 5865 1756  ..........P.Xe.V
+00004150: 075c 0100 00b5 0200 0019 0000 0000 0000  .\..............
+00004160: 0000 0000 0080 815c 2f00 0078 6c2f 776f  .......\/..xl/wo
+00004170: 726b 7368 6565 7473 2f73 6865 6574 3234  rksheets/sheet24
+00004180: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00004190: d050 a858 d205 f146 5202 0000 470a 0000  .P.X...FR...G...
+000041a0: 0d00 0000 0000 0000 0000 0000 8001 ef30  ...............0
+000041b0: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
+000041c0: 4b01 0214 0314 0000 0008 00d0 50a8 58b7  K...........P.X.
+000041d0: 47eb 8ac0 0000 0016 0200 000b 0000 0000  G...............
+000041e0: 0000 0000 0000 0080 016c 3300 005f 7265  .........l3.._re
+000041f0: 6c73 2f2e 7265 6c73 504b 0102 1403 1400  ls/.relsPK......
+00004200: 0000 0800 d050 a858 dc9a 467c 9402 0000  .....P.X..F|....
+00004210: 0f09 0000 0f00 0000 0000 0000 0000 0000  ................
+00004220: 8001 5534 0000 786c 2f77 6f72 6b62 6f6f  ..U4..xl/workboo
+00004230: 6b2e 786d 6c50 4b01 0214 0314 0000 0008  k.xmlPK.........
+00004240: 00d0 50a8 5872 967e 9137 0100 0039 0f00  ..P.Xr.~.7...9..
+00004250: 001a 0000 0000 0000 0000 0000 0080 0116  ................
+00004260: 3700 0078 6c2f 5f72 656c 732f 776f 726b  7..xl/_rels/work
+00004270: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
+00004280: 0214 0314 0000 0008 00d0 50a8 588b 1ae4  ..........P.X...
+00004290: a471 0100 0035 1000 0013 0000 0000 0000  .q...5..........
+000042a0: 0000 0000 0080 0185 3800 005b 436f 6e74  ........8..[Cont
+000042b0: 656e 745f 5479 7065 735d 2e78 6d6c 504b  ent_Types].xmlPK
+000042c0: 0506 0000 0000 2000 2000 9708 0000 273a  ...... . .....':
+000042d0: 0000 0000                                ....
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/graphql/shareyourcloning_linkml.graphql` & `shareyourcloning_linkml-0.1.3a0/project/graphql/shareyourcloning_linkml.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+type AddGeneIdSource
+  {
+    id: Integer!
+    input: [Sequence]
+    output: Sequence
+    type: String
+    repositoryName: RepositoryName!
+    repositoryId: String!
+    sequenceFileUrl: String
+    addgeneSequenceType: AddGeneSequenceType
+  }
+
 type AssemblyJoin
   {
     leftFragment: Sequence!
     rightFragment: Sequence!
     leftLocation: SimpleSequenceLocation!
     rightLocation: SimpleSequenceLocation!
   }
@@ -20,14 +32,25 @@
   {
     sequences: [Sequence]!
     sources: [Source]!
     primers: [Primer]
     description: String
   }
 
+type CRISPRSource
+  {
+    id: Integer!
+    output: Sequence
+    type: String
+    circular: Boolean
+    assembly: [AssemblyJoin]!
+    input: [Sequence]
+    guides: [Primer]!
+  }
+
 type GenomeCoordinatesSource
   {
     id: Integer!
     input: [Sequence]
     output: Sequence
     type: String
     assemblyAccession: String
@@ -38,47 +61,49 @@
     end: Integer!
     strand: Integer!
   }
 
 type GibsonAssemblySource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     circular: Boolean
     assembly: [AssemblyJoin]!
+    input: [Sequence]
   }
 
 type HomologousRecombinationSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     circular: Boolean
     assembly: [AssemblyJoin]!
+    input: [Sequence]
   }
 
 type LigationSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     circular: Boolean
     assembly: [AssemblyJoin]!
+    input: [Sequence]
   }
 
 type ManuallyTypedSource
   {
     id: Integer!
     input: [Sequence]
     output: Sequence
     type: String
+    overhangCrick3prime: Integer
+    overhangWatson3prime: Integer
     userInput: String!
     circular: Boolean
   }
 
 type NamedThing
   {
     id: Integer!
@@ -86,37 +111,37 @@
 
 type OligoHybridizationSource
   {
     id: Integer!
     input: [Sequence]
     output: Sequence
     type: String
+    overhangCrick3prime: Integer
     forwardOligo: Primer!
     reverseOligo: Primer!
-    overhangCrick3prime: Integer
   }
 
 type PCRSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     circular: Boolean
     assembly: [AssemblyJoin]!
     forwardPrimer: Primer!
     reversePrimer: Primer!
+    input: [Sequence]
   }
 
 type PolymeraseExtensionSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
+    input: [Sequence]
   }
 
 type Primer
   {
     id: Integer!
     type: String
     name: String
@@ -132,59 +157,59 @@
     repositoryName: RepositoryName!
     repositoryId: String!
   }
 
 type RestrictionAndLigationSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     circular: Boolean
     assembly: [AssemblyJoin]!
     restrictionEnzymes: [String]!
+    input: [Sequence]
   }
 
 type RestrictionEnzymeDigestionSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
+    input: [Sequence]
     leftEdge: RestrictionSequenceCut
     rightEdge: RestrictionSequenceCut
   }
 
 type RestrictionSequenceCut
   {
-    cutWatson: Integer
-    overhang: Integer
+    cutWatson: Integer!
+    overhang: Integer!
     restrictionEnzyme: String!
   }
 
 interface Sequence
   {
     id: Integer!
     type: String
   }
 
 type SequenceCut
   {
-    cutWatson: Integer
-    overhang: Integer
+    cutWatson: Integer!
+    overhang: Integer!
   }
 
 type SequenceCutSource
   {
     id: Integer!
-    input: [Sequence]
     output: Sequence
     type: String
     leftEdge: SequenceCut
     rightEdge: SequenceCut
+    input: [Sequence]
   }
 
 type SimpleSequenceLocation
   {
     start: Integer!
     end: Integer!
     strand: Integer
@@ -199,17 +224,17 @@
   }
 
 type TextFileSequence
   {
     id: Integer!
     type: String
     sequenceFileFormat: SequenceFileFormat!
-    fileContent: String
     overhangCrick3prime: Integer
     overhangWatson3prime: Integer
+    fileContent: String
   }
 
 type UploadedFileSource
   {
     id: Integer!
     input: [Sequence]
     output: Sequence
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/jsonld/shareyourcloning_linkml.context.jsonld` & `shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.context.jsonld`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9427083333333334%*

 * *Differences: {"'@context'": "{'addgene_sequence_type': OrderedDict([('@context', OrderedDict([('@vocab', "*

 * *               "'@null'), ('text', 'skos:notation'), ('description', 'skos:prefLabel'), "*

 * *               "('meaning', '@id')])), ('@id', 'addgene_sequence_type')]), 'guides': "*

 * *               "OrderedDict([('@type', '@id'), ('@id', 'guides')]), 'sequence_file_url': "*

 * *               "OrderedDict([('@id', 'sequence_file_url')]), 'AddGeneIdSource': "*

 * *               "OrderedDict([('@id', 'AddGeneIdSource')]), 'CRISPRSo […]*

```diff
@@ -1,16 +1,22 @@
 {
     "@context": {
         "@vocab": "https://w3id.org/genestorian/ShareYourCloning_LinkML/",
+        "AddGeneIdSource": {
+            "@id": "AddGeneIdSource"
+        },
         "AssemblyJoin": {
             "@id": "AssemblyJoin"
         },
         "AssemblySource": {
             "@id": "AssemblySource"
         },
+        "CRISPRSource": {
+            "@id": "CRISPRSource"
+        },
         "CloningStrategy": {
             "@id": "CloningStrategy"
         },
         "GenomeCoordinatesSource": {
             "@id": "GenomeCoordinatesSource"
         },
         "GibsonAssemblySource": {
@@ -77,14 +83,23 @@
         },
         "TextFileSequence": {
             "@id": "TextFileSequence"
         },
         "UploadedFileSource": {
             "@id": "UploadedFileSource"
         },
+        "addgene_sequence_type": {
+            "@context": {
+                "@vocab": "@null",
+                "description": "skos:prefLabel",
+                "meaning": "@id",
+                "text": "skos:notation"
+            },
+            "@id": "addgene_sequence_type"
+        },
         "assembly": {
             "@id": "assembly",
             "@type": "@id"
         },
         "assembly_accession": {
             "@id": "assembly_accession"
         },
@@ -119,14 +134,18 @@
             "@id": "forward_primer",
             "@type": "@id"
         },
         "gene_id": {
             "@id": "gene_id",
             "@type": "xsd:integer"
         },
+        "guides": {
+            "@id": "guides",
+            "@type": "@id"
+        },
         "id": "@id",
         "index_in_file": {
             "@id": "index_in_file",
             "@type": "xsd:integer"
         },
         "input": {
             "@id": "input",
@@ -221,14 +240,17 @@
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
             },
             "@id": "sequence_file_format"
         },
+        "sequence_file_url": {
+            "@id": "sequence_file_url"
+        },
         "sequences": {
             "@id": "sequences",
             "@type": "@id"
         },
         "shareyourcloning_linkml": "https://w3id.org/genestorian/ShareYourCloning_LinkML/",
         "skos": "http://www.w3.org/2004/02/skos/core#",
         "sources": {
@@ -248,11 +270,11 @@
         },
         "user_input": {
             "@id": "user_input"
         }
     },
     "comments": {
         "description": "Auto generated by LinkML jsonld context generator",
-        "generation_date": "2024-04-24T17:03:58",
+        "generation_date": "2024-05-08T10:06:27",
         "source": "shareyourcloning_linkml.yaml"
     }
 }
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/jsonld/shareyourcloning_linkml.jsonld` & `shareyourcloning_linkml-0.1.3a0/project/jsonld/shareyourcloning_linkml.jsonld`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9130123273792107%*

 * *Differences: {"'classes'": "{2: {'slots': {insert: [(3, 'TextFileSequence_overhang_crick_3prime'), (4, "*

 * *              "'TextFileSequence_overhang_watson_3prime')], delete: [5, 4]}, 'attributes': "*

 * *              "{delete: [2, 1]}}, 4: {'attributes': {0: {'required': True}, 1: {'required': "*

 * *              "True}}}, 7: {'slots': {insert: [(4, 'ManuallyTypedSource_overhang_crick_3prime'), "*

 * *              "(5, 'ManuallyTypedSource_overhang_watson_3prime')]}}, 12: {'slots': {insert: [(5, "*

 * *              "'SequenceCutSource_i […]*

```diff
@@ -40,42 +40,30 @@
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
                     "name": "file_content",
                     "range": "string"
-                },
-                {
-                    "@type": "SlotDefinition",
-                    "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
-                    "name": "overhang_crick_3prime",
-                    "range": "integer"
-                },
-                {
-                    "@type": "SlotDefinition",
-                    "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
-                    "name": "overhang_watson_3prime",
-                    "range": "integer"
                 }
             ],
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/TextFileSequence",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/TextFileSequence",
             "description": "A sequence (may have features) defined by the content of a text file",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "Sequence",
             "name": "TextFileSequence",
             "slot_usage": {},
             "slots": [
                 "id",
                 "type",
                 "TextFileSequence_sequence_file_format",
-                "textFileSequence__file_content",
-                "textFileSequence__overhang_crick_3prime",
-                "textFileSequence__overhang_watson_3prime"
+                "TextFileSequence_overhang_crick_3prime",
+                "TextFileSequence_overhang_watson_3prime",
+                "textFileSequence__file_content"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
@@ -101,21 +89,23 @@
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
                     "description": "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.",
                     "name": "cut_watson",
-                    "range": "integer"
+                    "range": "integer",
+                    "required": true
                 },
                 {
                     "@type": "SlotDefinition",
                     "description": "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.",
                     "name": "overhang",
-                    "range": "integer"
+                    "range": "integer",
+                    "required": true
                 }
             ],
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceCut",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceCut",
             "description": "Represents a cut in a DNA sequence",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "SequenceCut",
@@ -182,14 +172,16 @@
             "name": "ManuallyTypedSource",
             "slot_usage": {},
             "slots": [
                 "id",
                 "input",
                 "output",
                 "type",
+                "ManuallyTypedSource_overhang_crick_3prime",
+                "ManuallyTypedSource_overhang_watson_3prime",
                 "manuallyTypedSource__user_input",
                 "manuallyTypedSource__circular"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
@@ -257,14 +249,41 @@
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
+                    "name": "addgene_sequence_type",
+                    "range": "AddGeneSequenceType"
+                }
+            ],
+            "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneIdSource",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneIdSource",
+            "description": "Represents the source of a sequence that is identified by an AddGene id",
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "RepositoryIdSource",
+            "name": "AddGeneIdSource",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "input",
+                "output",
+                "type",
+                "repositoryIdSource__repository_name",
+                "repositoryIdSource__repository_id",
+                "sequence_file_url",
+                "addGeneIdSource__addgene_sequence_type"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "attributes": [
+                {
+                    "@type": "SlotDefinition",
                     "description": "The accession of the assembly",
                     "name": "assembly_accession",
                     "range": "string"
                 },
                 {
                     "@type": "SlotDefinition",
                     "description": "The accession of the sequence",
@@ -348,19 +367,19 @@
             "description": "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting.",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "Source",
             "name": "SequenceCutSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "sequenceCutSource__left_edge",
-                "sequenceCutSource__right_edge"
+                "sequenceCutSource__right_edge",
+                "SequenceCutSource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
@@ -380,17 +399,17 @@
             "description": "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes.",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "SequenceCutSource",
             "name": "RestrictionEnzymeDigestionSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
+                "SequenceCutSource_input",
                 "restrictionEnzymeDigestionSource__left_edge",
                 "restrictionEnzymeDigestionSource__right_edge"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
@@ -530,94 +549,123 @@
             "description": "Represents the source of a sequence that is generated by PCR",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "AssemblySource",
             "name": "PCRSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "assemblySource__circular",
                 "assemblySource__assembly",
                 "pCRSource__forward_primer",
-                "pCRSource__reverse_primer"
+                "pCRSource__reverse_primer",
+                "PCRSource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/LigationSource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/LigationSource",
             "description": "Represents the source of a sequence that is generated by ligation with sticky or blunt ends.",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "AssemblySource",
             "name": "LigationSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "assemblySource__circular",
-                "assemblySource__assembly"
+                "assemblySource__assembly",
+                "LigationSource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/HomologousRecombinationSource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/HomologousRecombinationSource",
             "description": "Represents the source of a sequence that is generated by homologous recombination",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "AssemblySource",
             "name": "HomologousRecombinationSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "assemblySource__circular",
-                "assemblySource__assembly"
+                "assemblySource__assembly",
+                "HomologousRecombinationSource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/GibsonAssemblySource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/GibsonAssemblySource",
             "description": "Represents the source of a sequence that is generated by Gibson assembly",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "AssemblySource",
             "name": "GibsonAssemblySource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "assemblySource__circular",
-                "assemblySource__assembly"
+                "assemblySource__assembly",
+                "GibsonAssemblySource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/RestrictionAndLigationSource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/RestrictionAndLigationSource",
             "description": "Represents the source of a sequence that is generated by restriction and ligation",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "AssemblySource",
             "name": "RestrictionAndLigationSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
                 "type",
                 "assemblySource__circular",
                 "assemblySource__assembly",
-                "RestrictionAndLigationSource_restriction_enzymes"
+                "RestrictionAndLigationSource_restriction_enzymes",
+                "RestrictionAndLigationSource_input"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "attributes": [
+                {
+                    "@type": "SlotDefinition",
+                    "description": "The guide RNAs used in the CRISPR",
+                    "multivalued": true,
+                    "name": "guides",
+                    "range": "Primer",
+                    "required": true
+                }
+            ],
+            "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/CRISPRSource",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/CRISPRSource",
+            "description": "Represents the source of a sequence that is generated by CRISPR",
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "HomologousRecombinationSource",
+            "name": "CRISPRSource",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "output",
+                "type",
+                "assemblySource__circular",
+                "assemblySource__assembly",
+                "HomologousRecombinationSource_input",
+                "cRISPRSource__guides"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
@@ -628,53 +676,47 @@
                 },
                 {
                     "@type": "SlotDefinition",
                     "description": "The reverse oligo used in the hybridization",
                     "name": "reverse_oligo",
                     "range": "Primer",
                     "required": true
-                },
-                {
-                    "@type": "SlotDefinition",
-                    "description": "The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand.",
-                    "name": "overhang_crick_3prime",
-                    "range": "integer"
                 }
             ],
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/OligoHybridizationSource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/OligoHybridizationSource",
             "description": "Represents the source of a sequence that is generated by oligo hybridization",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "Source",
             "name": "OligoHybridizationSource",
             "slot_usage": {},
             "slots": [
                 "id",
                 "input",
                 "output",
                 "type",
+                "overhang_crick_3prime",
                 "oligoHybridizationSource__forward_oligo",
-                "oligoHybridizationSource__reverse_oligo",
-                "oligoHybridizationSource__overhang_crick_3prime"
+                "oligoHybridizationSource__reverse_oligo"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/PolymeraseExtensionSource",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/PolymeraseExtensionSource",
             "description": "Represents the source of a sequence that is generated by polymerase extension",
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "is_a": "Source",
             "name": "PolymeraseExtensionSource",
             "slot_usage": {},
             "slots": [
                 "id",
-                "input",
                 "output",
-                "type"
+                "type",
+                "PolymeraseExtensionSource_input"
             ]
         },
         {
             "@type": "ClassDefinition",
             "attributes": [
                 {
                     "@type": "SlotDefinition",
@@ -752,17 +794,32 @@
                 {
                     "text": "genbank"
                 },
                 {
                     "text": "snapgene"
                 }
             ]
+        },
+        {
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType",
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "name": "AddGeneSequenceType",
+            "permissible_values": [
+                {
+                    "description": "Full sequence of the plasmid submitted by the depositor",
+                    "text": "depositor-full"
+                },
+                {
+                    "description": "Full sequence of the plasmid performed by Addgene",
+                    "text": "addgene-full"
+                }
+            ]
         }
     ],
-    "generation_date": "2024-04-24T17:03:58",
+    "generation_date": "2024-05-08T10:06:27",
     "id": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
     "imports": [
         "linkml:types"
     ],
     "license": "MIT",
     "metamodel_version": "1.7.0",
     "name": "ShareYourCloning_LinkML",
@@ -920,49 +977,67 @@
             "name": "sequence_file_format",
             "owner": "UploadedFileSource",
             "range": "SequenceFileFormat",
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_format"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "file_content",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime",
+            "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
             "domain_of": [
-                "TextFileSequence"
+                "TextFileSequence",
+                "ManuallyTypedSource",
+                "OligoHybridizationSource"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "textFileSequence__file_content",
-            "owner": "TextFileSequence",
-            "range": "string",
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/file_content"
+            "name": "overhang_crick_3prime",
+            "owner": "OligoHybridizationSource",
+            "range": "integer",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "overhang_crick_3prime",
-            "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime",
+            "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
             "domain_of": [
-                "TextFileSequence"
+                "TextFileSequence",
+                "ManuallyTypedSource"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "textFileSequence__overhang_crick_3prime",
-            "owner": "TextFileSequence",
+            "ifabsent": "int(0)",
+            "name": "overhang_watson_3prime",
+            "owner": "ManuallyTypedSource",
             "range": "integer",
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime"
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "overhang_watson_3prime",
-            "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_url",
+            "description": "The URL of a sequence file",
+            "domain_of": [
+                "AddGeneIdSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "name": "sequence_file_url",
+            "owner": "AddGeneIdSource",
+            "pattern": "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$",
+            "range": "string",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_url"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "file_content",
             "domain_of": [
                 "TextFileSequence"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "textFileSequence__overhang_watson_3prime",
+            "name": "textFileSequence__file_content",
             "owner": "TextFileSequence",
-            "range": "integer",
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime"
+            "range": "string",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/file_content"
         },
         {
             "@type": "SlotDefinition",
             "alias": "sequence",
             "domain_of": [
                 "Primer"
             ],
@@ -980,27 +1055,29 @@
             "domain_of": [
                 "SequenceCut"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "sequenceCut__cut_watson",
             "owner": "SequenceCut",
             "range": "integer",
+            "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/cut_watson"
         },
         {
             "@type": "SlotDefinition",
             "alias": "overhang",
             "description": "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.",
             "domain_of": [
                 "SequenceCut"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "sequenceCut__overhang",
             "owner": "SequenceCut",
             "range": "integer",
+            "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang"
         },
         {
             "@type": "SlotDefinition",
             "alias": "user_input",
             "domain_of": [
                 "ManuallyTypedSource"
@@ -1077,14 +1154,26 @@
             "owner": "RepositoryIdSource",
             "range": "string",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/repository_id"
         },
         {
             "@type": "SlotDefinition",
+            "alias": "addgene_sequence_type",
+            "domain_of": [
+                "AddGeneIdSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "name": "addGeneIdSource__addgene_sequence_type",
+            "owner": "AddGeneIdSource",
+            "range": "AddGeneSequenceType",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/addgene_sequence_type"
+        },
+        {
+            "@type": "SlotDefinition",
             "alias": "assembly_accession",
             "description": "The accession of the assembly",
             "domain_of": [
                 "GenomeCoordinatesSource"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "genomeCoordinatesSource__assembly_accession",
@@ -1379,14 +1468,29 @@
             "owner": "PCRSource",
             "range": "Primer",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/reverse_primer"
         },
         {
             "@type": "SlotDefinition",
+            "alias": "guides",
+            "description": "The guide RNAs used in the CRISPR",
+            "domain_of": [
+                "CRISPRSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "multivalued": true,
+            "name": "cRISPRSource__guides",
+            "owner": "CRISPRSource",
+            "range": "Primer",
+            "required": true,
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/guides"
+        },
+        {
+            "@type": "SlotDefinition",
             "alias": "forward_oligo",
             "description": "The forward oligo used in the hybridization",
             "domain_of": [
                 "OligoHybridizationSource"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "name": "oligoHybridizationSource__forward_oligo",
@@ -1407,27 +1511,14 @@
             "owner": "OligoHybridizationSource",
             "range": "Primer",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/reverse_oligo"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "overhang_crick_3prime",
-            "description": "The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand.",
-            "domain_of": [
-                "OligoHybridizationSource"
-            ],
-            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
-            "name": "oligoHybridizationSource__overhang_crick_3prime",
-            "owner": "OligoHybridizationSource",
-            "range": "integer",
-            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime"
-        },
-        {
-            "@type": "SlotDefinition",
             "alias": "sequences",
             "description": "The sequences that are used in the cloning strategy",
             "domain_of": [
                 "CloningStrategy"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
             "inlined": true,
@@ -1500,14 +1591,52 @@
             "range": "SequenceFileFormat",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_format",
             "usage_slot_name": "sequence_file_format"
         },
         {
             "@type": "SlotDefinition",
+            "alias": "overhang_crick_3prime",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime",
+            "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
+            "domain": "TextFileSequence",
+            "domain_of": [
+                "TextFileSequence"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "ifabsent": "int(0)",
+            "is_a": "overhang_crick_3prime",
+            "is_usage_slot": true,
+            "name": "TextFileSequence_overhang_crick_3prime",
+            "owner": "TextFileSequence",
+            "range": "integer",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime",
+            "usage_slot_name": "overhang_crick_3prime"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "overhang_watson_3prime",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime",
+            "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
+            "domain": "TextFileSequence",
+            "domain_of": [
+                "TextFileSequence"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "ifabsent": "int(0)",
+            "is_a": "overhang_watson_3prime",
+            "is_usage_slot": true,
+            "name": "TextFileSequence_overhang_watson_3prime",
+            "owner": "TextFileSequence",
+            "range": "integer",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime",
+            "usage_slot_name": "overhang_watson_3prime"
+        },
+        {
+            "@type": "SlotDefinition",
             "alias": "restriction_enzyme",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/restriction_enzyme",
             "domain": "RestrictionSequenceCut",
             "domain_of": [
                 "RestrictionSequenceCut"
             ],
             "exact_mappings": [
@@ -1521,14 +1650,52 @@
             "range": "string",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/restriction_enzyme",
             "usage_slot_name": "restriction_enzyme"
         },
         {
             "@type": "SlotDefinition",
+            "alias": "overhang_crick_3prime",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime",
+            "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
+            "domain": "ManuallyTypedSource",
+            "domain_of": [
+                "ManuallyTypedSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "ifabsent": "int(0)",
+            "is_a": "overhang_crick_3prime",
+            "is_usage_slot": true,
+            "name": "ManuallyTypedSource_overhang_crick_3prime",
+            "owner": "ManuallyTypedSource",
+            "range": "integer",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_crick_3prime",
+            "usage_slot_name": "overhang_crick_3prime"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "overhang_watson_3prime",
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime",
+            "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
+            "domain": "ManuallyTypedSource",
+            "domain_of": [
+                "ManuallyTypedSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "ifabsent": "int(0)",
+            "is_a": "overhang_watson_3prime",
+            "is_usage_slot": true,
+            "name": "ManuallyTypedSource_overhang_watson_3prime",
+            "owner": "ManuallyTypedSource",
+            "range": "integer",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/overhang_watson_3prime",
+            "usage_slot_name": "overhang_watson_3prime"
+        },
+        {
+            "@type": "SlotDefinition",
             "alias": "sequence_file_format",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_format",
             "description": "The format of a sequence file",
             "domain": "UploadedFileSource",
             "domain_of": [
                 "UploadedFileSource"
             ],
@@ -1540,14 +1707,159 @@
             "range": "SequenceFileFormat",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/sequence_file_format",
             "usage_slot_name": "sequence_file_format"
         },
         {
             "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "exact_card",
+                        "exact_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "SequenceCutSource",
+            "domain_of": [
+                "SequenceCutSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "SequenceCutSource_input",
+            "owner": "SequenceCutSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "exact_card",
+                        "exact_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "PCRSource",
+            "domain_of": [
+                "PCRSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "PCRSource_input",
+            "owner": "PCRSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "min_card",
+                        "minimum_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "LigationSource",
+            "domain_of": [
+                "LigationSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "LigationSource_input",
+            "owner": "LigationSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "exact_card",
+                        "exact_cardinality": 2
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "HomologousRecombinationSource",
+            "domain_of": [
+                "HomologousRecombinationSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "HomologousRecombinationSource_input",
+            "owner": "HomologousRecombinationSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "min_card",
+                        "minimum_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "GibsonAssemblySource",
+            "domain_of": [
+                "GibsonAssemblySource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "GibsonAssemblySource_input",
+            "owner": "GibsonAssemblySource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
             "alias": "restriction_enzymes",
             "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/restriction_enzymes",
             "domain": "RestrictionAndLigationSource",
             "domain_of": [
                 "RestrictionAndLigationSource"
             ],
             "exact_mappings": [
@@ -1559,19 +1871,77 @@
             "multivalued": true,
             "name": "RestrictionAndLigationSource_restriction_enzymes",
             "owner": "RestrictionAndLigationSource",
             "range": "string",
             "required": true,
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/restriction_enzymes",
             "usage_slot_name": "restriction_enzymes"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "min_card",
+                        "minimum_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "RestrictionAndLigationSource",
+            "domain_of": [
+                "RestrictionAndLigationSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "RestrictionAndLigationSource_input",
+            "owner": "RestrictionAndLigationSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
+        },
+        {
+            "@type": "SlotDefinition",
+            "alias": "input",
+            "array": {
+                "@type": "ArrayExpression",
+                "dimensions": [
+                    {
+                        "@type": "DimensionExpression",
+                        "alias": "exact_card",
+                        "exact_cardinality": 1
+                    }
+                ]
+            },
+            "definition_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+            "domain": "PolymeraseExtensionSource",
+            "domain_of": [
+                "PolymeraseExtensionSource"
+            ],
+            "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "is_a": "input",
+            "is_usage_slot": true,
+            "multivalued": true,
+            "name": "PolymeraseExtensionSource_input",
+            "owner": "PolymeraseExtensionSource",
+            "range": "Sequence",
+            "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
+            "usage_slot_name": "input"
         }
     ],
     "source_file": "shareyourcloning_linkml.yaml",
-    "source_file_date": "2024-04-24T14:18:18",
-    "source_file_size": 13200,
+    "source_file_date": "2024-05-08T09:28:36",
+    "source_file_size": 15500,
     "title": "ShareYourCloning_LinkML",
     "types": [
         {
             "@type": "TypeDefinition",
             "base": "str",
             "definition_uri": "https://w3id.org/linkml/String",
             "description": "A character string",
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/jsonschema/shareyourcloning_linkml.schema.json` & `shareyourcloning_linkml-0.1.3a0/project/jsonschema/shareyourcloning_linkml.schema.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927723933359512%*

 * *Differences: {"'$defs'": "{'CloningStrategy': {'properties': {'sources': {'items': {'anyOf': {insert: [(13, "*

 * *            "OrderedDict([('$ref', '#/$defs/CRISPRSource')])), (15, OrderedDict([('$ref', "*

 * *            "'#/$defs/AddGeneIdSource')]))]}}}}}, 'ManuallyTypedSource': {'properties': "*

 * *            '{\'overhang_crick_3prime\': OrderedDict([(\'description\', "Taken from pydna\'s '*

 * *            "`dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' "*

 * *            'of the molecule, or 3\' of […]*

```diff
@@ -1,9 +1,68 @@
 {
     "$defs": {
+        "AddGeneIdSource": {
+            "additionalProperties": false,
+            "description": "Represents the source of a sequence that is identified by an AddGene id",
+            "properties": {
+                "addgene_sequence_type": {
+                    "$ref": "#/$defs/AddGeneSequenceType"
+                },
+                "id": {
+                    "description": "A unique identifier for a thing",
+                    "type": "integer"
+                },
+                "input": {
+                    "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+                    "items": {
+                        "type": "integer"
+                    },
+                    "type": "array"
+                },
+                "output": {
+                    "description": "Identifier of the sequence that is the output of this source.",
+                    "type": "integer"
+                },
+                "repository_id": {
+                    "description": "The id of the sequence in the repository",
+                    "type": "string"
+                },
+                "repository_name": {
+                    "$ref": "#/$defs/RepositoryName"
+                },
+                "sequence_file_url": {
+                    "description": "The URL of a sequence file",
+                    "pattern": "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$",
+                    "type": "string"
+                },
+                "type": {
+                    "description": "The type of the source",
+                    "enum": [
+                        "AddGeneIdSource"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "repository_name",
+                "repository_id",
+                "id"
+            ],
+            "title": "AddGeneIdSource",
+            "type": "object"
+        },
+        "AddGeneSequenceType": {
+            "description": "",
+            "enum": [
+                "depositor-full",
+                "addgene-full"
+            ],
+            "title": "AddGeneSequenceType",
+            "type": "string"
+        },
         "AssemblyJoin": {
             "additionalProperties": false,
             "description": "Represents a joint between two fragments in an assembly",
             "properties": {
                 "left_fragment": {
                     "type": "integer"
                 },
@@ -69,14 +128,67 @@
             "required": [
                 "assembly",
                 "id"
             ],
             "title": "AssemblySource",
             "type": "object"
         },
+        "CRISPRSource": {
+            "additionalProperties": false,
+            "description": "Represents the source of a sequence that is generated by CRISPR",
+            "properties": {
+                "assembly": {
+                    "description": "The joins between the fragments in the assembly",
+                    "items": {
+                        "$ref": "#/$defs/AssemblyJoin"
+                    },
+                    "type": "array"
+                },
+                "circular": {
+                    "description": "Whether the assembly is circular or not",
+                    "type": "boolean"
+                },
+                "guides": {
+                    "description": "The guide RNAs used in the CRISPR",
+                    "items": {
+                        "type": "integer"
+                    },
+                    "type": "array"
+                },
+                "id": {
+                    "description": "A unique identifier for a thing",
+                    "type": "integer"
+                },
+                "input": {
+                    "description": "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.",
+                    "items": {
+                        "type": "integer"
+                    },
+                    "type": "array"
+                },
+                "output": {
+                    "description": "Identifier of the sequence that is the output of this source.",
+                    "type": "integer"
+                },
+                "type": {
+                    "description": "The type of the source",
+                    "enum": [
+                        "CRISPRSource"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "guides",
+                "assembly",
+                "id"
+            ],
+            "title": "CRISPRSource",
+            "type": "object"
+        },
         "CloningStrategy": {
             "additionalProperties": false,
             "description": "Represents a cloning strategy",
             "properties": {
                 "description": {
                     "description": "A description of the cloning strategy",
                     "type": "string"
@@ -142,15 +254,21 @@
                             {
                                 "$ref": "#/$defs/GibsonAssemblySource"
                             },
                             {
                                 "$ref": "#/$defs/RestrictionAndLigationSource"
                             },
                             {
+                                "$ref": "#/$defs/CRISPRSource"
+                            },
+                            {
                                 "$ref": "#/$defs/RestrictionEnzymeDigestionSource"
+                            },
+                            {
+                                "$ref": "#/$defs/AddGeneIdSource"
                             }
                         ]
                     },
                     "type": "array"
                 }
             },
             "required": [
@@ -379,14 +497,22 @@
                     },
                     "type": "array"
                 },
                 "output": {
                     "description": "Identifier of the sequence that is the output of this source.",
                     "type": "integer"
                 },
+                "overhang_crick_3prime": {
+                    "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
+                    "type": "integer"
+                },
+                "overhang_watson_3prime": {
+                    "description": "The equivalent of `overhang_crick_3prime` but for the watson strand",
+                    "type": "integer"
+                },
                 "type": {
                     "description": "The type of the source",
                     "enum": [
                         "ManuallyTypedSource"
                     ],
                     "type": "string"
                 },
@@ -437,15 +563,15 @@
                     "type": "array"
                 },
                 "output": {
                     "description": "Identifier of the sequence that is the output of this source.",
                     "type": "integer"
                 },
                 "overhang_crick_3prime": {
-                    "description": "The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand.",
+                    "description": "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand",
                     "type": "integer"
                 },
                 "reverse_oligo": {
                     "description": "The reverse oligo used in the hybridization",
                     "type": "integer"
                 },
                 "type": {
@@ -737,15 +863,17 @@
                     "type": "integer"
                 },
                 "restriction_enzyme": {
                     "type": "string"
                 }
             },
             "required": [
-                "restriction_enzyme"
+                "restriction_enzyme",
+                "cut_watson",
+                "overhang"
             ],
             "title": "RestrictionSequenceCut",
             "type": "object"
         },
         "SequenceCut": {
             "additionalProperties": false,
             "description": "Represents a cut in a DNA sequence",
@@ -755,14 +883,18 @@
                     "type": "integer"
                 },
                 "overhang": {
                     "description": "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.",
                     "type": "integer"
                 }
             },
+            "required": [
+                "cut_watson",
+                "overhang"
+            ],
             "title": "SequenceCut",
             "type": "object"
         },
         "SequenceCutSource": {
             "additionalProperties": false,
             "description": "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting.",
             "properties": {
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/owl/shareyourcloning_linkml.owl.ttl` & `shareyourcloning_linkml-0.1.3a0/project/owl/shareyourcloning_linkml.owl.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -9,308 +9,369 @@
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 shareyourcloning_linkml:CloningStrategy a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "CloningStrategy" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sources ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:primers ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:sequences ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Source ;
-            owl:onProperty shareyourcloning_linkml:sources ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:primers ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Source ;
+            owl:onProperty shareyourcloning_linkml:sources ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
+            owl:onProperty shareyourcloning_linkml:sequences ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequences ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:description ] ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sources ] ;
     skos:definition "Represents a cloning strategy" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:AssemblyJoin a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblyJoin" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_fragment ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
-            owl:onProperty shareyourcloning_linkml:left_location ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left_fragment ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:left_fragment ],
+            owl:onProperty shareyourcloning_linkml:right_location ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:right_location ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:right_fragment ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
+            owl:onProperty shareyourcloning_linkml:right_location ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
+            owl:onProperty shareyourcloning_linkml:left_location ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_fragment ],
+            owl:onProperty shareyourcloning_linkml:left_fragment ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_location ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:left_fragment ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_location ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
-            owl:onProperty shareyourcloning_linkml:right_location ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:right_fragment ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_location ],
+            owl:onProperty shareyourcloning_linkml:right_fragment ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:left_fragment ] ;
     skos:definition "Represents a joint between two fragments in an assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:GenomeCoordinatesSource a owl:Class,
+shareyourcloning_linkml:AddGeneIdSource a owl:Class,
         linkml:ClassDefinition ;
-    rdfs:label "GenomeCoordinatesSource" ;
+    rdfs:label "AddGeneIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_accession ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
+            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+            owl:allValuesFrom shareyourcloning_linkml:AddGeneSequenceType ;
+            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
+            owl:allValuesFrom [ a rdfs:Datatype ;
+                    owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
+                                owl:onDatatype xsd:string ;
+                                owl:withRestrictions ( [ xsd:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ] ) ] ) ] ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
+        shareyourcloning_linkml:RepositoryIdSource ;
+    skos:definition "Represents the source of a sequence that is identified by an AddGene id" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
+<https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full> a owl:Class,
+        shareyourcloning_linkml:AddGeneSequenceType ;
+    rdfs:label "addgene-full" ;
+    rdfs:subClassOf shareyourcloning_linkml:AddGeneSequenceType .
+
+<https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#depositor-full> a owl:Class,
+        shareyourcloning_linkml:AddGeneSequenceType ;
+    rdfs:label "depositor-full" ;
+    rdfs:subClassOf shareyourcloning_linkml:AddGeneSequenceType .
+
+shareyourcloning_linkml:CRISPRSource a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "CRISPRSource" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:guides ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:guides ],
+        shareyourcloning_linkml:HomologousRecombinationSource ;
+    skos:definition "Represents the source of a sequence that is generated by CRISPR" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
+shareyourcloning_linkml:GenomeCoordinatesSource a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "GenomeCoordinatesSource" ;
+    rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:locus_tag ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_accession ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:end ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:end ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:gene_id ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:GibsonAssemblySource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "GibsonAssemblySource" ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by Gibson assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:HomologousRecombinationSource a owl:Class,
-        linkml:ClassDefinition ;
-    rdfs:label "HomologousRecombinationSource" ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
-    skos:definition "Represents the source of a sequence that is generated by homologous recombination" ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
 shareyourcloning_linkml:LigationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "LigationSource" ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:ManuallyTypedSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "ManuallyTypedSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:user_input ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty shareyourcloning_linkml:circular ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:user_input ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:user_input ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:user_input ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty shareyourcloning_linkml:circular ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is manually typed by the user" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:NamedThing a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "NamedThing" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ] ;
     skos:exactMatch schema1:Thing ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:OligoHybridizationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "OligoHybridizationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is generated by oligo hybridization" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:PCRSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "PCRSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_primer ],
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:forward_primer ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_primer ],
         [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_primer ],
+            owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_primer ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_primer ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by PCR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:PolymeraseExtensionSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "PolymeraseExtensionSource" ;
-    rdfs:subClassOf shareyourcloning_linkml:Source ;
-    skos:definition "Represents the source of a sequence that is generated by polymerase extension" ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
-shareyourcloning_linkml:RepositoryIdSource a owl:Class,
-        linkml:ClassDefinition ;
-    rdfs:label "RepositoryIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:RepositoryName ;
-            owl:onProperty shareyourcloning_linkml:repository_name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_name ],
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_name ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
         shareyourcloning_linkml:Source ;
-    skos:definition "Represents the source of a sequence that is identified by a repository id" ;
+    skos:definition "Represents the source of a sequence that is generated by polymerase extension" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#addgene> a owl:Class,
         shareyourcloning_linkml:RepositoryName ;
     rdfs:label "addgene" ;
     rdfs:subClassOf shareyourcloning_linkml:RepositoryName .
 
@@ -319,60 +380,66 @@
     rdfs:label "genbank" ;
     rdfs:subClassOf shareyourcloning_linkml:RepositoryName .
 
 shareyourcloning_linkml:RestrictionAndLigationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionAndLigationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by restriction and ligation" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionEnzymeDigestionSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
-            owl:onProperty shareyourcloning_linkml:left_edge ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
+            owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
+            owl:onProperty shareyourcloning_linkml:left_edge ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:left_edge ],
+            owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         shareyourcloning_linkml:SequenceCutSource ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionSequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionSequenceCut" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
         shareyourcloning_linkml:SequenceCut ;
     skos:definition "Represents a cut in a DNA sequence that is made by a restriction enzyme" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta> a owl:Class,
         shareyourcloning_linkml:SequenceFileFormat ;
     rdfs:label "fasta" ;
@@ -388,131 +455,130 @@
     rdfs:label "snapgene" ;
     rdfs:subClassOf shareyourcloning_linkml:SequenceFileFormat .
 
 shareyourcloning_linkml:SimpleSequenceLocation a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SimpleSequenceLocation" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:start ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ] ;
     skos:definition "Represents a location within a sequence, for now support for ranges only" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:TextFileSequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TextFileSequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "A sequence (may have features) defined by the content of a text file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:UploadedFileSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "UploadedFileSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:file_name ],
-        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:file_name ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:file_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:index_in_file ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is uploaded as a file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:assembly a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "assembly" ;
     skos:definition "The joins between the fragments in the assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:input a owl:ObjectProperty,
+shareyourcloning_linkml:guides a owl:ObjectProperty,
         linkml:SlotDefinition ;
-    rdfs:label "input" ;
-    rdfs:range shareyourcloning_linkml:Sequence ;
-    skos:definition "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+    rdfs:label "guides" ;
+    skos:definition "The guide RNAs used in the CRISPR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:primers a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "primers" ;
     skos:definition "The primers that are used in the cloning strategy" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
@@ -532,63 +598,112 @@
 
 shareyourcloning_linkml:sources a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "sources" ;
     skos:definition "The sources of the sequences that are used in the cloning strategy" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:HomologousRecombinationSource a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "HomologousRecombinationSource" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        shareyourcloning_linkml:AssemblySource ;
+    skos:definition "Represents the source of a sequence that is generated by homologous recombination" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
+shareyourcloning_linkml:RepositoryIdSource a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "RepositoryIdSource" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_name ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_name ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:RepositoryName ;
+            owl:onProperty shareyourcloning_linkml:repository_name ],
+        shareyourcloning_linkml:Source ;
+    skos:definition "Represents the source of a sequence that is identified by a repository id" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:SequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCut" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:cut_watson ],
+            owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang ],
+            owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:cut_watson ] ;
     skos:definition "Represents a cut in a DNA sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceCutSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCutSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:right_edge ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:addgene_sequence_type a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "addgene_sequence_type" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:assembly_accession a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "assembly_accession" ;
     skos:definition "The accession of the assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:cut_watson a owl:ObjectProperty,
@@ -671,20 +786,14 @@
 
 shareyourcloning_linkml:overhang a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "overhang" ;
     skos:definition "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
-shareyourcloning_linkml:overhang_watson_3prime a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "overhang_watson_3prime" ;
-    skos:definition "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
-    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
-
 shareyourcloning_linkml:repository_id a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "repository_id" ;
     skos:definition "The id of the sequence in the repository" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:repository_name a owl:ObjectProperty,
@@ -729,19 +838,35 @@
 
 shareyourcloning_linkml:sequence_accession a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "sequence_accession" ;
     skos:definition "The accession of the sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:sequence_file_url a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "sequence_file_url" ;
+    rdfs:range [ a rdfs:Datatype ;
+            owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
+                        owl:onDatatype xsd:string ;
+                        owl:withRestrictions ( [ xsd:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ] ) ] ) ] ;
+    skos:definition "The URL of a sequence file" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:user_input a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "user_input" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:AddGeneSequenceType a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#depositor-full> <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full> ) ;
+    linkml:permissible_values <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full>,
+        <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#depositor-full> .
+
 shareyourcloning_linkml:RepositoryName a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#addgene> <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#genbank> ) ;
     linkml:permissible_values <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#addgene>,
         <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#genbank> .
 
 shareyourcloning_linkml:circular a owl:ObjectProperty,
@@ -756,16 +881,20 @@
     rdfs:range linkml:Integer ;
     skos:definition "A unique identifier for a thing" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:left_edge a owl:ObjectProperty,
         linkml:SlotDefinition .
 
-shareyourcloning_linkml:overhang_crick_3prime a owl:ObjectProperty,
-        linkml:SlotDefinition .
+shareyourcloning_linkml:overhang_watson_3prime a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "overhang_watson_3prime" ;
+    rdfs:range linkml:Integer ;
+    skos:definition "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:right_edge a owl:ObjectProperty,
         linkml:SlotDefinition .
 
 shareyourcloning_linkml:sequence_file_format a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "sequence_file_format" ;
@@ -779,102 +908,103 @@
 shareyourcloning_linkml:strand a owl:ObjectProperty,
         linkml:SlotDefinition .
 
 shareyourcloning_linkml:AssemblySource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblySource" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:assembly ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
-        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:AssemblyJoin ;
             owl:onProperty shareyourcloning_linkml:assembly ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is an assembly of other sequences" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Primer a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Primer" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
-        [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:name ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:name ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "An oligonucleotide or primer" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceFileFormat a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#genbank> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> ) ;
     linkml:permissible_values <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta>,
         <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#genbank>,
         <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> .
 
+shareyourcloning_linkml:overhang_crick_3prime a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "overhang_crick_3prime" ;
+    rdfs:range linkml:Integer ;
+    skos:definition "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:Sequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Sequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:type ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:id ],
+            owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:type ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:id ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Source a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Source" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:output ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:type ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
@@ -882,20 +1012,33 @@
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
+            owl:onProperty shareyourcloning_linkml:output ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:type ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents the source of a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
+shareyourcloning_linkml:input a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "input" ;
+    rdfs:range shareyourcloning_linkml:Sequence ;
+    skos:definition "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+    skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
+
 shareyourcloning_linkml:type a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "type" ;
     rdfs:range linkml:String ;
     skos:definition "The type of the source" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
@@ -908,90 +1051,101 @@
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:PCRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:PCRSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:Sequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
+    rdfs:subClassOf shareyourcloning_linkml:AddGeneIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Sequence .
+    owl:someValuesFrom shareyourcloning_linkml:AddGeneIdSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:OligoHybridizationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:Primer ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:OligoHybridizationSource .
+    owl:someValuesFrom shareyourcloning_linkml:Primer .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:GenomeCoordinatesSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:GenomeCoordinatesSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
+    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
+
+[] a owl:Restriction ;
+    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
+    owl:onProperty shareyourcloning_linkml:type ;
+    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:Source ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:Source .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
+    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
+    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
+    rdfs:subClassOf shareyourcloning_linkml:OligoHybridizationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
+    owl:someValuesFrom shareyourcloning_linkml:OligoHybridizationSource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:RestrictionEnzymeDigestionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:UploadedFileSource ;
+    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:UploadedFileSource .
+    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:UploadedFileSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:UploadedFileSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
+    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
+    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:TextFileSequence ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:TextFileSequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Primer ;
+    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Primer .
+    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:CRISPRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:CRISPRSource .
+
+[] a owl:Restriction ;
+    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    owl:onProperty shareyourcloning_linkml:type ;
+    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:RepositoryIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:RepositoryIdSource .
+
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/protobuf/shareyourcloning_linkml.proto` & `shareyourcloning_linkml-0.1.3a0/project/protobuf/shareyourcloning_linkml.proto`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+// Represents the source of a sequence that is identified by an AddGene id
+message AddGeneIdSource
+ {
+  integer id = 0
+ repeated  sequence input = 0
+  sequence output = 0
+  string type = 0
+  repositoryName repositoryName = 0
+  string repositoryId = 0
+  string sequenceFileUrl = 0
+  addGeneSequenceType addgeneSequenceType = 0
+ }
 // Represents a joint between two fragments in an assembly
 message AssemblyJoin
  {
   sequence leftFragment = 0
   sequence rightFragment = 0
   simpleSequenceLocation leftLocation = 0
   simpleSequenceLocation rightLocation = 0
@@ -20,14 +32,25 @@
 message CloningStrategy
  {
  repeated  sequence sequences = 0
  repeated  source sources = 0
  repeated  primer primers = 0
   string description = 0
  }
+// Represents the source of a sequence that is generated by CRISPR
+message CRISPRSource
+ {
+  integer id = 0
+  sequence output = 0
+  string type = 0
+  boolean circular = 0
+ repeated  assemblyJoin assembly = 0
+ repeated  sequence input = 0
+ repeated  primer guides = 0
+ }
 // Represents the source of a sequence that is identified by genome coordinates, requested from NCBI
 message GenomeCoordinatesSource
  {
   integer id = 0
  repeated  sequence input = 0
   sequence output = 0
   string type = 0
@@ -39,84 +62,86 @@
   integer end = 0
   integer strand = 0
  }
 // Represents the source of a sequence that is generated by Gibson assembly
 message GibsonAssemblySource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   boolean circular = 0
  repeated  assemblyJoin assembly = 0
+ repeated  sequence input = 0
  }
 // Represents the source of a sequence that is generated by homologous recombination
 message HomologousRecombinationSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   boolean circular = 0
  repeated  assemblyJoin assembly = 0
+ repeated  sequence input = 0
  }
 // Represents the source of a sequence that is generated by ligation with sticky or blunt ends.
 message LigationSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   boolean circular = 0
  repeated  assemblyJoin assembly = 0
+ repeated  sequence input = 0
  }
 // Represents the source of a sequence that is manually typed by the user
 message ManuallyTypedSource
  {
   integer id = 0
  repeated  sequence input = 0
   sequence output = 0
   string type = 0
+  integer overhangCrick3prime = 0
+  integer overhangWatson3prime = 0
   string userInput = 0
   boolean circular = 0
  }
 message NamedThing
  {
   integer id = 0
  }
 // Represents the source of a sequence that is generated by oligo hybridization
 message OligoHybridizationSource
  {
   integer id = 0
  repeated  sequence input = 0
   sequence output = 0
   string type = 0
+  integer overhangCrick3prime = 0
   primer forwardOligo = 0
   primer reverseOligo = 0
-  integer overhangCrick3prime = 0
  }
 // Represents the source of a sequence that is generated by PCR
 message PCRSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   boolean circular = 0
  repeated  assemblyJoin assembly = 0
   primer forwardPrimer = 0
   primer reversePrimer = 0
+ repeated  sequence input = 0
  }
 // Represents the source of a sequence that is generated by polymerase extension
 message PolymeraseExtensionSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
+ repeated  sequence input = 0
  }
 // An oligonucleotide or primer
 message Primer
  {
   integer id = 0
   string type = 0
   string name = 0
@@ -132,28 +157,28 @@
   repositoryName repositoryName = 0
   string repositoryId = 0
  }
 // Represents the source of a sequence that is generated by restriction and ligation
 message RestrictionAndLigationSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   boolean circular = 0
  repeated  assemblyJoin assembly = 0
  repeated  string restrictionEnzymes = 0
+ repeated  sequence input = 0
  }
 // Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes.
 message RestrictionEnzymeDigestionSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
+ repeated  sequence input = 0
   restrictionSequenceCut leftEdge = 0
   restrictionSequenceCut rightEdge = 0
  }
 // Represents a cut in a DNA sequence that is made by a restriction enzyme
 message RestrictionSequenceCut
  {
   integer cutWatson = 0
@@ -166,36 +191,36 @@
   integer cutWatson = 0
   integer overhang = 0
  }
 // Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting.
 message SequenceCutSource
  {
   integer id = 0
- repeated  sequence input = 0
   sequence output = 0
   string type = 0
   sequenceCut leftEdge = 0
   sequenceCut rightEdge = 0
+ repeated  sequence input = 0
  }
 // Represents a location within a sequence, for now support for ranges only
 message SimpleSequenceLocation
  {
   integer start = 0
   integer end = 0
   integer strand = 0
  }
 // A sequence (may have features) defined by the content of a text file
 message TextFileSequence
  {
   integer id = 0
   string type = 0
   sequenceFileFormat sequenceFileFormat = 0
-  string fileContent = 0
   integer overhangCrick3prime = 0
   integer overhangWatson3prime = 0
+  string fileContent = 0
  }
 // Represents the source of a sequence that is uploaded as a file
 message UploadedFileSource
  {
   integer id = 0
  repeated  sequence input = 0
   sequence output = 0
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/python/shareyourcloning_linkml.py` & `shareyourcloning_linkml-0.1.3a0/project/python/shareyourcloning_linkml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 # Auto generated from shareyourcloning_linkml.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-04-24T17:03:58
+# Generation date: 2024-05-08T10:06:28
 # Schema: ShareYourCloning_LinkML
 #
 # id: https://w3id.org/genestorian/ShareYourCloning_LinkML
 # description: A LinkML data model for ShareYourCloning
 # license: MIT
 
 import dataclasses
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
 from datetime import date, datetime
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-    PvFormulaOptions,
-)
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_str,
-    extended_float,
-    extended_int,
-)
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.linkml_model.types import Boolean, Integer, String
 from linkml_runtime.utils.metamodelcore import Bool
 
@@ -87,14 +76,18 @@
     pass
 
 
 class RepositoryIdSourceId(SourceId):
     pass
 
 
+class AddGeneIdSourceId(RepositoryIdSourceId):
+    pass
+
+
 class GenomeCoordinatesSourceId(SourceId):
     pass
 
 
 class SequenceCutSourceId(SourceId):
     pass
 
@@ -123,14 +116,18 @@
     pass
 
 
 class RestrictionAndLigationSourceId(AssemblySourceId):
     pass
 
 
+class CRISPRSourceId(HomologousRecombinationSourceId):
+    pass
+
+
 class OligoHybridizationSourceId(SourceId):
     pass
 
 
 class PolymeraseExtensionSourceId(SourceId):
     pass
 
@@ -209,38 +206,38 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["TextFileSequence"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:TextFileSequence"
     class_name: ClassVar[str] = "TextFileSequence"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.TextFileSequence
 
     id: Union[int, TextFileSequenceId] = None
     sequence_file_format: Union[str, "SequenceFileFormat"] = None
+    overhang_crick_3prime: Optional[int] = 0
+    overhang_watson_3prime: Optional[int] = 0
     file_content: Optional[str] = None
-    overhang_crick_3prime: Optional[int] = None
-    overhang_watson_3prime: Optional[int] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TextFileSequenceId):
             self.id = TextFileSequenceId(self.id)
 
         if self._is_empty(self.sequence_file_format):
             self.MissingRequiredField("sequence_file_format")
         if not isinstance(self.sequence_file_format, SequenceFileFormat):
             self.sequence_file_format = SequenceFileFormat(self.sequence_file_format)
 
-        if self.file_content is not None and not isinstance(self.file_content, str):
-            self.file_content = str(self.file_content)
-
         if self.overhang_crick_3prime is not None and not isinstance(self.overhang_crick_3prime, int):
             self.overhang_crick_3prime = int(self.overhang_crick_3prime)
 
         if self.overhang_watson_3prime is not None and not isinstance(self.overhang_watson_3prime, int):
             self.overhang_watson_3prime = int(self.overhang_watson_3prime)
 
+        if self.file_content is not None and not isinstance(self.file_content, str):
+            self.file_content = str(self.file_content)
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class Primer(Sequence):
     """
@@ -283,22 +280,26 @@
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["SequenceCut"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:SequenceCut"
     class_name: ClassVar[str] = "SequenceCut"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.SequenceCut
 
-    cut_watson: Optional[int] = None
-    overhang: Optional[int] = None
+    cut_watson: int = None
+    overhang: int = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.cut_watson is not None and not isinstance(self.cut_watson, int):
+        if self._is_empty(self.cut_watson):
+            self.MissingRequiredField("cut_watson")
+        if not isinstance(self.cut_watson, int):
             self.cut_watson = int(self.cut_watson)
 
-        if self.overhang is not None and not isinstance(self.overhang, int):
+        if self._is_empty(self.overhang):
+            self.MissingRequiredField("overhang")
+        if not isinstance(self.overhang, int):
             self.overhang = int(self.overhang)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RestrictionSequenceCut(SequenceCut):
@@ -309,14 +310,16 @@
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["RestrictionSequenceCut"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:RestrictionSequenceCut"
     class_name: ClassVar[str] = "RestrictionSequenceCut"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.RestrictionSequenceCut
 
+    cut_watson: int = None
+    overhang: int = None
     restriction_enzyme: str = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.restriction_enzyme):
             self.MissingRequiredField("restriction_enzyme")
         if not isinstance(self.restriction_enzyme, str):
             self.restriction_enzyme = str(self.restriction_enzyme)
@@ -382,27 +385,35 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["ManuallyTypedSource"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:ManuallyTypedSource"
     class_name: ClassVar[str] = "ManuallyTypedSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.ManuallyTypedSource
 
     id: Union[int, ManuallyTypedSourceId] = None
     user_input: str = None
+    overhang_crick_3prime: Optional[int] = 0
+    overhang_watson_3prime: Optional[int] = 0
     circular: Optional[Union[bool, Bool]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ManuallyTypedSourceId):
             self.id = ManuallyTypedSourceId(self.id)
 
         if self._is_empty(self.user_input):
             self.MissingRequiredField("user_input")
         if not isinstance(self.user_input, str):
             self.user_input = str(self.user_input)
 
+        if self.overhang_crick_3prime is not None and not isinstance(self.overhang_crick_3prime, int):
+            self.overhang_crick_3prime = int(self.overhang_crick_3prime)
+
+        if self.overhang_watson_3prime is not None and not isinstance(self.overhang_watson_3prime, int):
+            self.overhang_watson_3prime = int(self.overhang_watson_3prime)
+
         if self.circular is not None and not isinstance(self.circular, Bool):
             self.circular = Bool(self.circular)
 
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
@@ -479,14 +490,49 @@
             self.repository_id = str(self.repository_id)
 
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
+class AddGeneIdSource(RepositoryIdSource):
+    """
+    Represents the source of a sequence that is identified by an AddGene id
+    """
+
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["AddGeneIdSource"]
+    class_class_curie: ClassVar[str] = "shareyourcloning_linkml:AddGeneIdSource"
+    class_name: ClassVar[str] = "AddGeneIdSource"
+    class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.AddGeneIdSource
+
+    id: Union[int, AddGeneIdSourceId] = None
+    repository_name: Union[str, "RepositoryName"] = None
+    repository_id: str = None
+    sequence_file_url: Optional[str] = None
+    addgene_sequence_type: Optional[Union[str, "AddGeneSequenceType"]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, AddGeneIdSourceId):
+            self.id = AddGeneIdSourceId(self.id)
+
+        if self.sequence_file_url is not None and not isinstance(self.sequence_file_url, str):
+            self.sequence_file_url = str(self.sequence_file_url)
+
+        if self.addgene_sequence_type is not None and not isinstance(self.addgene_sequence_type, AddGeneSequenceType):
+            self.addgene_sequence_type = AddGeneSequenceType(self.addgene_sequence_type)
+
+        super().__post_init__(**kwargs)
+        self.type = str(self.class_name)
+
+
+@dataclass
 class GenomeCoordinatesSource(Source):
     """
     Represents the source of a sequence that is identified by genome coordinates, requested from NCBI
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
@@ -555,27 +601,32 @@
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:SequenceCutSource"
     class_name: ClassVar[str] = "SequenceCutSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.SequenceCutSource
 
     id: Union[int, SequenceCutSourceId] = None
     left_edge: Optional[Union[dict, SequenceCut]] = None
     right_edge: Optional[Union[dict, SequenceCut]] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, SequenceCutSourceId):
             self.id = SequenceCutSourceId(self.id)
 
         if self.left_edge is not None and not isinstance(self.left_edge, SequenceCut):
             self.left_edge = SequenceCut(**as_dict(self.left_edge))
 
         if self.right_edge is not None and not isinstance(self.right_edge, SequenceCut):
             self.right_edge = SequenceCut(**as_dict(self.right_edge))
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class RestrictionEnzymeDigestionSource(SequenceCutSource):
     """
@@ -735,14 +786,15 @@
     class_name: ClassVar[str] = "PCRSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.PCRSource
 
     id: Union[int, PCRSourceId] = None
     assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
     forward_primer: Union[int, PrimerId] = None
     reverse_primer: Union[int, PrimerId] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, PCRSourceId):
             self.id = PCRSourceId(self.id)
 
@@ -752,14 +804,18 @@
             self.forward_primer = PrimerId(self.forward_primer)
 
         if self._is_empty(self.reverse_primer):
             self.MissingRequiredField("reverse_primer")
         if not isinstance(self.reverse_primer, PrimerId):
             self.reverse_primer = PrimerId(self.reverse_primer)
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class LigationSource(AssemblySource):
     """
@@ -771,21 +827,26 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["LigationSource"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:LigationSource"
     class_name: ClassVar[str] = "LigationSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.LigationSource
 
     id: Union[int, LigationSourceId] = None
     assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, LigationSourceId):
             self.id = LigationSourceId(self.id)
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class HomologousRecombinationSource(AssemblySource):
     """
@@ -797,21 +858,26 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["HomologousRecombinationSource"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:HomologousRecombinationSource"
     class_name: ClassVar[str] = "HomologousRecombinationSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.HomologousRecombinationSource
 
     id: Union[int, HomologousRecombinationSourceId] = None
     assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, HomologousRecombinationSourceId):
             self.id = HomologousRecombinationSourceId(self.id)
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class GibsonAssemblySource(AssemblySource):
     """
@@ -823,21 +889,26 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["GibsonAssemblySource"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:GibsonAssemblySource"
     class_name: ClassVar[str] = "GibsonAssemblySource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.GibsonAssemblySource
 
     id: Union[int, GibsonAssemblySourceId] = None
     assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, GibsonAssemblySourceId):
             self.id = GibsonAssemblySourceId(self.id)
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class RestrictionAndLigationSource(AssemblySource):
     """
@@ -850,27 +921,65 @@
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:RestrictionAndLigationSource"
     class_name: ClassVar[str] = "RestrictionAndLigationSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.RestrictionAndLigationSource
 
     id: Union[int, RestrictionAndLigationSourceId] = None
     assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
     restriction_enzymes: Union[str, List[str]] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, RestrictionAndLigationSourceId):
             self.id = RestrictionAndLigationSourceId(self.id)
 
         if self._is_empty(self.restriction_enzymes):
             self.MissingRequiredField("restriction_enzymes")
         if not isinstance(self.restriction_enzymes, list):
             self.restriction_enzymes = [self.restriction_enzymes] if self.restriction_enzymes is not None else []
         self.restriction_enzymes = [v if isinstance(v, str) else str(v) for v in self.restriction_enzymes]
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
+        super().__post_init__(**kwargs)
+        self.type = str(self.class_name)
+
+
+@dataclass
+class CRISPRSource(HomologousRecombinationSource):
+    """
+    Represents the source of a sequence that is generated by CRISPR
+    """
+
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["CRISPRSource"]
+    class_class_curie: ClassVar[str] = "shareyourcloning_linkml:CRISPRSource"
+    class_name: ClassVar[str] = "CRISPRSource"
+    class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.CRISPRSource
+
+    id: Union[int, CRISPRSourceId] = None
+    assembly: Union[Union[dict, AssemblyJoin], List[Union[dict, AssemblyJoin]]] = None
+    guides: Union[Union[int, PrimerId], List[Union[int, PrimerId]]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, CRISPRSourceId):
+            self.id = CRISPRSourceId(self.id)
+
+        if self._is_empty(self.guides):
+            self.MissingRequiredField("guides")
+        if not isinstance(self.guides, list):
+            self.guides = [self.guides] if self.guides is not None else []
+        self.guides = [v if isinstance(v, PrimerId) else PrimerId(v) for v in self.guides]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class OligoHybridizationSource(Source):
     """
@@ -922,21 +1031,26 @@
 
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["PolymeraseExtensionSource"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:PolymeraseExtensionSource"
     class_name: ClassVar[str] = "PolymeraseExtensionSource"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.PolymeraseExtensionSource
 
     id: Union[int, PolymeraseExtensionSourceId] = None
+    input: Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, PolymeraseExtensionSourceId):
             self.id = PolymeraseExtensionSourceId(self.id)
 
+        if not isinstance(self.input, list):
+            self.input = [self.input] if self.input is not None else []
+        self.input = [v if isinstance(v, SequenceId) else SequenceId(v) for v in self.input]
+
         super().__post_init__(**kwargs)
         self.type = str(self.class_name)
 
 
 @dataclass
 class CloningStrategy(YAMLRoot):
     """
@@ -992,14 +1106,36 @@
     snapgene = PermissibleValue(text="snapgene")
 
     _defn = EnumDefinition(
         name="SequenceFileFormat",
     )
 
 
+class AddGeneSequenceType(EnumDefinitionImpl):
+
+    _defn = EnumDefinition(
+        name="AddGeneSequenceType",
+    )
+
+    @classmethod
+    def _addvals(cls):
+        setattr(
+            cls,
+            "depositor-full",
+            PermissibleValue(
+                text="depositor-full", description="Full sequence of the plasmid submitted by the depositor"
+            ),
+        )
+        setattr(
+            cls,
+            "addgene-full",
+            PermissibleValue(text="addgene-full", description="Full sequence of the plasmid performed by Addgene"),
+        )
+
+
 # Slots
 class slots:
     pass
 
 
 slots.id = Slot(
     uri=SCHEMA.identifier,
@@ -1069,41 +1205,53 @@
     name="sequence_file_format",
     curie=SHAREYOURCLONING_LINKML.curie("sequence_file_format"),
     model_uri=SHAREYOURCLONING_LINKML.sequence_file_format,
     domain=None,
     range=Optional[Union[str, "SequenceFileFormat"]],
 )
 
-slots.textFileSequence__file_content = Slot(
-    uri=SHAREYOURCLONING_LINKML.file_content,
-    name="textFileSequence__file_content",
-    curie=SHAREYOURCLONING_LINKML.curie("file_content"),
-    model_uri=SHAREYOURCLONING_LINKML.textFileSequence__file_content,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.textFileSequence__overhang_crick_3prime = Slot(
+slots.overhang_crick_3prime = Slot(
     uri=SHAREYOURCLONING_LINKML.overhang_crick_3prime,
-    name="textFileSequence__overhang_crick_3prime",
+    name="overhang_crick_3prime",
     curie=SHAREYOURCLONING_LINKML.curie("overhang_crick_3prime"),
-    model_uri=SHAREYOURCLONING_LINKML.textFileSequence__overhang_crick_3prime,
+    model_uri=SHAREYOURCLONING_LINKML.overhang_crick_3prime,
     domain=None,
     range=Optional[int],
 )
 
-slots.textFileSequence__overhang_watson_3prime = Slot(
+slots.overhang_watson_3prime = Slot(
     uri=SHAREYOURCLONING_LINKML.overhang_watson_3prime,
-    name="textFileSequence__overhang_watson_3prime",
+    name="overhang_watson_3prime",
     curie=SHAREYOURCLONING_LINKML.curie("overhang_watson_3prime"),
-    model_uri=SHAREYOURCLONING_LINKML.textFileSequence__overhang_watson_3prime,
+    model_uri=SHAREYOURCLONING_LINKML.overhang_watson_3prime,
     domain=None,
     range=Optional[int],
 )
 
+slots.sequence_file_url = Slot(
+    uri=SHAREYOURCLONING_LINKML.sequence_file_url,
+    name="sequence_file_url",
+    curie=SHAREYOURCLONING_LINKML.curie("sequence_file_url"),
+    model_uri=SHAREYOURCLONING_LINKML.sequence_file_url,
+    domain=None,
+    range=Optional[str],
+    pattern=re.compile(
+        r"^https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$"
+    ),
+)
+
+slots.textFileSequence__file_content = Slot(
+    uri=SHAREYOURCLONING_LINKML.file_content,
+    name="textFileSequence__file_content",
+    curie=SHAREYOURCLONING_LINKML.curie("file_content"),
+    model_uri=SHAREYOURCLONING_LINKML.textFileSequence__file_content,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.primer__sequence = Slot(
     uri=SHAREYOURCLONING_LINKML.sequence,
     name="primer__sequence",
     curie=SHAREYOURCLONING_LINKML.curie("sequence"),
     model_uri=SHAREYOURCLONING_LINKML.primer__sequence,
     domain=None,
     range=Optional[str],
@@ -1112,24 +1260,24 @@
 
 slots.sequenceCut__cut_watson = Slot(
     uri=SHAREYOURCLONING_LINKML.cut_watson,
     name="sequenceCut__cut_watson",
     curie=SHAREYOURCLONING_LINKML.curie("cut_watson"),
     model_uri=SHAREYOURCLONING_LINKML.sequenceCut__cut_watson,
     domain=None,
-    range=Optional[int],
+    range=int,
 )
 
 slots.sequenceCut__overhang = Slot(
     uri=SHAREYOURCLONING_LINKML.overhang,
     name="sequenceCut__overhang",
     curie=SHAREYOURCLONING_LINKML.curie("overhang"),
     model_uri=SHAREYOURCLONING_LINKML.sequenceCut__overhang,
     domain=None,
-    range=Optional[int],
+    range=int,
 )
 
 slots.manuallyTypedSource__user_input = Slot(
     uri=SHAREYOURCLONING_LINKML.user_input,
     name="manuallyTypedSource__user_input",
     curie=SHAREYOURCLONING_LINKML.curie("user_input"),
     model_uri=SHAREYOURCLONING_LINKML.manuallyTypedSource__user_input,
@@ -1179,14 +1327,23 @@
     name="repositoryIdSource__repository_id",
     curie=SHAREYOURCLONING_LINKML.curie("repository_id"),
     model_uri=SHAREYOURCLONING_LINKML.repositoryIdSource__repository_id,
     domain=None,
     range=str,
 )
 
+slots.addGeneIdSource__addgene_sequence_type = Slot(
+    uri=SHAREYOURCLONING_LINKML.addgene_sequence_type,
+    name="addGeneIdSource__addgene_sequence_type",
+    curie=SHAREYOURCLONING_LINKML.curie("addgene_sequence_type"),
+    model_uri=SHAREYOURCLONING_LINKML.addGeneIdSource__addgene_sequence_type,
+    domain=None,
+    range=Optional[Union[str, "AddGeneSequenceType"]],
+)
+
 slots.genomeCoordinatesSource__assembly_accession = Slot(
     uri=SHAREYOURCLONING_LINKML.assembly_accession,
     name="genomeCoordinatesSource__assembly_accession",
     curie=SHAREYOURCLONING_LINKML.curie("assembly_accession"),
     model_uri=SHAREYOURCLONING_LINKML.genomeCoordinatesSource__assembly_accession,
     domain=None,
     range=Optional[str],
@@ -1377,14 +1534,23 @@
     name="pCRSource__reverse_primer",
     curie=SHAREYOURCLONING_LINKML.curie("reverse_primer"),
     model_uri=SHAREYOURCLONING_LINKML.pCRSource__reverse_primer,
     domain=None,
     range=Union[int, PrimerId],
 )
 
+slots.cRISPRSource__guides = Slot(
+    uri=SHAREYOURCLONING_LINKML.guides,
+    name="cRISPRSource__guides",
+    curie=SHAREYOURCLONING_LINKML.curie("guides"),
+    model_uri=SHAREYOURCLONING_LINKML.cRISPRSource__guides,
+    domain=None,
+    range=Union[Union[int, PrimerId], List[Union[int, PrimerId]]],
+)
+
 slots.oligoHybridizationSource__forward_oligo = Slot(
     uri=SHAREYOURCLONING_LINKML.forward_oligo,
     name="oligoHybridizationSource__forward_oligo",
     curie=SHAREYOURCLONING_LINKML.curie("forward_oligo"),
     model_uri=SHAREYOURCLONING_LINKML.oligoHybridizationSource__forward_oligo,
     domain=None,
     range=Union[int, PrimerId],
@@ -1395,23 +1561,14 @@
     name="oligoHybridizationSource__reverse_oligo",
     curie=SHAREYOURCLONING_LINKML.curie("reverse_oligo"),
     model_uri=SHAREYOURCLONING_LINKML.oligoHybridizationSource__reverse_oligo,
     domain=None,
     range=Union[int, PrimerId],
 )
 
-slots.oligoHybridizationSource__overhang_crick_3prime = Slot(
-    uri=SHAREYOURCLONING_LINKML.overhang_crick_3prime,
-    name="oligoHybridizationSource__overhang_crick_3prime",
-    curie=SHAREYOURCLONING_LINKML.curie("overhang_crick_3prime"),
-    model_uri=SHAREYOURCLONING_LINKML.oligoHybridizationSource__overhang_crick_3prime,
-    domain=None,
-    range=Optional[int],
-)
-
 slots.cloningStrategy__sequences = Slot(
     uri=SHAREYOURCLONING_LINKML.sequences,
     name="cloningStrategy__sequences",
     curie=SHAREYOURCLONING_LINKML.curie("sequences"),
     model_uri=SHAREYOURCLONING_LINKML.cloningStrategy__sequences,
     domain=None,
     range=Union[Dict[Union[int, SequenceId], Union[dict, Sequence]], List[Union[dict, Sequence]]],
@@ -1449,33 +1606,132 @@
     name="TextFileSequence_sequence_file_format",
     curie=SHAREYOURCLONING_LINKML.curie("sequence_file_format"),
     model_uri=SHAREYOURCLONING_LINKML.TextFileSequence_sequence_file_format,
     domain=TextFileSequence,
     range=Union[str, "SequenceFileFormat"],
 )
 
+slots.TextFileSequence_overhang_crick_3prime = Slot(
+    uri=SHAREYOURCLONING_LINKML.overhang_crick_3prime,
+    name="TextFileSequence_overhang_crick_3prime",
+    curie=SHAREYOURCLONING_LINKML.curie("overhang_crick_3prime"),
+    model_uri=SHAREYOURCLONING_LINKML.TextFileSequence_overhang_crick_3prime,
+    domain=TextFileSequence,
+    range=Optional[int],
+)
+
+slots.TextFileSequence_overhang_watson_3prime = Slot(
+    uri=SHAREYOURCLONING_LINKML.overhang_watson_3prime,
+    name="TextFileSequence_overhang_watson_3prime",
+    curie=SHAREYOURCLONING_LINKML.curie("overhang_watson_3prime"),
+    model_uri=SHAREYOURCLONING_LINKML.TextFileSequence_overhang_watson_3prime,
+    domain=TextFileSequence,
+    range=Optional[int],
+)
+
 slots.RestrictionSequenceCut_restriction_enzyme = Slot(
     uri=SHAREYOURCLONING_LINKML.restriction_enzyme,
     name="RestrictionSequenceCut_restriction_enzyme",
     curie=SHAREYOURCLONING_LINKML.curie("restriction_enzyme"),
     model_uri=SHAREYOURCLONING_LINKML.RestrictionSequenceCut_restriction_enzyme,
     domain=RestrictionSequenceCut,
     range=str,
 )
 
+slots.ManuallyTypedSource_overhang_crick_3prime = Slot(
+    uri=SHAREYOURCLONING_LINKML.overhang_crick_3prime,
+    name="ManuallyTypedSource_overhang_crick_3prime",
+    curie=SHAREYOURCLONING_LINKML.curie("overhang_crick_3prime"),
+    model_uri=SHAREYOURCLONING_LINKML.ManuallyTypedSource_overhang_crick_3prime,
+    domain=ManuallyTypedSource,
+    range=Optional[int],
+)
+
+slots.ManuallyTypedSource_overhang_watson_3prime = Slot(
+    uri=SHAREYOURCLONING_LINKML.overhang_watson_3prime,
+    name="ManuallyTypedSource_overhang_watson_3prime",
+    curie=SHAREYOURCLONING_LINKML.curie("overhang_watson_3prime"),
+    model_uri=SHAREYOURCLONING_LINKML.ManuallyTypedSource_overhang_watson_3prime,
+    domain=ManuallyTypedSource,
+    range=Optional[int],
+)
+
 slots.UploadedFileSource_sequence_file_format = Slot(
     uri=SHAREYOURCLONING_LINKML.sequence_file_format,
     name="UploadedFileSource_sequence_file_format",
     curie=SHAREYOURCLONING_LINKML.curie("sequence_file_format"),
     model_uri=SHAREYOURCLONING_LINKML.UploadedFileSource_sequence_file_format,
     domain=UploadedFileSource,
     range=Union[str, "SequenceFileFormat"],
 )
 
+slots.SequenceCutSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="SequenceCutSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.SequenceCutSource_input,
+    domain=SequenceCutSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
+slots.PCRSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="PCRSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.PCRSource_input,
+    domain=PCRSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
+slots.LigationSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="LigationSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.LigationSource_input,
+    domain=LigationSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
+slots.HomologousRecombinationSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="HomologousRecombinationSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.HomologousRecombinationSource_input,
+    domain=HomologousRecombinationSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
+slots.GibsonAssemblySource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="GibsonAssemblySource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.GibsonAssemblySource_input,
+    domain=GibsonAssemblySource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
 slots.RestrictionAndLigationSource_restriction_enzymes = Slot(
     uri=SHAREYOURCLONING_LINKML.restriction_enzymes,
     name="RestrictionAndLigationSource_restriction_enzymes",
     curie=SHAREYOURCLONING_LINKML.curie("restriction_enzymes"),
     model_uri=SHAREYOURCLONING_LINKML.RestrictionAndLigationSource_restriction_enzymes,
     domain=RestrictionAndLigationSource,
     range=Union[str, List[str]],
 )
+
+slots.RestrictionAndLigationSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="RestrictionAndLigationSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.RestrictionAndLigationSource_input,
+    domain=RestrictionAndLigationSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
+
+slots.PolymeraseExtensionSource_input = Slot(
+    uri=SHAREYOURCLONING_LINKML.input,
+    name="PolymeraseExtensionSource_input",
+    curie=SHAREYOURCLONING_LINKML.curie("input"),
+    model_uri=SHAREYOURCLONING_LINKML.PolymeraseExtensionSource_input,
+    domain=PolymeraseExtensionSource,
+    range=Optional[Union[Union[int, SequenceId], List[Union[int, SequenceId]]]],
+)
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/shacl/shareyourcloning_linkml.shacl.ttl` & `shareyourcloning_linkml-0.1.3a0/project/shacl/shareyourcloning_linkml.shacl.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,73 @@
     sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path schema1:identifier ] ;
     sh:targetClass schema1:Thing .
 
+shareyourcloning_linkml:AddGeneIdSource a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents the source of a sequence that is identified by an AddGene id" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:in ( "depositor-full" "addgene-full" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:addgene_sequence_type ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:in ( "addgene" "genbank" ) ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:repository_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "The id of the sequence in the repository" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:repository_id ],
+        [ sh:datatype xsd:string ;
+            sh:description "The URL of a sequence file" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence_file_url ;
+            sh:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 7 ;
+            sh:path schema1:identifier ] ;
+    sh:targetClass shareyourcloning_linkml:AddGeneIdSource .
+
 shareyourcloning_linkml:AssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is an assembly of other sequences" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:boolean ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
@@ -31,177 +85,250 @@
             sh:path shareyourcloning_linkml:assembly ],
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
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ] ;
+    sh:targetClass shareyourcloning_linkml:AssemblySource .
+
+shareyourcloning_linkml:CRISPRSource a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents the source of a sequence that is generated by CRISPR" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+        [ sh:class shareyourcloning_linkml:Primer ;
+            sh:description "The guide RNAs used in the CRISPR" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:guides ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+            sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:assembly ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ] ;
-    sh:targetClass shareyourcloning_linkml:AssemblySource .
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ] ;
+    sh:targetClass shareyourcloning_linkml:CRISPRSource .
 
 shareyourcloning_linkml:CloningStrategy a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cloning strategy" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Source ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are used in the cloning strategy" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequences ],
+        [ sh:class shareyourcloning_linkml:Source ;
             sh:description "The sources of the sequences that are used in the cloning strategy" ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:sources ],
         [ sh:datatype xsd:string ;
             sh:description "A description of the cloning strategy" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:description ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are used in the cloning strategy" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequences ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The primers that are used in the cloning strategy" ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:primers ] ;
     sh:targetClass shareyourcloning_linkml:CloningStrategy .
 
 shareyourcloning_linkml:GenomeCoordinatesSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "The strand of the sequence in the sequence accession, should be 1 or -1" ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "The locus tag of the sequence" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:strand ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:locus_tag ],
         [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+            sh:description "The starting coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 10 ;
-            sh:path schema1:identifier ],
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:start ],
         [ sh:datatype xsd:integer ;
             sh:description "The ending coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:end ],
-        [ sh:datatype xsd:string ;
-            sh:description "The locus tag of the sequence" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:locus_tag ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:string ;
-            sh:description "The accession of the sequence" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sequence_accession ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 8 ;
             sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
-            sh:description "The starting coordinate (1-based) of the sequence in the sequence accession" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:start ],
-        [ sh:datatype xsd:string ;
-            sh:description "The accession of the assembly" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:assembly_accession ],
-        [ sh:datatype xsd:integer ;
             sh:description "The gene id of the sequence" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:gene_id ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 7 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The accession of the assembly" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:assembly_accession ],
+        [ sh:datatype xsd:string ;
+            sh:description "The accession of the sequence" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sequence_accession ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 10 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The strand of the sequence in the sequence accession, should be 1 or -1" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:strand ] ;
     sh:targetClass shareyourcloning_linkml:GenomeCoordinatesSource .
 
 shareyourcloning_linkml:GibsonAssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by Gibson assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+            sh:description "The joins between the fragments in the assembly" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ] ;
+    sh:targetClass shareyourcloning_linkml:GibsonAssemblySource .
+
+shareyourcloning_linkml:HomologousRecombinationSource a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents the source of a sequence that is generated by homologous recombination" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ] ;
-    sh:targetClass shareyourcloning_linkml:GibsonAssemblySource .
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ] ;
+    sh:targetClass shareyourcloning_linkml:HomologousRecombinationSource .
 
-shareyourcloning_linkml:HomologousRecombinationSource a sh:NodeShape ;
+shareyourcloning_linkml:LigationSource a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Represents the source of a sequence that is generated by homologous recombination" ;
+    sh:description "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoin ;
-            sh:description "The joins between the fragments in the assembly" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ],
-        [ sh:datatype xsd:string ;
+    sh:property [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
@@ -209,103 +336,82 @@
             sh:order 5 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ] ;
-    sh:targetClass shareyourcloning_linkml:HomologousRecombinationSource .
-
-shareyourcloning_linkml:LigationSource a sh:NodeShape ;
-    sh:closed true ;
-    sh:description "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
-    sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ] ;
+            sh:path shareyourcloning_linkml:assembly ] ;
     sh:targetClass shareyourcloning_linkml:LigationSource .
 
 shareyourcloning_linkml:ManuallyTypedSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is manually typed by the user" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:user_input ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the sequence is circular or not" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:path shareyourcloning_linkml:circular ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 5 ;
+            sh:order 7 ;
             sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:user_input ;
+            sh:pattern "^[acgtACGT]+$" ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
+            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:overhang_crick_3prime ],
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
+            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ] ;
     sh:targetClass shareyourcloning_linkml:ManuallyTypedSource .
 
 shareyourcloning_linkml:OligoHybridizationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by oligo hybridization" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
@@ -317,113 +423,113 @@
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Primer ;
+            sh:description "The reverse oligo used in the hybridization" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:reverse_oligo ],
+        [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The forward oligo used in the hybridization" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 0 ;
+            sh:order 1 ;
             sh:path shareyourcloning_linkml:forward_oligo ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Primer ;
-            sh:description "The reverse oligo used in the hybridization" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:reverse_oligo ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
-            sh:description "The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand." ;
+            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
+            sh:order 0 ;
             sh:path shareyourcloning_linkml:overhang_crick_3prime ] ;
     sh:targetClass shareyourcloning_linkml:OligoHybridizationSource .
 
 shareyourcloning_linkml:PCRSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by PCR" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 7 ;
             sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Primer ;
-            sh:description "The forward primer used in the PCR" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:forward_primer ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:circular ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:assembly ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:class shareyourcloning_linkml:Primer ;
+            sh:description "The forward primer used in the PCR" ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:forward_primer ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The reverse primer used in the PCR" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:reverse_primer ] ;
+            sh:path shareyourcloning_linkml:reverse_primer ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:PCRSource .
 
 shareyourcloning_linkml:PolymeraseExtensionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by polymerase extension" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
@@ -432,351 +538,357 @@
             sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:PolymeraseExtensionSource .
 
 shareyourcloning_linkml:RepositoryIdSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by a repository id" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "The id of the sequence in the repository" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:repository_id ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:in ( "addgene" "genbank" ) ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:repository_name ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:string ;
-            sh:description "The id of the sequence in the repository" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:repository_id ],
-        [ sh:in ( "addgene" "genbank" ) ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:repository_name ] ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:RepositoryIdSource .
 
 shareyourcloning_linkml:RestrictionAndLigationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by restriction and ligation" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:restriction_enzymes ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
-            sh:description "The joins between the fragments in the assembly" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:assembly ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+    sh:property [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:circular ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
+        [ sh:datatype xsd:string ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:restriction_enzymes ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+            sh:description "The joins between the fragments in the assembly" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:input ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionAndLigationSource .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:right_edge ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:left_edge ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:right_edge ] ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 shareyourcloning_linkml:SequenceCutSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:SequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:left_edge ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:SequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_edge ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:right_edge ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:SequenceCut ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:right_edge ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ] ;
     sh:targetClass shareyourcloning_linkml:SequenceCutSource .
 
 shareyourcloning_linkml:TextFileSequence a sh:NodeShape ;
     sh:closed true ;
     sh:description "A sequence (may have features) defined by the content of a text file" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
             sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
+            sh:order 1 ;
             sh:path shareyourcloning_linkml:overhang_crick_3prime ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:description "The format of a sequence file" ;
             sh:in ( "fasta" "genbank" "snapgene" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:sequence_file_format ],
         [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+            sh:defaultValue 0 ;
+            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 1 ;
+            sh:order 3 ;
             sh:path shareyourcloning_linkml:file_content ],
-        [ sh:datatype xsd:integer ;
-            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:overhang_watson_3prime ] ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:TextFileSequence .
 
 shareyourcloning_linkml:UploadedFileSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is uploaded as a file" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:string ;
             sh:description "The name of the file" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:file_name ],
         [ sh:description "The format of a sequence file" ;
             sh:in ( "fasta" "genbank" "snapgene" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:sequence_file_format ],
-        [ sh:datatype xsd:integer ;
-            sh:description "The index of the sequence in the file" ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:index_in_file ],
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 6 ;
             sh:path schema1:identifier ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The index of the sequence in the file" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:index_in_file ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:input ] ;
+            sh:path shareyourcloning_linkml:output ] ;
     sh:targetClass shareyourcloning_linkml:UploadedFileSource .
 
 shareyourcloning_linkml:Source a sh:NodeShape ;
     sh:closed false ;
     sh:description "Represents the source of a sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:input ] ;
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:Source .
 
 shareyourcloning_linkml:RestrictionSequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence that is made by a restriction enzyme" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
             sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:overhang ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:restriction_enzyme ],
         [ sh:datatype xsd:integer ;
             sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:cut_watson ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionSequenceCut .
 
 shareyourcloning_linkml:SequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
             sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:cut_watson ],
         [ sh:datatype xsd:integer ;
             sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:overhang ] ;
     sh:targetClass shareyourcloning_linkml:SequenceCut .
 
 shareyourcloning_linkml:SimpleSequenceLocation a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a location within a sequence, for now support for ranges only" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
-            sh:description "The strand of the location, should be 1 or -1 or null" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:strand ],
-        [ sh:datatype xsd:integer ;
             sh:description "The ending coordinate (1-based) of the location" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:end ],
         [ sh:datatype xsd:integer ;
             sh:description "The starting coordinate (1-based) of the location" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
-            sh:path shareyourcloning_linkml:start ] ;
+            sh:path shareyourcloning_linkml:start ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The strand of the location, should be 1 or -1 or null" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:strand ] ;
     sh:targetClass shareyourcloning_linkml:SimpleSequenceLocation .
 
 shareyourcloning_linkml:Primer a sh:NodeShape ;
     sh:closed true ;
     sh:description "An oligonucleotide or primer" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sequence ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a thing" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sequence ;
+            sh:pattern "^[acgtACGT]+$" ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
@@ -790,47 +902,48 @@
     sh:closed true ;
     sh:description "Represents a joint between two fragments in an assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:right_fragment ],
-        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
-            sh:description "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join." ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:left_location ],
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:left_fragment ],
         [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
             sh:description "Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:right_location ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_fragment ] ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:right_fragment ],
+        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
+            sh:description "Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:left_location ] ;
     sh:targetClass shareyourcloning_linkml:AssemblyJoin .
 
 shareyourcloning_linkml:Sequence a sh:NodeShape ;
     sh:closed false ;
     sh:description "Represents a sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:Sequence .
+
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/shex/shareyourcloning_linkml.shex` & `shareyourcloning_linkml-0.1.3a0/project/shex/shareyourcloning_linkml.shex`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,25 @@
 
 linkml:Jsonpointer xsd:string
 
 linkml:Jsonpath xsd:string
 
 linkml:Sparqlpath xsd:string
 
+<AddGeneIdSource> CLOSED {
+    (  $<AddGeneIdSource_tes> (  &<RepositoryIdSource_tes> ;
+          rdf:type [ <RepositoryIdSource> ] ? ;
+          <sequence_file_url> @linkml:String ? ;
+          <addgene_sequence_type> [ <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#depositor-full>
+             <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full> ] ?
+       ) ;
+       rdf:type [ <AddGeneIdSource> ]
+    )
+}
+
 <AssemblyJoin> CLOSED {
     (  $<AssemblyJoin_tes> (  <left_fragment> @<Sequence> ;
           <right_fragment> @<Sequence> ;
           <left_location> @<SimpleSequenceLocation> ;
           <right_location> @<SimpleSequenceLocation>
        ) ;
        rdf:type [ <AssemblyJoin> ] ?
@@ -72,14 +83,23 @@
           <primers> @<Primer> * ;
           <description> @linkml:String ?
        ) ;
        rdf:type [ <CloningStrategy> ] ?
     )
 }
 
+<CRISPRSource> CLOSED {
+    (  $<CRISPRSource_tes> (  &<HomologousRecombinationSource_tes> ;
+          rdf:type [ <HomologousRecombinationSource> ] ? ;
+          <guides> @<Primer> +
+       ) ;
+       rdf:type [ <CRISPRSource> ]
+    )
+}
+
 <GenomeCoordinatesSource> CLOSED {
     (  $<GenomeCoordinatesSource_tes> (  &<Source_tes> ;
           rdf:type [ <Source> ] ? ;
           <assembly_accession> @linkml:String ? ;
           <sequence_accession> @linkml:String ;
           <locus_tag> @linkml:String ? ;
           <gene_id> @linkml:Integer ? ;
@@ -89,39 +109,46 @@
        ) ;
        rdf:type [ <GenomeCoordinatesSource> ]
     )
 }
 
 <GibsonAssemblySource> CLOSED {
     (  $<GibsonAssemblySource_tes> (  &<AssemblySource_tes> ;
-          rdf:type [ <AssemblySource> ] ?
+          rdf:type [ <AssemblySource> ] ? ;
+          <input> @<Sequence> *
        ) ;
        rdf:type [ <GibsonAssemblySource> ]
     )
 }
 
-<HomologousRecombinationSource> CLOSED {
-    (  $<HomologousRecombinationSource_tes> (  &<AssemblySource_tes> ;
-          rdf:type [ <AssemblySource> ] ?
-       ) ;
-       rdf:type [ <HomologousRecombinationSource> ]
-    )
-}
+<HomologousRecombinationSource>  (
+    CLOSED {
+       (  $<HomologousRecombinationSource_tes> (  &<AssemblySource_tes> ;
+             rdf:type [ <AssemblySource> ] ? ;
+             <input> @<Sequence> *
+          ) ;
+          rdf:type [ <HomologousRecombinationSource> ]
+       )
+    } OR @<CRISPRSource>
+)
 
 <LigationSource> CLOSED {
     (  $<LigationSource_tes> (  &<AssemblySource_tes> ;
-          rdf:type [ <AssemblySource> ] ?
+          rdf:type [ <AssemblySource> ] ? ;
+          <input> @<Sequence> *
        ) ;
        rdf:type [ <LigationSource> ]
     )
 }
 
 <ManuallyTypedSource> CLOSED {
     (  $<ManuallyTypedSource_tes> (  &<Source_tes> ;
           rdf:type [ <Source> ] ? ;
+          <overhang_crick_3prime> @linkml:Integer ? ;
+          <overhang_watson_3prime> @linkml:Integer ? ;
           <user_input> @linkml:String ;
           <circular> @linkml:Boolean ?
        ) ;
        rdf:type [ <ManuallyTypedSource> ]
     )
 }
 
@@ -132,35 +159,37 @@
        )
     } OR @<Sequence> OR @<Source>
 )
 
 <OligoHybridizationSource> CLOSED {
     (  $<OligoHybridizationSource_tes> (  &<Source_tes> ;
           rdf:type [ <Source> ] ? ;
+          <overhang_crick_3prime> @linkml:Integer ? ;
           <forward_oligo> @<Primer> ;
-          <reverse_oligo> @<Primer> ;
-          <overhang_crick_3prime> @linkml:Integer ?
+          <reverse_oligo> @<Primer>
        ) ;
        rdf:type [ <OligoHybridizationSource> ]
     )
 }
 
 <PCRSource> CLOSED {
     (  $<PCRSource_tes> (  &<AssemblySource_tes> ;
           rdf:type [ <AssemblySource> ] ? ;
           <forward_primer> @<Primer> ;
-          <reverse_primer> @<Primer>
+          <reverse_primer> @<Primer> ;
+          <input> @<Sequence> *
        ) ;
        rdf:type [ <PCRSource> ]
     )
 }
 
 <PolymeraseExtensionSource> CLOSED {
     (  $<PolymeraseExtensionSource_tes> (  &<Source_tes> ;
-          rdf:type [ <Source> ] ?
+          rdf:type [ <Source> ] ? ;
+          <input> @<Sequence> *
        ) ;
        rdf:type [ <PolymeraseExtensionSource> ]
     )
 }
 
 <Primer> CLOSED {
     (  $<Primer_tes> (  &<Sequence_tes> ;
@@ -168,29 +197,32 @@
           schema1:name @linkml:String ? ;
           <sequence> @linkml:String ?
        ) ;
        rdf:type [ <Primer> ]
     )
 }
 
-<RepositoryIdSource> CLOSED {
-    (  $<RepositoryIdSource_tes> (  &<Source_tes> ;
-          rdf:type [ <Source> ] ? ;
-          <repository_name> [ <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#addgene>
-             <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#genbank> ] ;
-          <repository_id> @linkml:String
-       ) ;
-       rdf:type [ <RepositoryIdSource> ]
-    )
-}
+<RepositoryIdSource>  (
+    CLOSED {
+       (  $<RepositoryIdSource_tes> (  &<Source_tes> ;
+             rdf:type [ <Source> ] ? ;
+             <repository_name> [ <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#addgene>
+                <https://w3id.org/genestorian/ShareYourCloning_LinkML/RepositoryName#genbank> ] ;
+             <repository_id> @linkml:String
+          ) ;
+          rdf:type [ <RepositoryIdSource> ]
+       )
+    } OR @<AddGeneIdSource>
+)
 
 <RestrictionAndLigationSource> CLOSED {
     (  $<RestrictionAndLigationSource_tes> (  &<AssemblySource_tes> ;
           rdf:type [ <AssemblySource> ] ? ;
-          <restriction_enzymes> @linkml:String +
+          <restriction_enzymes> @linkml:String + ;
+          <input> @<Sequence> *
        ) ;
        rdf:type [ <RestrictionAndLigationSource> ]
     )
 }
 
 <RestrictionEnzymeDigestionSource> CLOSED {
     (  $<RestrictionEnzymeDigestionSource_tes> (  &<SequenceCutSource_tes> ;
@@ -222,28 +254,29 @@
        ) ;
        rdf:type [ <Sequence> ]
     )
 }
 
 <SequenceCut>  (
     CLOSED {
-       (  $<SequenceCut_tes> (  <cut_watson> @linkml:Integer ? ;
-             <overhang> @linkml:Integer ?
+       (  $<SequenceCut_tes> (  <cut_watson> @linkml:Integer ;
+             <overhang> @linkml:Integer
           ) ;
           rdf:type [ <SequenceCut> ] ?
        )
     } OR @<RestrictionSequenceCut>
 )
 
 <SequenceCutSource>  (
     CLOSED {
        (  $<SequenceCutSource_tes> (  &<Source_tes> ;
              rdf:type [ <Source> ] ? ;
              <left_edge> @<SequenceCut> ? ;
-             <right_edge> @<SequenceCut> ?
+             <right_edge> @<SequenceCut> ? ;
+             <input> @<Sequence> *
           ) ;
           rdf:type [ <SequenceCutSource> ]
        )
     } OR @<RestrictionEnzymeDigestionSource>
 )
 
 <SimpleSequenceLocation> CLOSED {
@@ -273,17 +306,17 @@
 
 <TextFileSequence> CLOSED {
     (  $<TextFileSequence_tes> (  &<Sequence_tes> ;
           rdf:type [ <Sequence> ] ? ;
           <sequence_file_format> [ <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta>
              <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#genbank>
              <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> ] ;
-          <file_content> @linkml:String ? ;
           <overhang_crick_3prime> @linkml:Integer ? ;
-          <overhang_watson_3prime> @linkml:Integer ?
+          <overhang_watson_3prime> @linkml:Integer ? ;
+          <file_content> @linkml:String ?
        ) ;
        rdf:type [ <TextFileSequence> ]
     )
 }
 
 <UploadedFileSource> CLOSED {
     (  $<UploadedFileSource_tes> (  &<Source_tes> ;
```

### Comparing `shareyourcloning_linkml-0.1.2a0/project/sqlschema/shareyourcloning_linkml.sql` & `shareyourcloning_linkml-0.1.3a0/project/sqlschema/shareyourcloning_linkml.sql`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "Sequence" Description: "Represents a sequence"
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 --     * Slot: CloningStrategy_id Description: Autocreated FK slot
 -- # Class: "TextFileSequence" Description: "A sequence (may have features) defined by the content of a text file"
 --     * Slot: sequence_file_format Description: The format of a sequence file
---     * Slot: file_content Description: 
 --     * Slot: overhang_crick_3prime Description: Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand
 --     * Slot: overhang_watson_3prime Description: The equivalent of `overhang_crick_3prime` but for the watson strand
+--     * Slot: file_content Description: 
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 -- # Class: "Primer" Description: "An oligonucleotide or primer"
 --     * Slot: name Description: A human-readable name for a thing
 --     * Slot: sequence Description: 
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
@@ -27,14 +27,16 @@
 --     * Slot: overhang Description: The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.
 -- # Class: "Source" Description: "Represents the source of a sequence"
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: CloningStrategy_id Description: Autocreated FK slot
 -- # Class: "ManuallyTypedSource" Description: "Represents the source of a sequence that is manually typed by the user"
+--     * Slot: overhang_crick_3prime Description: Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand
+--     * Slot: overhang_watson_3prime Description: The equivalent of `overhang_crick_3prime` but for the watson strand
 --     * Slot: user_input Description: 
 --     * Slot: circular Description: Whether the sequence is circular or not
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "UploadedFileSource" Description: "Represents the source of a sequence that is uploaded as a file"
 --     * Slot: sequence_file_format Description: The format of a sequence file
@@ -45,14 +47,22 @@
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "RepositoryIdSource" Description: "Represents the source of a sequence that is identified by a repository id"
 --     * Slot: repository_name Description: 
 --     * Slot: repository_id Description: The id of the sequence in the repository
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
+-- # Class: "AddGeneIdSource" Description: "Represents the source of a sequence that is identified by an AddGene id"
+--     * Slot: sequence_file_url Description: The URL of a sequence file
+--     * Slot: addgene_sequence_type Description: 
+--     * Slot: repository_name Description: 
+--     * Slot: repository_id Description: The id of the sequence in the repository
+--     * Slot: output Description: Identifier of the sequence that is the output of this source.
+--     * Slot: type Description: The type of the source
+--     * Slot: id Description: A unique identifier for a thing
 -- # Class: "GenomeCoordinatesSource" Description: "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI"
 --     * Slot: assembly_accession Description: The accession of the assembly
 --     * Slot: sequence_accession Description: The accession of the sequence
 --     * Slot: locus_tag Description: The locus tag of the sequence
 --     * Slot: gene_id Description: The gene id of the sequence
 --     * Slot: start Description: The starting coordinate (1-based) of the sequence in the sequence accession
 --     * Slot: end Description: The ending coordinate (1-based) of the sequence in the sequence accession
@@ -83,14 +93,15 @@
 --     * Slot: right_fragment Description: 
 --     * Slot: AssemblySource_id Description: Autocreated FK slot
 --     * Slot: PCRSource_id Description: Autocreated FK slot
 --     * Slot: LigationSource_id Description: Autocreated FK slot
 --     * Slot: HomologousRecombinationSource_id Description: Autocreated FK slot
 --     * Slot: GibsonAssemblySource_id Description: Autocreated FK slot
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
+--     * Slot: CRISPRSource_id Description: Autocreated FK slot
 --     * Slot: left_location_id Description: Location of the overlap in the left fragment. Might be an empty location (start == end) to indicate blunt join.
 --     * Slot: right_location_id Description: Location of the overlap in the right fragment. Might be an empty location (start == end) to indicate blunt join.
 -- # Class: "AssemblySource" Description: "Represents the source of a sequence that is an assembly of other sequences"
 --     * Slot: circular Description: Whether the assembly is circular or not
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
@@ -117,18 +128,23 @@
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "RestrictionAndLigationSource" Description: "Represents the source of a sequence that is generated by restriction and ligation"
 --     * Slot: circular Description: Whether the assembly is circular or not
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
+-- # Class: "CRISPRSource" Description: "Represents the source of a sequence that is generated by CRISPR"
+--     * Slot: circular Description: Whether the assembly is circular or not
+--     * Slot: output Description: Identifier of the sequence that is the output of this source.
+--     * Slot: type Description: The type of the source
+--     * Slot: id Description: A unique identifier for a thing
 -- # Class: "OligoHybridizationSource" Description: "Represents the source of a sequence that is generated by oligo hybridization"
+--     * Slot: overhang_crick_3prime Description: Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand
 --     * Slot: forward_oligo Description: The forward oligo used in the hybridization
 --     * Slot: reverse_oligo Description: The reverse oligo used in the hybridization
---     * Slot: overhang_crick_3prime Description: The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand.
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
 -- # Class: "PolymeraseExtensionSource" Description: "Represents the source of a sequence that is generated by polymerase extension"
 --     * Slot: output Description: Identifier of the sequence that is the output of this source.
 --     * Slot: type Description: The type of the source
 --     * Slot: id Description: A unique identifier for a thing
@@ -143,14 +159,17 @@
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "UploadedFileSource_input" Description: ""
 --     * Slot: UploadedFileSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "RepositoryIdSource_input" Description: ""
 --     * Slot: RepositoryIdSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
+-- # Class: "AddGeneIdSource_input" Description: ""
+--     * Slot: AddGeneIdSource_id Description: Autocreated FK slot
+--     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "GenomeCoordinatesSource_input" Description: ""
 --     * Slot: GenomeCoordinatesSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "SequenceCutSource_input" Description: ""
 --     * Slot: SequenceCutSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "RestrictionEnzymeDigestionSource_input" Description: ""
@@ -173,14 +192,20 @@
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "RestrictionAndLigationSource_restriction_enzymes" Description: ""
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
 --     * Slot: restriction_enzymes Description: 
 -- # Class: "RestrictionAndLigationSource_input" Description: ""
 --     * Slot: RestrictionAndLigationSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
+-- # Class: "CRISPRSource_guides" Description: ""
+--     * Slot: CRISPRSource_id Description: Autocreated FK slot
+--     * Slot: guides_id Description: The guide RNAs used in the CRISPR
+-- # Class: "CRISPRSource_input" Description: ""
+--     * Slot: CRISPRSource_id Description: Autocreated FK slot
+--     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "OligoHybridizationSource_input" Description: ""
 --     * Slot: OligoHybridizationSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "PolymeraseExtensionSource_input" Description: ""
 --     * Slot: PolymeraseExtensionSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "CloningStrategy_primers" Description: ""
@@ -189,39 +214,39 @@
 
 CREATE TABLE "NamedThing" (
 	id INTEGER NOT NULL, 
 	PRIMARY KEY (id)
 );
 CREATE TABLE "TextFileSequence" (
 	sequence_file_format VARCHAR(8) NOT NULL, 
-	file_content TEXT, 
 	overhang_crick_3prime INTEGER, 
 	overhang_watson_3prime INTEGER, 
+	file_content TEXT, 
 	id INTEGER NOT NULL, 
 	type TEXT, 
 	PRIMARY KEY (id)
 );
 CREATE TABLE "Primer" (
 	name TEXT, 
 	sequence TEXT, 
 	id INTEGER NOT NULL, 
 	type TEXT, 
 	PRIMARY KEY (id)
 );
 CREATE TABLE "SequenceCut" (
 	id INTEGER NOT NULL, 
-	cut_watson INTEGER, 
-	overhang INTEGER, 
+	cut_watson INTEGER NOT NULL, 
+	overhang INTEGER NOT NULL, 
 	PRIMARY KEY (id)
 );
 CREATE TABLE "RestrictionSequenceCut" (
 	id INTEGER NOT NULL, 
 	restriction_enzyme TEXT NOT NULL, 
-	cut_watson INTEGER, 
-	overhang INTEGER, 
+	cut_watson INTEGER NOT NULL, 
+	overhang INTEGER NOT NULL, 
 	PRIMARY KEY (id)
 );
 CREATE TABLE "SimpleSequenceLocation" (
 	id INTEGER NOT NULL, 
 	start INTEGER NOT NULL, 
 	"end" INTEGER NOT NULL, 
 	strand INTEGER, 
@@ -252,14 +277,16 @@
 	id INTEGER NOT NULL, 
 	"CloningStrategy_id" INTEGER, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(output) REFERENCES "Sequence" (id), 
 	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id)
 );
 CREATE TABLE "ManuallyTypedSource" (
+	overhang_crick_3prime INTEGER, 
+	overhang_watson_3prime INTEGER, 
 	user_input TEXT NOT NULL, 
 	circular BOOLEAN, 
 	output INTEGER, 
 	type TEXT, 
 	id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
@@ -279,14 +306,25 @@
 	repository_id TEXT NOT NULL, 
 	output INTEGER, 
 	type TEXT, 
 	id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
+CREATE TABLE "AddGeneIdSource" (
+	sequence_file_url TEXT, 
+	addgene_sequence_type VARCHAR(14), 
+	repository_name VARCHAR(7) NOT NULL, 
+	repository_id TEXT NOT NULL, 
+	output INTEGER, 
+	type TEXT, 
+	id INTEGER NOT NULL, 
+	PRIMARY KEY (id), 
+	FOREIGN KEY(output) REFERENCES "Sequence" (id)
+);
 CREATE TABLE "GenomeCoordinatesSource" (
 	assembly_accession TEXT, 
 	sequence_accession TEXT NOT NULL, 
 	locus_tag TEXT, 
 	gene_id INTEGER, 
 	start INTEGER NOT NULL, 
 	"end" INTEGER NOT NULL, 
@@ -367,18 +405,26 @@
 	circular BOOLEAN, 
 	output INTEGER, 
 	type TEXT, 
 	id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
 );
+CREATE TABLE "CRISPRSource" (
+	circular BOOLEAN, 
+	output INTEGER, 
+	type TEXT, 
+	id INTEGER NOT NULL, 
+	PRIMARY KEY (id), 
+	FOREIGN KEY(output) REFERENCES "Sequence" (id)
+);
 CREATE TABLE "OligoHybridizationSource" (
+	overhang_crick_3prime INTEGER, 
 	forward_oligo INTEGER NOT NULL, 
 	reverse_oligo INTEGER NOT NULL, 
-	overhang_crick_3prime INTEGER, 
 	output INTEGER, 
 	type TEXT, 
 	id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(forward_oligo) REFERENCES "Primer" (id), 
 	FOREIGN KEY(reverse_oligo) REFERENCES "Primer" (id), 
 	FOREIGN KEY(output) REFERENCES "Sequence" (id)
@@ -396,25 +442,27 @@
 	right_fragment INTEGER NOT NULL, 
 	"AssemblySource_id" INTEGER, 
 	"PCRSource_id" INTEGER, 
 	"LigationSource_id" INTEGER, 
 	"HomologousRecombinationSource_id" INTEGER, 
 	"GibsonAssemblySource_id" INTEGER, 
 	"RestrictionAndLigationSource_id" INTEGER, 
+	"CRISPRSource_id" INTEGER, 
 	left_location_id INTEGER NOT NULL, 
 	right_location_id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(left_fragment) REFERENCES "Sequence" (id), 
 	FOREIGN KEY(right_fragment) REFERENCES "Sequence" (id), 
 	FOREIGN KEY("AssemblySource_id") REFERENCES "AssemblySource" (id), 
 	FOREIGN KEY("PCRSource_id") REFERENCES "PCRSource" (id), 
 	FOREIGN KEY("LigationSource_id") REFERENCES "LigationSource" (id), 
 	FOREIGN KEY("HomologousRecombinationSource_id") REFERENCES "HomologousRecombinationSource" (id), 
 	FOREIGN KEY("GibsonAssemblySource_id") REFERENCES "GibsonAssemblySource" (id), 
 	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id), 
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
 	FOREIGN KEY(left_location_id) REFERENCES "SimpleSequenceLocation" (id), 
 	FOREIGN KEY(right_location_id) REFERENCES "SimpleSequenceLocation" (id)
 );
 CREATE TABLE "Source_input" (
 	"Source_id" INTEGER, 
 	input_id INTEGER, 
 	PRIMARY KEY ("Source_id", input_id), 
@@ -438,14 +486,21 @@
 CREATE TABLE "RepositoryIdSource_input" (
 	"RepositoryIdSource_id" INTEGER, 
 	input_id INTEGER, 
 	PRIMARY KEY ("RepositoryIdSource_id", input_id), 
 	FOREIGN KEY("RepositoryIdSource_id") REFERENCES "RepositoryIdSource" (id), 
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
+CREATE TABLE "AddGeneIdSource_input" (
+	"AddGeneIdSource_id" INTEGER, 
+	input_id INTEGER, 
+	PRIMARY KEY ("AddGeneIdSource_id", input_id), 
+	FOREIGN KEY("AddGeneIdSource_id") REFERENCES "AddGeneIdSource" (id), 
+	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
+);
 CREATE TABLE "GenomeCoordinatesSource_input" (
 	"GenomeCoordinatesSource_id" INTEGER, 
 	input_id INTEGER, 
 	PRIMARY KEY ("GenomeCoordinatesSource_id", input_id), 
 	FOREIGN KEY("GenomeCoordinatesSource_id") REFERENCES "GenomeCoordinatesSource" (id), 
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
@@ -507,14 +562,28 @@
 CREATE TABLE "RestrictionAndLigationSource_input" (
 	"RestrictionAndLigationSource_id" INTEGER, 
 	input_id INTEGER, 
 	PRIMARY KEY ("RestrictionAndLigationSource_id", input_id), 
 	FOREIGN KEY("RestrictionAndLigationSource_id") REFERENCES "RestrictionAndLigationSource" (id), 
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
+CREATE TABLE "CRISPRSource_guides" (
+	"CRISPRSource_id" INTEGER, 
+	guides_id INTEGER NOT NULL, 
+	PRIMARY KEY ("CRISPRSource_id", guides_id), 
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
+	FOREIGN KEY(guides_id) REFERENCES "Primer" (id)
+);
+CREATE TABLE "CRISPRSource_input" (
+	"CRISPRSource_id" INTEGER, 
+	input_id INTEGER, 
+	PRIMARY KEY ("CRISPRSource_id", input_id), 
+	FOREIGN KEY("CRISPRSource_id") REFERENCES "CRISPRSource" (id), 
+	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
+);
 CREATE TABLE "OligoHybridizationSource_input" (
 	"OligoHybridizationSource_id" INTEGER, 
 	input_id INTEGER, 
 	PRIMARY KEY ("OligoHybridizationSource_id", input_id), 
 	FOREIGN KEY("OligoHybridizationSource_id") REFERENCES "OligoHybridizationSource" (id), 
 	FOREIGN KEY(input_id) REFERENCES "Sequence" (id)
 );
```

### Comparing `shareyourcloning_linkml-0.1.2a0/pyproject.toml` & `shareyourcloning_linkml-0.1.3a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Manuel Lera-Ramirez <manuel.lera-ramirez@ucl.ac.uk>"]
 description = "A LinkML data model for ShareYourCloning"
 include = ["README.md", "src/shareyourcloning_linkml/schema", "project"]
 license = "MIT"
 name = "shareyourcloning-linkml"
 readme = "README.md"
-version = "0.1.2a0"
+version = "0.1.3a0"
 
 homepage = "https://github.com/genestorian/ShareYourCloning_LinkML"
 repository = "https://github.com/genestorian/ShareYourCloning_LinkML"
 documentation = "https://genestorian.github.io/ShareYourCloning_LinkML"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/datamodel/_models.py` & `shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/datamodel/_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 from datetime import datetime, date
 from decimal import Decimal
 from enum import Enum
 import re
 import sys
 from typing import Any, List, Literal, Dict, Optional, Union
 from pydantic.version import VERSION as PYDANTIC_VERSION
+from pydantic import conlist
 
 if int(PYDANTIC_VERSION[0]) >= 2:
     from pydantic import BaseModel, ConfigDict, Field, field_validator
 else:
     from pydantic import BaseModel, Field, validator
 
+from pydantic import conlist
+from pydantic import conlist
+from pydantic import conlist
+
 metamodel_version = "None"
 version = "None"
 
 
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
@@ -37,14 +42,21 @@
 
 class SequenceFileFormat(str, Enum):
     fasta = "fasta"
     genbank = "genbank"
     snapgene = "snapgene"
 
 
+class AddGeneSequenceType(str, Enum):
+    # Full sequence of the plasmid submitted by the depositor
+    depositor_full = "depositor-full"
+    # Full sequence of the plasmid performed by Addgene
+    addgene_full = "addgene-full"
+
+
 class NamedThing(ConfiguredBaseModel):
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class Sequence(NamedThing):
     """
     Represents a sequence
@@ -56,23 +68,22 @@
 
 class TextFileSequence(Sequence):
     """
     A sequence (may have features) defined by the content of a text file
     """
 
     sequence_file_format: SequenceFileFormat = Field(..., description="""The format of a sequence file""")
-    file_content: Optional[str] = Field(None)
     overhang_crick_3prime: Optional[int] = Field(
-        None,
+        0,
         description="""Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand""",
     )
     overhang_watson_3prime: Optional[int] = Field(
-        None,
-        description="""The equivalent of `overhang_crick_3prime` but for the watson strand""",
+        0, description="""The equivalent of `overhang_crick_3prime` but for the watson strand"""
     )
+    file_content: Optional[str] = Field(None)
     id: int = Field(..., description="""A unique identifier for a thing""")
     type: Literal["TextFileSequence"] = Field("TextFileSequence", description="""The type of the source""")
 
 
 class Primer(Sequence):
     """
     An oligonucleotide or primer
@@ -97,71 +108,76 @@
 
 
 class SequenceCut(ConfiguredBaseModel):
     """
     Represents a cut in a DNA sequence
     """
 
-    cut_watson: Optional[int] = Field(
-        None,
+    cut_watson: int = Field(
+        ...,
         description="""The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.""",
     )
-    overhang: Optional[int] = Field(
-        None,
+    overhang: int = Field(
+        ...,
         description="""The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.""",
     )
 
 
 class RestrictionSequenceCut(SequenceCut):
     """
     Represents a cut in a DNA sequence that is made by a restriction enzyme
     """
 
     restriction_enzyme: str = Field(...)
-    cut_watson: Optional[int] = Field(
-        None,
+    cut_watson: int = Field(
+        ...,
         description="""The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.""",
     )
-    overhang: Optional[int] = Field(
-        None,
+    overhang: int = Field(
+        ...,
         description="""The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.""",
     )
 
 
 class Source(NamedThing):
     """
     Represents the source of a sequence
     """
 
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["Source"] = Field("Source", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class ManuallyTypedSource(Source):
     """
     Represents the source of a sequence that is manually typed by the user
     """
 
+    overhang_crick_3prime: Optional[int] = Field(
+        0,
+        description="""Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand""",
+    )
+    overhang_watson_3prime: Optional[int] = Field(
+        0, description="""The equivalent of `overhang_crick_3prime` but for the watson strand"""
+    )
     user_input: str = Field(...)
     circular: Optional[bool] = Field(None, description="""Whether the sequence is circular or not""")
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["ManuallyTypedSource"] = Field("ManuallyTypedSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
     @field_validator("user_input")
     def pattern_user_input(cls, v):
         pattern = re.compile(r"^[acgtACGT]+$")
@@ -184,16 +200,15 @@
     file_name: Optional[str] = Field(None, description="""The name of the file""")
     index_in_file: Optional[int] = Field(None, description="""The index of the sequence in the file""")
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["UploadedFileSource"] = Field("UploadedFileSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class RepositoryIdSource(Source):
     """
@@ -203,89 +218,112 @@
     repository_name: RepositoryName = Field(...)
     repository_id: str = Field(..., description="""The id of the sequence in the repository""")
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["RepositoryIdSource"] = Field("RepositoryIdSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
+class AddGeneIdSource(RepositoryIdSource):
+    """
+    Represents the source of a sequence that is identified by an AddGene id
+    """
+
+    sequence_file_url: Optional[str] = Field(None, description="""The URL of a sequence file""")
+    addgene_sequence_type: Optional[AddGeneSequenceType] = Field(None)
+    repository_name: RepositoryName = Field(...)
+    repository_id: str = Field(..., description="""The id of the sequence in the repository""")
+    input: Optional[List[int]] = Field(
+        default_factory=list,
+        description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
+    )
+    output: Optional[int] = Field(
+        None, description="""Identifier of the sequence that is the output of this source."""
+    )
+    type: Literal["AddGeneIdSource"] = Field("AddGeneIdSource", description="""The type of the source""")
+    id: int = Field(..., description="""A unique identifier for a thing""")
+
+    @field_validator("sequence_file_url")
+    def pattern_sequence_file_url(cls, v):
+        pattern = re.compile(
+            r"^https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$"
+        )
+        if isinstance(v, list):
+            for element in v:
+                if not pattern.match(element):
+                    raise ValueError(f"Invalid sequence_file_url format: {element}")
+        elif isinstance(v, str):
+            if not pattern.match(v):
+                raise ValueError(f"Invalid sequence_file_url format: {v}")
+        return v
+
+
 class GenomeCoordinatesSource(Source):
     """
     Represents the source of a sequence that is identified by genome coordinates, requested from NCBI
     """
 
     assembly_accession: Optional[str] = Field(None, description="""The accession of the assembly""")
     sequence_accession: str = Field(..., description="""The accession of the sequence""")
     locus_tag: Optional[str] = Field(None, description="""The locus tag of the sequence""")
     gene_id: Optional[int] = Field(None, description="""The gene id of the sequence""")
     start: int = Field(
-        ...,
-        description="""The starting coordinate (1-based) of the sequence in the sequence accession""",
-    )
-    end: int = Field(
-        ...,
-        description="""The ending coordinate (1-based) of the sequence in the sequence accession""",
-    )
-    strand: int = Field(
-        ...,
-        description="""The strand of the sequence in the sequence accession, should be 1 or -1""",
+        ..., description="""The starting coordinate (1-based) of the sequence in the sequence accession"""
     )
+    end: int = Field(..., description="""The ending coordinate (1-based) of the sequence in the sequence accession""")
+    strand: int = Field(..., description="""The strand of the sequence in the sequence accession, should be 1 or -1""")
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["GenomeCoordinatesSource"] = Field(
         "GenomeCoordinatesSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class SequenceCutSource(Source):
     """
     Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting.
     """
 
     left_edge: Optional[SequenceCut] = Field(None)
     right_edge: Optional[SequenceCut] = Field(None)
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, max_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["SequenceCutSource"] = Field("SequenceCutSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class RestrictionEnzymeDigestionSource(SequenceCutSource):
     """
     Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes.
     """
 
     left_edge: Optional[RestrictionSequenceCut] = Field(None)
     right_edge: Optional[RestrictionSequenceCut] = Field(None)
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, max_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["RestrictionEnzymeDigestionSource"] = Field(
         "RestrictionEnzymeDigestionSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
@@ -319,198 +357,204 @@
 class AssemblySource(Source):
     """
     Represents the source of a sequence that is an assembly of other sequences
     """
 
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["AssemblySource"] = Field("AssemblySource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class PCRSource(AssemblySource):
     """
     Represents the source of a sequence that is generated by PCR
     """
 
     forward_primer: int = Field(..., description="""The forward primer used in the PCR""")
     reverse_primer: int = Field(..., description="""The reverse primer used in the PCR""")
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, max_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["PCRSource"] = Field("PCRSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class LigationSource(AssemblySource):
     """
     Represents the source of a sequence that is generated by ligation with sticky or blunt ends.
     """
 
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["LigationSource"] = Field("LigationSource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class HomologousRecombinationSource(AssemblySource):
     """
     Represents the source of a sequence that is generated by homologous recombination
     """
 
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=2, max_length=2, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["HomologousRecombinationSource"] = Field(
         "HomologousRecombinationSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class GibsonAssemblySource(AssemblySource):
     """
     Represents the source of a sequence that is generated by Gibson assembly
     """
 
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["GibsonAssemblySource"] = Field("GibsonAssemblySource", description="""The type of the source""")
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class RestrictionAndLigationSource(AssemblySource):
     """
     Represents the source of a sequence that is generated by restriction and ligation
     """
 
     restriction_enzymes: List[str] = Field(default_factory=list)
     circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
     assembly: List[AssemblyJoin] = Field(
-        default_factory=list,
-        description="""The joins between the fragments in the assembly""",
+        default_factory=list, description="""The joins between the fragments in the assembly"""
     )
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["RestrictionAndLigationSource"] = Field(
         "RestrictionAndLigationSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
+class CRISPRSource(HomologousRecombinationSource):
+    """
+    Represents the source of a sequence that is generated by CRISPR
+    """
+
+    guides: List[int] = Field(default_factory=list, description="""The guide RNAs used in the CRISPR""")
+    circular: Optional[bool] = Field(None, description="""Whether the assembly is circular or not""")
+    assembly: List[AssemblyJoin] = Field(
+        default_factory=list, description="""The joins between the fragments in the assembly"""
+    )
+    input: Optional[conlist(min_length=2, max_length=2, item_type=int)] = Field(
+        default_factory=list,
+        description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
+    )
+    output: Optional[int] = Field(
+        None, description="""Identifier of the sequence that is the output of this source."""
+    )
+    type: Literal["CRISPRSource"] = Field("CRISPRSource", description="""The type of the source""")
+    id: int = Field(..., description="""A unique identifier for a thing""")
+
+
 class OligoHybridizationSource(Source):
     """
     Represents the source of a sequence that is generated by oligo hybridization
     """
 
-    forward_oligo: int = Field(..., description="""The forward oligo used in the hybridization""")
-    reverse_oligo: int = Field(..., description="""The reverse oligo used in the hybridization""")
     overhang_crick_3prime: Optional[int] = Field(
         None,
-        description="""The length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand.""",
+        description="""Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand""",
     )
+    forward_oligo: int = Field(..., description="""The forward oligo used in the hybridization""")
+    reverse_oligo: int = Field(..., description="""The reverse oligo used in the hybridization""")
     input: Optional[List[int]] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["OligoHybridizationSource"] = Field(
         "OligoHybridizationSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class PolymeraseExtensionSource(Source):
     """
     Represents the source of a sequence that is generated by polymerase extension
     """
 
-    input: Optional[List[int]] = Field(
+    input: Optional[conlist(min_length=1, max_length=1, item_type=int)] = Field(
         default_factory=list,
         description="""The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.""",
     )
     output: Optional[int] = Field(
-        None,
-        description="""Identifier of the sequence that is the output of this source.""",
+        None, description="""Identifier of the sequence that is the output of this source."""
     )
     type: Literal["PolymeraseExtensionSource"] = Field(
         "PolymeraseExtensionSource", description="""The type of the source"""
     )
     id: int = Field(..., description="""A unique identifier for a thing""")
 
 
 class CloningStrategy(ConfiguredBaseModel):
     """
     Represents a cloning strategy
     """
 
     sequences: List[Union[Sequence, TextFileSequence, Primer]] = Field(
-        default_factory=list,
-        description="""The sequences that are used in the cloning strategy""",
+        default_factory=list, description="""The sequences that are used in the cloning strategy"""
     )
     sources: List[
         Union[
             Source,
             ManuallyTypedSource,
             UploadedFileSource,
             RepositoryIdSource,
@@ -520,23 +564,23 @@
             OligoHybridizationSource,
             PolymeraseExtensionSource,
             PCRSource,
             LigationSource,
             HomologousRecombinationSource,
             GibsonAssemblySource,
             RestrictionAndLigationSource,
+            CRISPRSource,
             RestrictionEnzymeDigestionSource,
+            AddGeneIdSource,
         ]
     ] = Field(
-        default_factory=list,
-        description="""The sources of the sequences that are used in the cloning strategy""",
+        default_factory=list, description="""The sources of the sequences that are used in the cloning strategy"""
     )
     primers: Optional[List[int]] = Field(
-        default_factory=list,
-        description="""The primers that are used in the cloning strategy""",
+        default_factory=list, description="""The primers that are used in the cloning strategy"""
     )
     description: Optional[str] = Field(None, description="""A description of the cloning strategy""")
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 NamedThing.model_rebuild()
@@ -545,21 +589,23 @@
 Primer.model_rebuild()
 SequenceCut.model_rebuild()
 RestrictionSequenceCut.model_rebuild()
 Source.model_rebuild()
 ManuallyTypedSource.model_rebuild()
 UploadedFileSource.model_rebuild()
 RepositoryIdSource.model_rebuild()
+AddGeneIdSource.model_rebuild()
 GenomeCoordinatesSource.model_rebuild()
 SequenceCutSource.model_rebuild()
 RestrictionEnzymeDigestionSource.model_rebuild()
 SimpleSequenceLocation.model_rebuild()
 AssemblyJoin.model_rebuild()
 AssemblySource.model_rebuild()
 PCRSource.model_rebuild()
 LigationSource.model_rebuild()
 HomologousRecombinationSource.model_rebuild()
 GibsonAssemblySource.model_rebuild()
 RestrictionAndLigationSource.model_rebuild()
+CRISPRSource.model_rebuild()
 OligoHybridizationSource.model_rebuild()
 PolymeraseExtensionSource.model_rebuild()
 CloningStrategy.model_rebuild()
```

### Comparing `shareyourcloning_linkml-0.1.2a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml` & `shareyourcloning_linkml-0.1.3a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -38,31 +38,26 @@
       - type
 
   TextFileSequence:
     is_a: Sequence
     description: A sequence (may have features) defined by the content of a text file
     slots:
       - sequence_file_format
+      - overhang_crick_3prime
+      - overhang_watson_3prime
     attributes:
       - file_content:
           range: string
-      - overhang_crick_3prime:
-          range: integer
-          description: >-
-            Taken from pydna's `dseq::ovhg`An integer describing
-            the length of the crick strand overhang in the 5'
-            of the molecule, or 3' of the crick strand
-      - overhang_watson_3prime:
-          range: integer
-          description: >-
-            The equivalent of `overhang_crick_3prime` but for the
-            watson strand
     slot_usage:
       sequence_file_format:
         required: true
+      overhang_crick_3prime:
+        ifabsent: int(0)
+      overhang_watson_3prime:
+        ifabsent: int(0)
 
   Primer:
     is_a: Sequence
     description: >-
       An oligonucleotide or primer
     slots:
       - name
@@ -77,20 +72,22 @@
     attributes:
       - cut_watson:
           range: integer
           description: >-
             The position of the cut in the watson strand.
             The cut is made before the base at this position (zero-based),
             so that cut position 1 cuts after the first base.
+          required: true
       - overhang:
           range: integer
           description: >-
             The length of the overhang that is left after the cut. It can be
             negative, same meaning as in pydna's `dseq::ovhg` and biopython's
             `Bio.Restriction.RestrictionType.ovhg`.
+          required: true
 
   RestrictionSequenceCut:
     is_a: SequenceCut
     description: >-
       Represents a cut in a DNA sequence that is made by a restriction enzyme
     slots:
       - restriction_enzyme
@@ -110,23 +107,31 @@
 
   ManuallyTypedSource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is manually typed by the user
     # TODO: See if we can define a type of raw DNA seq with its own constraints,
     # should be the same as in primer
+    slots:
+      - overhang_crick_3prime
+      - overhang_watson_3prime
     attributes:
       - user_input:
           required: true
           range: string
           pattern: ^[acgtACGT]+$
       - circular:
           range: boolean
           description: >-
             Whether the sequence is circular or not
+    slot_usage:
+      overhang_crick_3prime:
+        ifabsent: int(0)
+      overhang_watson_3prime:
+        ifabsent: int(0)
 
   UploadedFileSource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is uploaded as a file
     slots:
       - sequence_file_format
@@ -152,15 +157,25 @@
           range: RepositoryName
           required: true
       - repository_id:
           range: string
           description: >-
             The id of the sequence in the repository
           required: true
-    # TODO: Check which one works
+
+  AddGeneIdSource:
+    is_a: RepositoryIdSource
+    description: >-
+      Represents the source of a sequence that is identified by an AddGene id
+    attributes:
+      # TODO: repository_name constrain to addgene
+      - addgene_sequence_type:
+          range: AddGeneSequenceType
+    slots:
+      - sequence_file_url
 
   GenomeCoordinatesSource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is identified by genome coordinates, requested from NCBI
     attributes:
       - assembly_accession:
@@ -211,15 +226,20 @@
           range: SequenceCut
           required: false # Empty means left end of linear sequence
           inlined: true
       - right_edge:
           range: SequenceCut
           required: false # Empty means right end of linear sequence
           inlined: true
-
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: exact_card
+              exact_cardinality: 1
     # TODO: Validation, at least one of them exists
 
   RestrictionEnzymeDigestionSource:
     is_a: SequenceCutSource
     description: >-
       Represents the source of a sequence that is a subfragment of another sequence,
       generated by sequence cutting using restriction enzymes.
@@ -276,15 +296,14 @@
           range: SimpleSequenceLocation
           description: >-
             Location of the overlap in the right fragment. Might be
             an empty location (start == end) to indicate blunt join.
           required: true
           inlined: true
 
-
   AssemblySource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is an assembly of other sequences
     attributes:
       - circular:
           range: boolean
@@ -309,77 +328,117 @@
           description: >-
             The forward primer used in the PCR
       - reverse_primer:
           range: Primer
           required: true
           description: >-
             The reverse primer used in the PCR
-
-      # TODO:
-      # - Constrain a single input
-      # - Constrain ids of inputs and primers to match those in the assembly
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: exact_card
+              exact_cardinality: 1
+    # TODO:
+    # - Constrain ids of inputs and primers to match those in the assembly
 
   LigationSource:
     is_a: AssemblySource
     description: >-
       Represents the source of a sequence that is generated by ligation with sticky or
       blunt ends.
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: min_card
+              minimum_cardinality: 1
 
   HomologousRecombinationSource:
     is_a: AssemblySource
     description: >-
       Represents the source of a sequence that is generated by homologous recombination
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: exact_card
+              exact_cardinality: 2
     # TODO:
     # Split input? Or just use assembly?
-    # Constrain to two inputs in case
 
   GibsonAssemblySource:
     is_a: AssemblySource
     description: >-
       Represents the source of a sequence that is generated by Gibson assembly
-    # TODO: minimum 1 input
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: min_card
+              minimum_cardinality: 1
 
   RestrictionAndLigationSource:
     is_a: AssemblySource
     description: >-
       Represents the source of a sequence that is generated by restriction and ligation
     slots:
       - restriction_enzymes
     slot_usage:
       restriction_enzymes:
         required: true
+      input:
+        array:
+          dimensions:
+            - alias: min_card
+              minimum_cardinality: 1
+
+  CRISPRSource:
+    is_a: HomologousRecombinationSource
+    description: >-
+      Represents the source of a sequence that is generated by CRISPR
+    attributes:
+      - guides:
+          range: Primer
+          required: true
+          description: >-
+            The guide RNAs used in the CRISPR
+          multivalued: true
 
   OligoHybridizationSource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is generated by oligo hybridization
+    slots:
+      - overhang_crick_3prime
     attributes:
       - forward_oligo:
           range: Primer
           required: true
           description: >-
             The forward oligo used in the hybridization
       - reverse_oligo:
           range: Primer
           required: true
           description: >-
             The reverse oligo used in the hybridization
-      - overhang_crick_3prime:
-          range: integer
-          description: >-
-            The length of the crick strand overhang in the 5'
-            of the molecule, or 3' of the crick strand.
 
   PolymeraseExtensionSource:
     is_a: Source
     description: >-
       Represents the source of a sequence that is generated by polymerase extension
     # TODO:
     # - Constrain to one input
     # - Constrain to having overhangs that can be filled
+    slot_usage:
+      input:
+        array:
+          dimensions:
+            - alias: exact_card
+              exact_cardinality: 1
 
   CloningStrategy:
     description: >-
       Represents a cloning strategy
 
     attributes:
       - sequences:
@@ -451,14 +510,34 @@
     range: string
 
   sequence_file_format:
     range: SequenceFileFormat
     description: >-
       The format of a sequence file
 
+  overhang_crick_3prime:
+    range: integer
+    description: >-
+      Taken from pydna's `dseq::ovhg`An integer describing
+      the length of the crick strand overhang in the 5'
+      of the molecule, or 3' of the crick strand
+
+  overhang_watson_3prime:
+    range: integer
+    description: >-
+      The equivalent of `overhang_crick_3prime` but for the
+      watson strand
+    ifabsent: int(0)
+
+  sequence_file_url:
+    range: string
+    description: >-
+      The URL of a sequence file
+    pattern: ^https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$
+
 enums:
   RepositoryName:
     permissible_values:
       addgene:
         description: >-
           Addgene
       genbank:
@@ -466,7 +545,19 @@
           GenBank
 
   SequenceFileFormat:
     permissible_values:
       fasta:
       genbank:
       snapgene:
+
+  # TODO:
+  # Full list is 'depositor-full', 'depositor-partial', 'addgene-full', 'addgene-partial'
+  # Only the first two should be accepted in the id, but it would be good to list them all
+  AddGeneSequenceType:
+    permissible_values:
+      depositor-full:
+        description: >-
+          Full sequence of the plasmid submitted by the depositor
+      addgene-full:
+        description: >-
+          Full sequence of the plasmid performed by Addgene
```

### Comparing `shareyourcloning_linkml-0.1.2a0/PKG-INFO` & `shareyourcloning_linkml-0.1.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareyourcloning-linkml
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A LinkML data model for ShareYourCloning
 Home-page: https://github.com/genestorian/ShareYourCloning_LinkML
 License: MIT
 Author: Manuel Lera-Ramirez
 Author-email: manuel.lera-ramirez@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

