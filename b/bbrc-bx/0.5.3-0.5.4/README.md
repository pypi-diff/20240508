# Comparing `tmp/bbrc-bx-0.5.3.tar.gz` & `tmp/bbrc-bx-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-bx-0.5.3.tar", last modified: Tue Dec 19 18:01:06 2023, max compression
+gzip compressed data, was "bbrc-bx-0.5.4.tar", last modified: Tue May  7 14:38:15 2024, max compression
```

## Comparing `bbrc-bx-0.5.3.tar` & `bbrc-bx-0.5.4.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:06.164957 bbrc-bx-0.5.3/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35147 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/LICENSE
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/MANIFEST.in
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20392 2023-12-19 18:01:06.154957 bbrc-bx-0.5.3/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19734 2023-12-19 18:00:09.000000 bbrc-bx-0.5.3/README.md
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.904957 bbrc-bx-0.5.3/bbrc_bx.egg-info/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20392 2023-12-19 18:01:05.000000 bbrc-bx-0.5.3/bbrc_bx.egg-info/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2460 2023-12-19 18:01:05.000000 bbrc-bx-0.5.3/bbrc_bx.egg-info/SOURCES.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-12-19 18:01:05.000000 bbrc-bx-0.5.3/bbrc_bx.egg-info/dependency_links.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-12-19 18:01:05.000000 bbrc-bx-0.5.3/bbrc_bx.egg-info/requires.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2023-12-19 18:01:05.000000 bbrc-bx-0.5.3/bbrc_bx.egg-info/top_level.txt
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.904957 bbrc-bx-0.5.3/bin/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bin/bx
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bin/dump
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.954957 bbrc-bx-0.5.3/bx/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2023-12-19 18:00:09.000000 bbrc-bx-0.5.3/bx/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/ants.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/archiving.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/ashs.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/bamos.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3957 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/basil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/braak.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/cache.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/cat12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1301 2023-12-19 17:43:58.000000 bbrc-bx-0.5.3/bx/command.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/dartel.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.964957 bbrc-bx-0.5.3/bx/data/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.964957 bbrc-bx-0.5.3/bx/data/aal2/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/aal2/AAL2.nii
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.974957 bbrc-bx-0.5.3/bx/data/braak/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/braak/Braak_III_IV.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/braak/Braak_I_II.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/braak/Braak_V_VI.nii.gz
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:05.894957 bbrc-bx-0.5.3/bx/data/dickerson/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:06.074957 bbrc-bx-0.5.3/bx/data/dickerson/ad/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.tpole.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/readme.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.tpole.label
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:06.144957 bbrc-bx-0.5.3/bx/data/dickerson/aging/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/logo
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-12-19 18:01:06.144957 bbrc-bx-0.5.3/bx/data/masks/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/data/masks/fdg_aging_mask.nii
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/dcm.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/donsurf.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13464 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/download.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/dtifit.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3147 2023-12-19 17:43:58.000000 bbrc-bx-0.5.3/bx/dump.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1538 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/fmriprep.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/freesurfer.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/id.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4614 2023-12-19 17:43:58.000000 bbrc-bx-0.5.3/bx/lcmodel.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    76969 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/lists.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2521 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/mrtrix3.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/nifti.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8840 2023-12-19 18:00:09.000000 bbrc-bx-0.5.3/bx/parse.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/pet.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/qsmxt.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/scandates.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/signature.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/spm12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/validation.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3517 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/xcpd.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/bx/xnat.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/requirements.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2023-12-19 18:01:06.164957 bbrc-bx-0.5.3/setup.cfg
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-12-18 14:40:19.000000 bbrc-bx-0.5.3/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35147 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/LICENSE
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/MANIFEST.in
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19803 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19145 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/README.md
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bbrc_bx.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19803 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2472 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2024-05-07 14:38:15.000000 bbrc-bx-0.5.4/bbrc_bx.egg-info/top_level.txt
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bin/bx
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bin/dump
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/ants.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/archiving.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3945 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/asl3d.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/bamos.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4046 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/basil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/braak.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/cache.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/cat12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1301 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/command.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dartel.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/aal2/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/aal2/AAL2.nii
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/braak/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_III_IV.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_I_II.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/braak/Braak_V_VI.nii.gz
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/ad/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.tpole.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/readme.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.tpole.label
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/dickerson/aging/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/logo
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/bx/data/masks/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/data/masks/fdg_aging_mask.nii
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dcm.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/donsurf.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13686 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/download.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/dtifit.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3147 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/dump.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1538 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/fmriprep.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/freesurfer.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/id.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4614 2023-12-19 17:43:58.000000 bbrc-bx-0.5.4/bx/lcmodel.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    76969 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/lists.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2521 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/mrtrix3.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/nifti.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8840 2023-12-19 18:00:09.000000 bbrc-bx-0.5.4/bx/parse.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/pet.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/qsmxt.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/scandates.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/signature.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/spm12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/validation.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3596 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/bx/xcpd.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/bx/xnat.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      221 2024-05-07 14:36:56.000000 bbrc-bx-0.5.4/requirements.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2024-05-07 14:38:15.656427 bbrc-bx-0.5.4/setup.cfg
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-12-18 14:40:19.000000 bbrc-bx-0.5.4/setup.py
```

### Comparing `bbrc-bx-0.5.3/LICENSE` & `bbrc-bx-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/PKG-INFO` & `bbrc-bx-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.3
+Version: 0.5.4
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.3/bx-v0.5.3.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4/bx-v0.5.4.tar.gz
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -78,14 +78,33 @@
      `snapshot`:	download a snapshot from the `ASHS` pipeline
      `report`:		download the validation report issued by `ASHSValidator`
      `tests`:		creates an Excel table with all automatic tests outcomes from `ASHSValidator`
 
     Usage:
      bx ashs <subcommand> <resource_id>
 
