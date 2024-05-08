# Comparing `tmp/ttrpgaag-4.0.0.tar.gz` & `tmp/ttrpgaag-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttrpgaag-4.0.0.tar", last modified: Mon May  6 18:48:19 2024, max compression
+gzip compressed data, was "ttrpgaag-4.0.1.tar", last modified: Wed May  8 12:01:18 2024, max compression
```

## Comparing `ttrpgaag-4.0.0.tar` & `ttrpgaag-4.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.282866 ttrpgaag-4.0.0/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-4.0.0/LICENSE
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-4.0.0/MANIFEST.in
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1573 2024-05-06 18:48:19.282185 ttrpgaag-4.0.0/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1346 2024-05-06 18:47:45.000000 ttrpgaag-4.0.0/README.md
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.245698 ttrpgaag-4.0.0/RPG/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-05-06 18:30:04.000000 ttrpgaag-4.0.0/RPG/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-4.0.0/RPG/baralho.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.248275 ttrpgaag-4.0.0/RPG/dado/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-4.0.0/RPG/dado/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-4.0.0/RPG/dado/dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-4.0.0/RPG/dado/dados.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.249639 ttrpgaag-4.0.0/RPG/dado/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.0/RPG/dado/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1513 2024-05-06 18:30:04.000000 ttrpgaag-4.0.0/RPG/dado/helpers/converter_notacao_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-4.0.0/RPG/dado/helpers/monta_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2024-05-06 18:30:04.000000 ttrpgaag-4.0.0/RPG/dado/rolar_dado_notacao.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-4.0.0/RPG/iniciativa.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.250491 ttrpgaag-4.0.0/RPG/sistemas/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.251934 ttrpgaag-4.0.0/RPG/sistemas/dnd/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.253369 ttrpgaag-4.0.0/RPG/sistemas/dnd/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/data/mecanicas.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/data/tesouro.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.255437 ttrpgaag-4.0.0/RPG/sistemas/dnd/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      406 2023-10-11 18:00:52.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/helpers/checa_testes.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-01-22 19:11:09.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/rola_tesouro.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5270 2024-02-28 11:57:10.000000 ttrpgaag-4.0.0/RPG/sistemas/dnd/teste.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.258056 ttrpgaag-4.0.0/RPG/sistemas/pf2/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/PC.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6182 2023-11-27 11:50:56.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/calcula_dano.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.264915 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/defesas_monstros.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/proficiency.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/saves.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/skills.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/tipos_ataques.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/data/tipos_defesas.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.267675 ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2023-11-27 11:50:56.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/base_calcula_dano.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      856 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/proficiencias.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-4.0.0/RPG/sistemas/pf2/proficiencia.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.269291 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1316 2024-04-23 18:43:15.000000 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/consulta_critico.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.270767 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-4.0.0/RPG/sistemas/rolemaster/data/criticos.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.272694 ttrpgaag-4.0.0/RPG/tabela_rolavel/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.277137 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 17:28:48.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-05-06 18:30:04.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/ajeita_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      724 2024-04-24 12:42:59.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/ajusta_resultados.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/rolamento_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-05-06 17:41:54.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/rolar_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     4860 2024-05-06 18:46:25.000000 ttrpgaag-4.0.0/RPG/tabela_rolavel/tabela_rolavel.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.281408 ttrpgaag-4.0.0/TTRPGaag.egg-info/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1573 2024-05-06 18:48:19.000000 ttrpgaag-4.0.0/TTRPGaag.egg-info/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-05-06 18:48:19.000000 ttrpgaag-4.0.0/TTRPGaag.egg-info/SOURCES.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-05-06 18:48:19.000000 ttrpgaag-4.0.0/TTRPGaag.egg-info/dependency_links.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-05-06 18:48:19.000000 ttrpgaag-4.0.0/TTRPGaag.egg-info/top_level.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-05-06 18:48:19.283015 ttrpgaag-4.0.0/setup.cfg
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-05-06 18:48:11.000000 ttrpgaag-4.0.0/setup.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:48:19.280696 ttrpgaag-4.0.0/tests/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-4.0.0/tests/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.933378 ttrpgaag-4.0.1/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-4.0.1/LICENSE
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-4.0.1/MANIFEST.in
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1643 2024-05-08 12:01:18.932798 ttrpgaag-4.0.1/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1416 2024-05-08 11:58:33.000000 ttrpgaag-4.0.1/README.md
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.902106 ttrpgaag-4.0.1/RPG/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/baralho.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.904765 ttrpgaag-4.0.1/RPG/dado/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-4.0.1/RPG/dado/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-4.0.1/RPG/dado/dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/dado/dados.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.906172 ttrpgaag-4.0.1/RPG/dado/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/dado/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1512 2024-05-08 11:48:20.000000 ttrpgaag-4.0.1/RPG/dado/helpers/converter_notacao_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/dado/helpers/monta_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/dado/rolar_dado_notacao.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/iniciativa.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.906667 ttrpgaag-4.0.1/RPG/sistemas/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.908083 ttrpgaag-4.0.1/RPG/sistemas/dnd/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.909898 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/mecanicas.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/data/tesouro.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.911645 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      391 2024-05-08 11:50:32.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/helpers/checa_testes.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-05-08 11:49:30.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/rola_tesouro.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5269 2024-05-08 11:49:50.000000 ttrpgaag-4.0.1/RPG/sistemas/dnd/teste.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.914162 ttrpgaag-4.0.1/RPG/sistemas/pf2/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/PC.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6181 2024-05-08 11:52:38.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/calcula_dano.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.918656 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/defesas_monstros.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/proficiency.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/saves.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/skills.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/tipos_ataques.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/data/tipos_defesas.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.921198 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2024-05-08 11:52:54.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      807 2024-05-08 11:53:30.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/proficiencias.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-4.0.1/RPG/sistemas/pf2/proficiencia.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.922516 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1315 2024-05-08 11:53:48.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/consulta_critico.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.923542 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/criticos.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.925725 ttrpgaag-4.0.1/RPG/tabela_rolavel/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.928638 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 17:28:48.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-05-08 11:47:32.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      723 2024-05-08 11:54:25.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajusta_resultados.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/rolamento_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-05-07 18:18:19.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/rolar_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     4858 2024-05-08 11:54:05.000000 ttrpgaag-4.0.1/RPG/tabela_rolavel/tabela_rolavel.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.932083 ttrpgaag-4.0.1/TTRPGaag.egg-info/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1643 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-05-08 12:01:18.000000 ttrpgaag-4.0.1/TTRPGaag.egg-info/top_level.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-05-08 12:01:18.933510 ttrpgaag-4.0.1/setup.cfg
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-05-08 11:58:05.000000 ttrpgaag-4.0.1/setup.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-08 12:01:18.931532 ttrpgaag-4.0.1/tests/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-4.0.1/tests/__init__.py
```

### Comparing `ttrpgaag-4.0.0/LICENSE` & `ttrpgaag-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/PKG-INFO` & `ttrpgaag-4.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 4.0.0
+Version: 4.0.1
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia`
```

