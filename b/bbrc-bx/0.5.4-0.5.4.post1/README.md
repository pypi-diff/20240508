# Comparing `tmp/bbrc-bx-0.5.4.tar.gz` & `tmp/bbrc-bx-0.5.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-bx-0.5.4.tar", last modified: Tue May  7 14:38:15 2024, max compression
+gzip compressed data, was "bbrc-bx-0.5.4.post1.tar", last modified: Wed May  8 09:24:34 2024, max compression
```

## Comparing `bbrc-bx-0.5.4.tar` & `bbrc-bx-0.5.4.post1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35147 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/LICENSE
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/MANIFEST.in
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19803 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19145 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/README.md
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bbrc_bx.egg-info/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19803 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2472 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/SOURCES.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/dependency_links.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/requires.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/top_level.txt
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bin/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bin/bx
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bin/dump
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/ants.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/archiving.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/ashs.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3945 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/asl3d.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/bamos.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4046 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/basil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/braak.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/cache.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/cat12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1301 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/command.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dartel.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/aal2/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/aal2/AAL2.nii
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/braak/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_III_IV.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_I_II.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_V_VI.nii.gz
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/ad/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.tpole.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/readme.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.tpole.label
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/aging/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/logo
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/masks/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/masks/fdg_aging_mask.nii
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dcm.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/donsurf.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13686 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/download.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dtifit.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3147 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/dump.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1538 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/fmriprep.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/freesurfer.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/id.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4614 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/lcmodel.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    76969 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/lists.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2521 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/mrtrix3.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/nifti.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8840 2023-12-19 18:00:09.000000 bbrc-bx-0.5.4/bx/parse.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/pet.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/qsmxt.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/scandates.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/signature.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/spm12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/validation.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3596 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/xcpd.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/xnat.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      221 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/requirements.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/setup.cfg
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:34.072137 bbrc-bx-0.5.4.post1/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35147 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/LICENSE
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/MANIFEST.in
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19821 2024-05-08 09:24:34.072137 bbrc-bx-0.5.4.post1/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19145 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4.post1/README.md
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.962137 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19821 2024-05-08 09:24:33.000000 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2472 2024-05-08 09:24:33.000000 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2024-05-08 09:24:33.000000 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2024-05-08 09:24:33.000000 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2024-05-08 09:24:33.000000 bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/top_level.txt
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.962137 bbrc-bx-0.5.4.post1/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bin/bx
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bin/dump
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.982137 bbrc-bx-0.5.4.post1/bx/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       28 2024-05-08 09:23:38.000000 bbrc-bx-0.5.4.post1/bx/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/ants.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/archiving.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3945 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4.post1/bx/asl3d.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/bamos.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4046 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4.post1/bx/basil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/braak.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/cache.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/cat12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1301 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4.post1/bx/command.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/dartel.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.982137 bbrc-bx-0.5.4.post1/bx/data/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.982137 bbrc-bx-0.5.4.post1/bx/data/aal2/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/aal2/AAL2.nii
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:34.002137 bbrc-bx-0.5.4.post1/bx/data/braak/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/braak/Braak_III_IV.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/braak/Braak_I_II.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/braak/Braak_V_VI.nii.gz
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:33.952137 bbrc-bx-0.5.4.post1/bx/data/dickerson/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:34.042137 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.tpole.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/readme.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.tpole.label
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:34.062137 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/logo
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-08 09:24:34.072137 bbrc-bx-0.5.4.post1/bx/data/masks/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/data/masks/fdg_aging_mask.nii
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/dcm.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/donsurf.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13686 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4.post1/bx/download.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/dtifit.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3147 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4.post1/bx/dump.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1538 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/fmriprep.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/freesurfer.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/id.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4614 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4.post1/bx/lcmodel.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    76969 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/lists.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2521 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/mrtrix3.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/nifti.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8840 2023-12-19 18:00:09.000000 bbrc-bx-0.5.4.post1/bx/parse.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/pet.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/qsmxt.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/scandates.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/signature.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/spm12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/validation.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3596 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4.post1/bx/xcpd.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/bx/xnat.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      221 2024-05-08 09:20:14.000000 bbrc-bx-0.5.4.post1/requirements.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2024-05-08 09:24:34.072137 bbrc-bx-0.5.4.post1/setup.cfg
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4.post1/setup.py
```

### Comparing `bbrc-bx-0.5.4/LICENSE` & `bbrc-bx-0.5.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/PKG-INFO` & `bbrc-bx-0.5.4.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.4
+Version: 0.5.4.post1
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4/bx-v0.5.4.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4.post1/bx-v0.5.4.post1.tar.gz
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bbrc-bx-0.5.4/README.md` & `bbrc-bx-0.5.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bbrc_bx.egg-info/PKG-INFO` & `bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.4
+Version: 0.5.4.post1
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4/bx-v0.5.4.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4.post1/bx-v0.5.4.post1.tar.gz
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bbrc-bx-0.5.4/bbrc_bx.egg-info/SOURCES.txt` & `bbrc-bx-0.5.4.post1/bbrc_bx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bin/bx` & `bbrc-bx-0.5.4.post1/bin/bx`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bin/dump` & `bbrc-bx-0.5.4.post1/bin/dump`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/ants.py` & `bbrc-bx-0.5.4.post1/bx/ants.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/archiving.py` & `bbrc-bx-0.5.4.post1/bx/archiving.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/ashs.py` & `bbrc-bx-0.5.4.post1/bx/ashs.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/asl3d.py` & `bbrc-bx-0.5.4.post1/bx/asl3d.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/bamos.py` & `bbrc-bx-0.5.4.post1/bx/bamos.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/basil.py` & `bbrc-bx-0.5.4.post1/bx/basil.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/braak.py` & `bbrc-bx-0.5.4.post1/bx/braak.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/cache.py` & `bbrc-bx-0.5.4.post1/bx/cache.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/cat12.py` & `bbrc-bx-0.5.4.post1/bx/cat12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/command.py` & `bbrc-bx-0.5.4.post1/bx/command.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/dartel.py` & `bbrc-bx-0.5.4.post1/bx/dartel.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/aal2/AAL2.nii` & `bbrc-bx-0.5.4.post1/bx/data/aal2/AAL2.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/braak/Braak_III_IV.nii.gz` & `bbrc-bx-0.5.4.post1/bx/data/braak/Braak_III_IV.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/braak/Braak_I_II.nii.gz` & `bbrc-bx-0.5.4.post1/bx/data/braak/Braak_I_II.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/braak/Braak_V_VI.nii.gz` & `bbrc-bx-0.5.4.post1/bx/data/braak/Braak_V_VI.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.annot` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ag.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ifs.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.itg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.mtl.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.precun.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.sfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.smg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.spl.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.tpole.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/lh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.annot` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ag.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ifs.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.itg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.mtl.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.precun.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.sfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.smg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.spl.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.tpole.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/ad/rh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ag.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.calcarine.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cfusi.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cinsula.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cmfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cuneus.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ifg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.loccip.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.msfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.precent.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.smg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ag.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.calcarine.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cfusi.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cinsula.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cmfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cuneus.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ifg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.loccip.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.msfg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.precent.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.smg.label` & `bbrc-bx-0.5.4.post1/bx/data/dickerson/aging/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/data/masks/fdg_aging_mask.nii` & `bbrc-bx-0.5.4.post1/bx/data/masks/fdg_aging_mask.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/dcm.py` & `bbrc-bx-0.5.4.post1/bx/dcm.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/donsurf.py` & `bbrc-bx-0.5.4.post1/bx/donsurf.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/download.py` & `bbrc-bx-0.5.4.post1/bx/download.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/dtifit.py` & `bbrc-bx-0.5.4.post1/bx/dtifit.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/dump.py` & `bbrc-bx-0.5.4.post1/bx/dump.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/fmriprep.py` & `bbrc-bx-0.5.4.post1/bx/fmriprep.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/freesurfer.py` & `bbrc-bx-0.5.4.post1/bx/freesurfer.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/id.py` & `bbrc-bx-0.5.4.post1/bx/id.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/lcmodel.py` & `bbrc-bx-0.5.4.post1/bx/lcmodel.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/lists.py` & `bbrc-bx-0.5.4.post1/bx/lists.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/mrtrix3.py` & `bbrc-bx-0.5.4.post1/bx/mrtrix3.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/nifti.py` & `bbrc-bx-0.5.4.post1/bx/nifti.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/parse.py` & `bbrc-bx-0.5.4.post1/bx/parse.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/pet.py` & `bbrc-bx-0.5.4.post1/bx/pet.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/qsmxt.py` & `bbrc-bx-0.5.4.post1/bx/qsmxt.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/scandates.py` & `bbrc-bx-0.5.4.post1/bx/scandates.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/signature.py` & `bbrc-bx-0.5.4.post1/bx/signature.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/spm12.py` & `bbrc-bx-0.5.4.post1/bx/spm12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/validation.py` & `bbrc-bx-0.5.4.post1/bx/validation.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/xcpd.py` & `bbrc-bx-0.5.4.post1/bx/xcpd.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/bx/xnat.py` & `bbrc-bx-0.5.4.post1/bx/xnat.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.4/setup.py` & `bbrc-bx-0.5.4.post1/setup.py`

 * *Files identical despite different names*