+### **`ASL3D`**:
+
+Cerebral perfusion quantification of reconstructed 3D Arterial Spin Labeling MRI.
+
+    Available subcommands:
+     `perfusion`:       creates an Excel table with global perfusion values.
+     `aal`:             creates an Excel table with regional perfusion values (in AAL atlas).
+     `maps`:            download the calibrated perfusion maps
+     `files`:           download all 3D-ASL QUANTIFICATION outputs (perfusion maps, files, everything...)
+     `snapshot`:        download a snapshot from the 3D-ASL QUANTIFICATION pipeline
+     `report`:          download the validation report issued by bbrc-validator
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx asl3d <subcommand> <resource_id>
+
+    References:
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
+
 ### **`BAMOS`**:
 
 BAMOS (Bayesian MOdel Selection for white matter lesion segmentation)
 
     Available subcommands:
      `files`:		download all `BAMOS` outputs
      `volumes`:		create an Excel table with global lesion volumes
@@ -119,14 +138,15 @@
      `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx basil <subcommand> <resource_id>
 
     References:
     - Chappell MA., IEEE Transactions on Signal Processing, 2009.
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
 
 ### **`BRAAK`**:
 
 Extract morphometric/metabolic measurements based on Braak staging.
 
     Morphometric values are based on regional volumes or cortical thickness
     as estimated individually by FreeSurfer with respect to each specific stage
@@ -223,14 +243,29 @@
     `snapshot`:		download a snapshot with FA map, RGB tensor and TOPUP distortion correction map
     `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
 
     Usage:
      bx dtifit <subcommand> <resource_id>
 
+### **`FMRIPREP`**:
+
+fMRIPrep - Preprocessing of fMRI data.
+
+    Available subcommands:
+     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
+     `report`:          download the validation report issued by `FMRIPrepValidator`
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx fmriprep <subcommand> <resource_id>
+
+    References:
+    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
+
 ### **`FREESURFER6`**:
 
 FreeSurfer v6.0.0
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
@@ -298,31 +333,29 @@
 Return generic information like subject/session labels, parent project.
 
     Usage:
      bx id <resource_id>
 	 
 ### **`LCMODEL`**:
 
-LCModel - this pipeline uses the LCModel package for automatic quantitation of in vivo proton MR spectra.
+LCModel - Quantification and tissue-correction of MR Spectroscopy images.
 
     Available subcommands:
-     `stats`:           creates an Excel table with the metabolite concentrations and other miscellaneous parameters (e.g. FWHM, SNR).
-     `correction`:      creates an Excel table with the values of the tissue correction parameters to statistically adjust
-                        the metabolite concentration results.
+     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
+     `correction`:      creates an Excel table with tissue correction parameters
      `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download a snapshot from the mask files extracted from T1_ALFA1 for each location (i.e. Angular gyrus, 
-                        Hippocampus and Cuneus)
-     `report`:          download the validation report issued by bbrc-validator
+     `snapshot`:        download snapshots from the LCMODEL pipeline
+     `report`:          download the validation report issued by `LCModelValidator`
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx lcmodel <subcommand> <resource_id>
 
     References:
-    Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Provencher SW., Magnetic Resonance in Medicine, 1993.
 
 ### **`LISTS`**:
 
 Manage experiment lists curated by BarcelonaBeta.
 
     Available subcommands:
      `show`:		display all existing lists (usage: bx lists show)
@@ -453,29 +486,14 @@
     thickness values as they do not have any "grayvol" version.
 
     References:
     - Jack et al., Alzheimers Dement. 2017
     - Dickerson et al., Neurology, 2011
     - Bakkour et al., NeuroImage, 2013
 
-### **`SPM12`**:
-
-SPM12 - Gray/white matter segmentation
-
-    Available subcommands:
-     `files`:		download all `SPM12` outputs (segmentation maps, warp fields, everything...)
-     `volumes`:		creates an Excel table with GM/WM/CSF volumes
-     `snapshot`:	download a snapshot from the segmentation results
-     `report`:		download the validation report issued by `SPM12Validator`
-     `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
-     `rc`:			downloads rc* files (DARTEL imports)
-
-    Usage:
-     bx spm12 <subcommand> <resource_id>
-
 ### **`XCPD`**:
 
 XCP-D - Resting State fMRI postprocessing and functional connectivity.
 
     Available subcommands:
      `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
      `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
@@ -485,47 +503,15 @@
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx xcpd <subcommand> <resource_id>
 
     References:
     - Ciric R, et al., Nat Protoc 13 (2018).
-
-### **`FMRIPREP`**:
-
-fMRIPrep - Preprocessing of fMRI data.
-
-    Available subcommands:
-     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
-     `report`:          download the validation report issued by `FMRIPrepValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx fmriprep <subcommand> <resource_id>
-
-    References:
-    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
-
-### **`LCMODEL`**:
-
-LCModel - Quantification and tissue-correction of MR Spectroscopy images.
-
-    Available subcommands:
-     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
-     `correction`:      creates an Excel table with tissue correction parameters
-     `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download snapshots from the LCMODEL pipeline
-     `report`:          download the validation report issued by `LCModelValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx lcmodel <subcommand> <resource_id>
-
-    References:
-    - Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Mehta K., Salo T. et al., bioRxiv (2023). DOI: 10.1101/2023.11.20.567926
 
 ## Dependencies
 
 Requires [`bbrc-pyxnat>=1.6.1`](https://github.com/pyxnat/pyxnat/tree/bbrc) and
 the librairies listed in `requirements.txt`.
```

### Comparing `bbrc-bx-0.5.3/README.md` & `bbrc-bx-0.5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,33 @@
      `snapshot`:	download a snapshot from the `ASHS` pipeline
      `report`:		download the validation report issued by `ASHSValidator`
      `tests`:		creates an Excel table with all automatic tests outcomes from `ASHSValidator`
 
     Usage:
      bx ashs <subcommand> <resource_id>
 