### Comparing `ttrpgaag-4.0.0/README.md` & `ttrpgaag-4.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia`
```

### Comparing `ttrpgaag-4.0.0/RPG/baralho.py` & `ttrpgaag-4.0.1/RPG/baralho.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/dado/dado.py` & `ttrpgaag-4.0.1/RPG/dado/dado.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/dado/dados.py` & `ttrpgaag-4.0.1/RPG/dado/dados.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/dado/helpers/converter_notacao_dado.py` & `ttrpgaag-4.0.1/RPG/dado/helpers/converter_notacao_dado.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from RPG.dado.helpers.monta_dado import monta_dado
+from ...dado.helpers.monta_dado import monta_dado
 
 
 def converter_notacao_dado(notacao: str) -> dict:
     """
     Converte a notação de _dados de RPG em um objeto para ser manipulado posteriormente
 
     :param notacao: a notação de dado usada. Exemplo: "3d6+1d4+3"
```

### Comparing `ttrpgaag-4.0.0/RPG/dado/rolar_dado_notacao.py` & `ttrpgaag-4.0.1/RPG/dado/rolar_dado_notacao.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/iniciativa.py` & `ttrpgaag-4.0.1/RPG/iniciativa.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/dnd/data/tesouro.py` & `ttrpgaag-4.0.1/RPG/sistemas/dnd/data/tesouro.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/dnd/rola_tesouro.py` & `ttrpgaag-4.0.1/RPG/sistemas/dnd/rola_tesouro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from RPG import rolar_dado_notacao, TabelaRolavel
+from ... import rolar_dado_notacao, TabelaRolavel
 
 from .data import tesouro, mecanicas
 
 
 @dataclass
 class Tesouro:
     _cr: int = 1
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/dnd/teste.py` & `ttrpgaag-4.0.1/RPG/sistemas/dnd/teste.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RPG.dado import d20
+from ...dado import d20
 from .helpers.checa_testes import checa_teste, checa_ataque
 
 
 class Teste:
 
     def __init__(self, modificador=0, dc=10, vantagem=False, desvantagem=False):
         """
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/PC.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/PC.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/calcula_dano.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/calcula_dano.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .helpers.base_calcula_dano import CalculaDanoBase
-from RPG.dado import Dado
+from ...dado import Dado
 
 
 class CalculaDanoAtaque(CalculaDanoBase):
     tipo = "Ataque"
 
     def __init__(self,
                  nome: str,
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/data/defesas_monstros.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/data/defesas_monstros.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/base_calcula_dano.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RPG.dado import Dado
+from ....dado import Dado
 
 
 class CalculaDanoBase:
     tipo: str = "Base"
 
     def __init__(self,
                  nome: str,
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/helpers/proficiencias.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/helpers/proficiencias.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass, field
-from RPG.sistemas.pf2.data import Data
-from RPG.sistemas.pf2 import calcula_proficiencia, aumenta_proficiencia
+from ...pf2 import calcula_proficiencia, aumenta_proficiencia
 
 
 @dataclass
 class Proficiencia:
     mod_atributo: int = field(repr=False)
     proficiencia: str = field(default=None)
     nivel: int = field(repr=False, default=1)
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/pf2/proficiencia.py` & `ttrpgaag-4.0.1/RPG/sistemas/pf2/proficiencia.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/rolemaster/consulta_critico.py` & `ttrpgaag-4.0.1/RPG/sistemas/rolemaster/consulta_critico.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RPG.tabela_rolavel import TabelaRolavel
+from ...tabela_rolavel import TabelaRolavel
 from .data.criticos import criticos
 
 tabela_criticos = {chave: TabelaRolavel(criticos[chave], 'd100') for chave in criticos.keys()}
 intensidades = 'ABCDE'
 
 
 def consulta_critico(tipo_critico: str, intensidade_critico: str, valor_rolado: int) -> str:
```

### Comparing `ttrpgaag-4.0.0/RPG/sistemas/rolemaster/data/criticos.py` & `ttrpgaag-4.0.1/RPG/sistemas/rolemaster/data/criticos.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/ajeita_tabela.py` & `ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/tabela_rolavel/helpers/ajusta_resultados.py` & `ttrpgaag-4.0.1/RPG/tabela_rolavel/helpers/ajusta_resultados.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RPG.dado.rolar_dado_notacao import rolar_dado_notacao
+from ...dado.rolar_dado_notacao import rolar_dado_notacao
 import re
 
 
 def rola_dados_resultado(rolar_dados: bool, resultado: str) -> str:
     """
     Transforma o texto que contenha notação de _dados em texto com resultado
     :param rolar_dados:
```

### Comparing `ttrpgaag-4.0.0/RPG/tabela_rolavel/rolar_tabela.py` & `ttrpgaag-4.0.1/RPG/tabela_rolavel/rolar_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-4.0.0/RPG/tabela_rolavel/tabela_rolavel.py` & `ttrpgaag-4.0.1/RPG/tabela_rolavel/tabela_rolavel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .rolar_tabela import rolar_tabela
 from .helpers.ajeita_tabela import ajeita_tabela
 from .helpers.busca_index_item_tabela import busca_index_item_tabela
 from .helpers.rolamento_dado import DadoRolado
-from RPG.dado import rolar_dado_notacao
+from ..dado import rolar_dado_notacao
 
 
 class TabelaRolavel:
     def __init__(self, tabela: list = None, dados: str | int = None, rola_subtabela: bool = False):
         """
         Cria um objeto com uma tabela vazia ou já existente (no formato de lista) para ser rolada e métodos para que busquem o
         resultado diretamente nela.
```

### Comparing `ttrpgaag-4.0.0/TTRPGaag.egg-info/PKG-INFO` & `ttrpgaag-4.0.1/TTRPGaag.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 4.0.0
+Version: 4.0.1
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **4.0.1** - Atualização das importações usando caminho relativo
 - **4.0.0** - Métodos de criação de tabelas da `TabelaRolavel` renomeados para o verbo no infinitivo. Inclusão de parâmetro para rolar a subtabela ou não
 - **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia`
```

### Comparing `ttrpgaag-4.0.0/TTRPGaag.egg-info/SOURCES.txt` & `ttrpgaag-4.0.1/TTRPGaag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