+### **`ASL3D`**:
+
+Cerebral perfusion quantification of reconstructed 3D Arterial Spin Labeling MRI.
+
+    Available subcommands:
+     `perfusion`:       creates an Excel table with global perfusion values.
+     `aal`:             creates an Excel table with regional perfusion values (in AAL atlas).
+     `maps`:            download the calibrated perfusion maps
+     `files`:           download all 3D-ASL QUANTIFICATION outputs (perfusion maps, files, everything...)
+     `snapshot`:        download a snapshot from the 3D-ASL QUANTIFICATION pipeline
+     `report`:          download the validation report issued by bbrc-validator
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx asl3d <subcommand> <resource_id>
+
+    References:
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
+
 ### **`BAMOS`**:
 
 BAMOS (Bayesian MOdel Selection for white matter lesion segmentation)
 
     Available subcommands:
      `files`:		download all `BAMOS` outputs
      `volumes`:		create an Excel table with global lesion volumes
@@ -100,14 +119,15 @@
      `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx basil <subcommand> <resource_id>
 
     References:
     - Chappell MA., IEEE Transactions on Signal Processing, 2009.
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
 
 ### **`BRAAK`**:
 
 Extract morphometric/metabolic measurements based on Braak staging.
 
     Morphometric values are based on regional volumes or cortical thickness
     as estimated individually by FreeSurfer with respect to each specific stage
@@ -204,14 +224,29 @@
     `snapshot`:		download a snapshot with FA map, RGB tensor and TOPUP distortion correction map
     `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
 
     Usage:
      bx dtifit <subcommand> <resource_id>
 
+### **`FMRIPREP`**:
+
+fMRIPrep - Preprocessing of fMRI data.
+
+    Available subcommands:
+     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
+     `report`:          download the validation report issued by `FMRIPrepValidator`
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx fmriprep <subcommand> <resource_id>
+
+    References:
+    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
+
 ### **`FREESURFER6`**:
 
 FreeSurfer v6.0.0
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
@@ -279,31 +314,29 @@
 Return generic information like subject/session labels, parent project.
 
     Usage:
      bx id <resource_id>
 	 
 ### **`LCMODEL`**:
 
-LCModel - this pipeline uses the LCModel package for automatic quantitation of in vivo proton MR spectra.
+LCModel - Quantification and tissue-correction of MR Spectroscopy images.
 
     Available subcommands:
-     `stats`:           creates an Excel table with the metabolite concentrations and other miscellaneous parameters (e.g. FWHM, SNR).
-     `correction`:      creates an Excel table with the values of the tissue correction parameters to statistically adjust
-                        the metabolite concentration results.
+     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
+     `correction`:      creates an Excel table with tissue correction parameters
      `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download a snapshot from the mask files extracted from T1_ALFA1 for each location (i.e. Angular gyrus, 
-                        Hippocampus and Cuneus)
-     `report`:          download the validation report issued by bbrc-validator
+     `snapshot`:        download snapshots from the LCMODEL pipeline
+     `report`:          download the validation report issued by `LCModelValidator`
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx lcmodel <subcommand> <resource_id>
 
     References:
-    Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Provencher SW., Magnetic Resonance in Medicine, 1993.
 
 ### **`LISTS`**:
 
 Manage experiment lists curated by BarcelonaBeta.
 
     Available subcommands:
      `show`:		display all existing lists (usage: bx lists show)
@@ -434,29 +467,14 @@
     thickness values as they do not have any "grayvol" version.
 
     References:
     - Jack et al., Alzheimers Dement. 2017
     - Dickerson et al., Neurology, 2011
     - Bakkour et al., NeuroImage, 2013
 
-### **`SPM12`**:
-
-SPM12 - Gray/white matter segmentation
-
-    Available subcommands:
-     `files`:		download all `SPM12` outputs (segmentation maps, warp fields, everything...)
-     `volumes`:		creates an Excel table with GM/WM/CSF volumes
-     `snapshot`:	download a snapshot from the segmentation results
-     `report`:		download the validation report issued by `SPM12Validator`
-     `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
-     `rc`:			downloads rc* files (DARTEL imports)
-
-    Usage:
-     bx spm12 <subcommand> <resource_id>
-
 ### **`XCPD`**:
 
 XCP-D - Resting State fMRI postprocessing and functional connectivity.
 
     Available subcommands:
      `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
      `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
@@ -466,47 +484,15 @@
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx xcpd <subcommand> <resource_id>
 
     References:
     - Ciric R, et al., Nat Protoc 13 (2018).
-
-### **`FMRIPREP`**:
-
-fMRIPrep - Preprocessing of fMRI data.
-
-    Available subcommands:
-     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
-     `report`:          download the validation report issued by `FMRIPrepValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx fmriprep <subcommand> <resource_id>
-
-    References:
-    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
-
-### **`LCMODEL`**:
-
-LCModel - Quantification and tissue-correction of MR Spectroscopy images.
-
-    Available subcommands:
-     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
-     `correction`:      creates an Excel table with tissue correction parameters
-     `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download snapshots from the LCMODEL pipeline
-     `report`:          download the validation report issued by `LCModelValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx lcmodel <subcommand> <resource_id>
-
-    References:
-    - Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Mehta K., Salo T. et al., bioRxiv (2023). DOI: 10.1101/2023.11.20.567926
 
 ## Dependencies
 
 Requires [`bbrc-pyxnat>=1.6.1`](https://github.com/pyxnat/pyxnat/tree/bbrc) and
 the librairies listed in `requirements.txt`.
```

### Comparing `bbrc-bx-0.5.3/bbrc_bx.egg-info/PKG-INFO` & `bbrc-bx-0.5.4/bbrc_bx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.3
+Version: 0.5.4
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.3/bx-v0.5.3.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.4/bx-v0.5.4.tar.gz
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -78,14 +78,33 @@
      `snapshot`:	download a snapshot from the `ASHS` pipeline
      `report`:		download the validation report issued by `ASHSValidator`
      `tests`:		creates an Excel table with all automatic tests outcomes from `ASHSValidator`
 
     Usage:
      bx ashs <subcommand> <resource_id>
 
+### **`ASL3D`**:
+
+Cerebral perfusion quantification of reconstructed 3D Arterial Spin Labeling MRI.
+
+    Available subcommands:
+     `perfusion`:       creates an Excel table with global perfusion values.
+     `aal`:             creates an Excel table with regional perfusion values (in AAL atlas).
+     `maps`:            download the calibrated perfusion maps
+     `files`:           download all 3D-ASL QUANTIFICATION outputs (perfusion maps, files, everything...)
+     `snapshot`:        download a snapshot from the 3D-ASL QUANTIFICATION pipeline
+     `report`:          download the validation report issued by bbrc-validator
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx asl3d <subcommand> <resource_id>
+
+    References:
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
+
 ### **`BAMOS`**:
 
 BAMOS (Bayesian MOdel Selection for white matter lesion segmentation)
 
     Available subcommands:
      `files`:		download all `BAMOS` outputs
      `volumes`:		create an Excel table with global lesion volumes
@@ -119,14 +138,15 @@
      `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx basil <subcommand> <resource_id>
 
     References:
     - Chappell MA., IEEE Transactions on Signal Processing, 2009.
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
 
 ### **`BRAAK`**:
 
 Extract morphometric/metabolic measurements based on Braak staging.
 
     Morphometric values are based on regional volumes or cortical thickness
     as estimated individually by FreeSurfer with respect to each specific stage
@@ -223,14 +243,29 @@
     `snapshot`:		download a snapshot with FA map, RGB tensor and TOPUP distortion correction map
     `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
 
     Usage:
      bx dtifit <subcommand> <resource_id>
 
+### **`FMRIPREP`**:
+
+fMRIPrep - Preprocessing of fMRI data.
+
+    Available subcommands:
+     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
+     `report`:          download the validation report issued by `FMRIPrepValidator`
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx fmriprep <subcommand> <resource_id>
+
+    References:
+    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
+
 ### **`FREESURFER6`**:
 
 FreeSurfer v6.0.0
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
@@ -298,31 +333,29 @@
 Return generic information like subject/session labels, parent project.
 
     Usage:
      bx id <resource_id>
 	 
 ### **`LCMODEL`**:
 
-LCModel - this pipeline uses the LCModel package for automatic quantitation of in vivo proton MR spectra.
+LCModel - Quantification and tissue-correction of MR Spectroscopy images.
 
     Available subcommands:
-     `stats`:           creates an Excel table with the metabolite concentrations and other miscellaneous parameters (e.g. FWHM, SNR).
-     `correction`:      creates an Excel table with the values of the tissue correction parameters to statistically adjust
-                        the metabolite concentration results.
+     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
+     `correction`:      creates an Excel table with tissue correction parameters
      `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download a snapshot from the mask files extracted from T1_ALFA1 for each location (i.e. Angular gyrus, 
-                        Hippocampus and Cuneus)
-     `report`:          download the validation report issued by bbrc-validator
+     `snapshot`:        download snapshots from the LCMODEL pipeline
+     `report`:          download the validation report issued by `LCModelValidator`
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx lcmodel <subcommand> <resource_id>
 
     References:
-    Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Provencher SW., Magnetic Resonance in Medicine, 1993.
 
 ### **`LISTS`**:
 
 Manage experiment lists curated by BarcelonaBeta.
 
     Available subcommands:
      `show`:		display all existing lists (usage: bx lists show)
@@ -453,29 +486,14 @@
     thickness values as they do not have any "grayvol" version.
 
     References:
     - Jack et al., Alzheimers Dement. 2017
     - Dickerson et al., Neurology, 2011
     - Bakkour et al., NeuroImage, 2013
 
-### **`SPM12`**:
-
-SPM12 - Gray/white matter segmentation
-
-    Available subcommands:
-     `files`:		download all `SPM12` outputs (segmentation maps, warp fields, everything...)
-     `volumes`:		creates an Excel table with GM/WM/CSF volumes
-     `snapshot`:	download a snapshot from the segmentation results
-     `report`:		download the validation report issued by `SPM12Validator`
-     `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
-     `rc`:			downloads rc* files (DARTEL imports)
-
-    Usage:
-     bx spm12 <subcommand> <resource_id>
-
 ### **`XCPD`**:
 
 XCP-D - Resting State fMRI postprocessing and functional connectivity.
 
     Available subcommands:
      `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
      `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
@@ -485,47 +503,15 @@
      `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx xcpd <subcommand> <resource_id>
 
     References:
     - Ciric R, et al., Nat Protoc 13 (2018).
-
-### **`FMRIPREP`**:
-
-fMRIPrep - Preprocessing of fMRI data.
-
-    Available subcommands:
-     `files`:           download all `FMRIPREP` outputs (preprocessed BOLD, confounds, segmentations, everything...)
-     `report`:          download the validation report issued by `FMRIPrepValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx fmriprep <subcommand> <resource_id>
-
-    References:
-    - Esteban O, et al., Nat Methods 16, 111–116 (2019).
-
-### **`LCMODEL`**:
-
-LCModel - Quantification and tissue-correction of MR Spectroscopy images.
-
-    Available subcommands:
-     `stats`:           creates an Excel table with metabolite concentrations and global signal quality stats
-     `correction`:      creates an Excel table with tissue correction parameters
-     `files`:           download all LCModel outputs (stats, tissue correction, masks, everything...)
-     `snapshot`:        download snapshots from the LCMODEL pipeline
-     `report`:          download the validation report issued by `LCModelValidator`
-     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
-
-    Usage:
-     bx lcmodel <subcommand> <resource_id>
-
-    References:
-    - Provencher SW., Magnetic Resonance in Medicine, 1993.
+    - Mehta K., Salo T. et al., bioRxiv (2023). DOI: 10.1101/2023.11.20.567926
 
 ## Dependencies
 
 Requires [`bbrc-pyxnat>=1.6.1`](https://github.com/pyxnat/pyxnat/tree/bbrc) and
 the librairies listed in `requirements.txt`.
```

### Comparing `bbrc-bx-0.5.3/bbrc_bx.egg-info/SOURCES.txt` & `bbrc-bx-0.5.4/bbrc_bx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 bbrc_bx.egg-info/top_level.txt
 bin/bx
 bin/dump
 bx/__init__.py
 bx/ants.py
 bx/archiving.py
 bx/ashs.py
+bx/asl3d.py
 bx/bamos.py
 bx/basil.py
 bx/braak.py
 bx/cache.py
 bx/cat12.py
 bx/command.py
 bx/dartel.py
```

### Comparing `bbrc-bx-0.5.3/bin/bx` & `bbrc-bx-0.5.4/bin/bx`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bin/dump` & `bbrc-bx-0.5.4/bin/dump`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/ants.py` & `bbrc-bx-0.5.4/bx/ants.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/archiving.py` & `bbrc-bx-0.5.4/bx/archiving.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/ashs.py` & `bbrc-bx-0.5.4/bx/ashs.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/bamos.py` & `bbrc-bx-0.5.4/bx/bamos.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/basil.py` & `bbrc-bx-0.5.4/bx/basil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from bx.command import Command
 from bx import download as dl
 import os
 import logging as log
 
 
 class BASILCommand(Command):
-    """BASIL - Bayesian Inference for Arterial Spin Labeling MRI. Arterial Spin
-    Labeling (ASL) MRI is a non-invasive method for the quantification of perfusion.
+    """BASIL - Bayesian Inference for Arterial Spin Labeling MRI.
+    Arterial Spin Labeling (ASL) MRI is a non-invasive method for the quantification
+    of perfusion.
 
     Available subcommands:
      perfusion:\t\tcreates an Excel table with global perfusion and arrival-time values.
      stats:\t\tcreates an Excel table with regional perfusion values (in Harvard-Oxford atlas).
      aal:\t\tcreates an Excel table with regional perfusion values (in AAL atlas).
      maps:\t\tdownload the calibrated perfusion maps
      files:\t\tdownload all BASIL-ASL outputs (perfusion maps, files, everything...)
@@ -19,21 +20,22 @@
      tests:\t\tcreate an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx basil <subcommand> <resource_id>
 
     References:
     - Chappell MA., IEEE Transactions on Signal Processing, 2009.
+    - Chappell MA. et al., Imaging Neuroscience, 2023. DOI: 10.1162/imag_a_00041
     """
     nargs = 2
     resource_name = 'BASIL'
     subcommands = ['perfusion', 'aal', 'stats', 'maps', 'files', 'report',
                    'snapshot', 'tests']
     validator = 'BASILValidator'
-    url = 'https://gitlab.com/bbrc/xnat/xnat-pipelines/-/tree/master/basil'
+    url = 'https://gitlab.com/bbrc/xnat/xnat-pipelines/-/tree/master/asl#basil'
 
     def __init__(self, *args, **kwargs):
         super(BASILCommand, self).__init__(*args, **kwargs)
 
     def parse(self):
         subcommand = self.args[0]
         id = self.args[1]
```

### Comparing `bbrc-bx-0.5.3/bx/braak.py` & `bbrc-bx-0.5.4/bx/braak.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/cache.py` & `bbrc-bx-0.5.4/bx/cache.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/cat12.py` & `bbrc-bx-0.5.4/bx/cat12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/command.py` & `bbrc-bx-0.5.4/bx/command.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/dartel.py` & `bbrc-bx-0.5.4/bx/dartel.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/aal2/AAL2.nii` & `bbrc-bx-0.5.4/bx/data/aal2/AAL2.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/braak/Braak_III_IV.nii.gz` & `bbrc-bx-0.5.4/bx/data/braak/Braak_III_IV.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/braak/Braak_I_II.nii.gz` & `bbrc-bx-0.5.4/bx/data/braak/Braak_I_II.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/braak/Braak_V_VI.nii.gz` & `bbrc-bx-0.5.4/bx/data/braak/Braak_V_VI.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.adsig.annot` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.adsig.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.ag.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.ifs.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.itg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.mtl.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.precun.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.sfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.smg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.spl.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/lh.tpole.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/lh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.adsig.annot` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.adsig.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.ag.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.ifs.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.itg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.mtl.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.precun.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.sfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.smg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.spl.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/ad/rh.tpole.label` & `bbrc-bx-0.5.4/bx/data/dickerson/ad/rh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.ag.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.calcarine.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cfusi.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cinsula.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cmfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.cuneus.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.ifg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.loccip.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.msfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.precent.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/lh.smg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.ag.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.calcarine.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cfusi.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cinsula.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cmfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.cuneus.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.ifg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.loccip.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.msfg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.precent.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/dickerson/aging/rh.smg.label` & `bbrc-bx-0.5.4/bx/data/dickerson/aging/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/data/masks/fdg_aging_mask.nii` & `bbrc-bx-0.5.4/bx/data/masks/fdg_aging_mask.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/dcm.py` & `bbrc-bx-0.5.4/bx/dcm.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/donsurf.py` & `bbrc-bx-0.5.4/bx/donsurf.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/download.py` & `bbrc-bx-0.5.4/bx/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,18 @@
                 volumes = __braak_fdg__(x, e_id, r)
             elif subfunc == 'basil_perfusion':
                 volumes = r.perfusion()
             elif subfunc in ['basil_stats', 'qsmxt_stats']:
                 volumes = r.stats()
             elif subfunc == 'basil_aal':
                 volumes = __perfusion__(x, e_id, r)
+            elif subfunc == 'asl3d_perfusion':
+                volumes = r.perfusion().query('atlas  == "global"')
+            elif subfunc == 'asl3d_aal':
+                volumes = r.perfusion().query('atlas  == "aal2"')
             elif subfunc == 'aging':
                 volumes = __aging_fdg__(x, e_id, r)
             elif subfunc in ['brainstem', 'thalamus', 'hypothalamus']:
                 cmd = {'brainstem': 'brainstem_substructures_volumes',
                        'thalamus': 'thalamic_nuclei_volumes',
                        'hypothalamus': 'hypothalamic_subunits_volumes'}
                 volumes = eval('r.{}()'.format(cmd[subfunc]))
```

### Comparing `bbrc-bx-0.5.3/bx/dtifit.py` & `bbrc-bx-0.5.4/bx/dtifit.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/dump.py` & `bbrc-bx-0.5.4/bx/dump.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/fmriprep.py` & `bbrc-bx-0.5.4/bx/fmriprep.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/freesurfer.py` & `bbrc-bx-0.5.4/bx/freesurfer.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/id.py` & `bbrc-bx-0.5.4/bx/id.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/lcmodel.py` & `bbrc-bx-0.5.4/bx/lcmodel.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/lists.py` & `bbrc-bx-0.5.4/bx/lists.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/mrtrix3.py` & `bbrc-bx-0.5.4/bx/mrtrix3.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/nifti.py` & `bbrc-bx-0.5.4/bx/nifti.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/parse.py` & `bbrc-bx-0.5.4/bx/parse.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/pet.py` & `bbrc-bx-0.5.4/bx/pet.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/qsmxt.py` & `bbrc-bx-0.5.4/bx/qsmxt.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/scandates.py` & `bbrc-bx-0.5.4/bx/scandates.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/signature.py` & `bbrc-bx-0.5.4/bx/signature.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/spm12.py` & `bbrc-bx-0.5.4/bx/spm12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/validation.py` & `bbrc-bx-0.5.4/bx/validation.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/bx/xcpd.py` & `bbrc-bx-0.5.4/bx/xcpd.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
      snapshot:\t\tdownload snapshots from the XCPD pipeline
      tests:\t\tcreate an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx xcpd <subcommand> <resource_id>
 
     References:
-    - Ciric R, et al., Nat Protoc 13 (2018).
+    - Ciric R. et al., Nat Protoc 13 (2018).
+    - Mehta K., Salo T. et al., bioRxiv (2023). DOI: 10.1101/2023.11.20.567926
     """
     nargs = 2
     resource_name = 'XCP_D'
     subcommands = ['conmat', 'timeseries', 'files', 'report', 'snapshot', 'tests']
     validator = 'XCPDValidator'
     url = 'https://gitlab.com/bbrc/xnat/docker-images/-/tree/master/xcp_d'
```

### Comparing `bbrc-bx-0.5.3/bx/xnat.py` & `bbrc-bx-0.5.4/bx/xnat.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.3/setup.py` & `bbrc-bx-0.5.4/setup.py`

 * *Files identical despite different names*

