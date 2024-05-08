# Comparing `tmp/babelfont-3.0.4.tar.gz` & `tmp/babelfont-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelfont-3.0.4.tar", last modified: Wed Apr 17 10:16:00 2024, max compression
+gzip compressed data, was "babelfont-3.0.5.tar", last modified: Wed May  8 09:20:12 2024, max compression
```

## Comparing `babelfont-3.0.4.tar` & `babelfont-3.0.5.tar`

### file list

```diff
@@ -1,292 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.413966 babelfont-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 10:15:37.000000 babelfont-3.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.361965 babelfont-3.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.365965 babelfont-3.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 10:15:37.000000 babelfont-3.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 10:15:37.000000 babelfont-3.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:15:37.000000 babelfont-3.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 10:15:37.000000 babelfont-3.0.4/AUTHORS.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.361965 babelfont-3.0.4/Babelfont.glyphsFileFormat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.365965 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 10:15:37.000000 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.365965 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/MacOS/
--rwxr-xr-x   0 runner    (1001) docker     (127)   120208 2024-04-17 10:15:37.000000 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/MacOS/plugin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.365965 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Resources/
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 10:15:37.000000 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-17 10:15:37.000000 babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 10:15:37.000000 babelfont-3.0.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 10:15:37.000000 babelfont-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-17 10:15:37.000000 babelfont-3.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-17 10:16:00.413966 babelfont-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-17 10:15:37.000000 babelfont-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.369965 babelfont-3.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Anchor.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Axis.md
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Font.md
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Gemfile
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Gemfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Glyph.md
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Instance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Master.md
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Names.md
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/Shape.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.369965 babelfont-3.0.4/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/_data/navigation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    36234 2024-04-17 10:15:37.000000 babelfont-3.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-17 10:15:37.000000 babelfont-3.0.4/makedoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56244 2024-04-17 10:15:37.000000 babelfont-3.0.4/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 10:15:37.000000 babelfont-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-17 10:15:37.000000 babelfont-3.0.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:16:00.413966 babelfont-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.361965 babelfont-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.373965 babelfont-3.0.4/src/babelfont/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/BaseObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Font.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Guide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Master.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Names.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/Shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.373965 babelfont-3.0.4/src/babelfont/convertors/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/designspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/fontforge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.373965 babelfont-3.0.4/src/babelfont/convertors/fontlab/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/fontlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/fontlab/vfj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.377965 babelfont-3.0.4/src/babelfont/convertors/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/glyphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphs2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26782 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphs3.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphspackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/glyphs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/nfsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/truetype.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/convertors/ufo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.377965 babelfont-3.0.4/src/babelfont/fontFilters/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/fontFilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/fontFilters/anchorPropagation.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/fontFilters/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/fontFilters/featureWriters.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 10:15:37.000000 babelfont-3.0.4/src/babelfont/fontFilters/marks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.413966 babelfont-3.0.4/src/babelfont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 10:16:00.000000 babelfont-3.0.4/src/babelfont.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 10:15:37.000000 babelfont-3.0.4/t.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.377965 babelfont-3.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.381965 babelfont-3.0.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1118555 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Castoro Roman.vfj
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Glyphs2ManyAxes.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/GlyphsFileFormatv3.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/GlyphsFileFormatv3.vfj
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/LICENSE_MutatorSans
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/LICENSE_UbuTestData.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/NewFont-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Nunito-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (127)   157208 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Nunito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53914 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/SimpleTwoAxis.vfj
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/SimpleTwoAxis3.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.381965 babelfont-3.0.4/tests/data/Test1.roundtrip.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.roundtrip.ufo/features.fea
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.385965 babelfont-3.0.4/tests/data/Test1.ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/features.fea
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.385965 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/A_.glif
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/B_.glif
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/contents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/i.glif
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/glyphs/idotless.glif
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/groups.plist
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/kerning.plist
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/layercontents.plist
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/lib.plist
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Test1.ufo/metainfo.plist
--rw-r--r--   0 runner    (1001) docker     (127)   432392 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/Ysabeau[wght].ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.385965 babelfont-3.0.4/tests/data/glyphsLib/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestBasic.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestFileName.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestInactive.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.385965 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.389965 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/order.plist
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/TestReencode.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.389965 babelfont-3.0.4/tests/data/glyphsLib/master_ufo/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:16:00.413966 babelfont-3.0.4/tests/data/testotfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1c2c3fc37b2d4c3cb2ef726c6cdaaabd4b7f3eb9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   125256 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    21160 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    22980 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/HBTest-VF.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/MORXTwentyeight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/TRAK.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   106096 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_glyphs2.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_glyphs3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_glyphs3_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_otf_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_ufo_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 10:15:37.000000 babelfont-3.0.4/tests/test_vfj_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.753008 babelfont-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-08 09:19:57.000000 babelfont-3.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.689008 babelfont-3.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.697008 babelfont-3.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 09:19:58.000000 babelfont-3.0.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-08 09:19:58.000000 babelfont-3.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 09:19:58.000000 babelfont-3.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 09:19:58.000000 babelfont-3.0.5/AUTHORS.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.689008 babelfont-3.0.5/Babelfont.glyphsFileFormat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.697008 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-08 09:19:58.000000 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.697008 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/MacOS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120208 2024-05-08 09:19:58.000000 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/MacOS/plugin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.697008 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-08 09:19:58.000000 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-05-08 09:19:58.000000 babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 09:19:58.000000 babelfont-3.0.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 09:19:58.000000 babelfont-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-08 09:19:58.000000 babelfont-3.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-08 09:20:12.753008 babelfont-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-08 09:19:58.000000 babelfont-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.701008 babelfont-3.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Anchor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Axis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Font.md
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Gemfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Glyph.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Instance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Master.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Names.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/Shape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.701008 babelfont-3.0.5/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/_data/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    36234 2024-05-08 09:19:58.000000 babelfont-3.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-08 09:19:58.000000 babelfont-3.0.5/makedoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56244 2024-05-08 09:19:58.000000 babelfont-3.0.5/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 09:19:58.000000 babelfont-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 09:19:58.000000 babelfont-3.0.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:20:12.753008 babelfont-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.693008 babelfont-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.705008 babelfont-3.0.5/src/babelfont/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/BaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.705008 babelfont-3.0.5/src/babelfont/convertors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/fontforge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.705008 babelfont-3.0.5/src/babelfont/convertors/fontlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/fontlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/fontlab/vfb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/fontlab/vfj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.709008 babelfont-3.0.5/src/babelfont/convertors/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/glyphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16492 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphspackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/glyphs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14657 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/nfsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/convertors/ufo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.713008 babelfont-3.0.5/src/babelfont/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  5067653 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/data/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.717008 babelfont-3.0.5/src/babelfont/fontFilters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/anchorPropagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/cu2qu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/decomposeMixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/dropUnexported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/featureWriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/fillOpentype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/glyphDataXML.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-08 09:19:58.000000 babelfont-3.0.5/src/babelfont/fontFilters/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.753008 babelfont-3.0.5/src/babelfont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:20:12.000000 babelfont-3.0.5/src/babelfont.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 09:19:58.000000 babelfont-3.0.5/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.717008 babelfont-3.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.721008 babelfont-3.0.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1118555 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Castoro Roman.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Designspace.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Glyphs2ManyAxes.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/GlyphsFileFormatv3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/GlyphsFileFormatv3.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/LICENSE_MutatorSans
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/LICENSE_UbuTestData.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/NewFont-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Nunito-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   157208 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53914 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/SimpleTwoAxis.vfj
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/SimpleTwoAxis3.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.721008 babelfont-3.0.5/tests/data/Test1.roundtrip.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.roundtrip.ufo/features.fea
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.725008 babelfont-3.0.5/tests/data/Test1.ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/features.fea
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.725008 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/A_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/B_.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/contents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/i.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/glyphs/idotless.glif
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/groups.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/kerning.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/layercontents.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/lib.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Test1.ufo/metainfo.plist
+-rw-r--r--   0 runner    (1001) docker     (127)   432392 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/Ysabeau[wght].ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.725008 babelfont-3.0.5/tests/data/glyphsLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestBasic.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestFileName.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestInactive.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.729008 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.729008 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/order.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/TestReencode.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.729008 babelfont-3.0.5/tests/data/glyphsLib/master_ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:20:12.753008 babelfont-3.0.5/tests/data/testotfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1c2c3fc37b2d4c3cb2ef726c6cdaaabd4b7f3eb9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125256 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    21160 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    22980 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/HBTest-VF.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/MORXTwentyeight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/TRAK.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106096 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    34116 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_glyphs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_glyphs3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_glyphs3_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_otf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_ufo_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 09:19:58.000000 babelfont-3.0.5/tests/test_vfj_loader.py
```

### Comparing `babelfont-3.0.4/.github/workflows/ci.yml` & `babelfont-3.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/.gitignore` & `babelfont-3.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Info.plist` & `babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/MacOS/plugin` & `babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/MacOS/plugin`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf` & `babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Resources/ExportIconTemplate.pdf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py` & `babelfont-3.0.5/Babelfont.glyphsFileFormat/Contents/Resources/plugin.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/LICENSE` & `babelfont-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/Makefile` & `babelfont-3.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/PKG-INFO` & `babelfont-3.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: babelfont
-Version: 3.0.4
+Version: 3.0.5
 Summary: Load, examine and save fonts in a variety of formats
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 Requires-Dist: orjson>=3.5.1
 Requires-Dist: fonttools>=4.40.0
 Requires-Dist: ufoLib2>=0.11.1
 Requires-Dist: openstep-plist>=0.2.2
-Requires-Dist: glyphsLib>=5.3.2
+Requires-Dist: glyphsLib>=6.7.1
 Requires-Dist: fontfeatures>=1.8.0
+Requires-Dist: vfbLib>=0.6.4
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: defcon; extra == "dev"
 
 # Babelfont: Load, examine and save fonts in a variety of formats
 
 *This describes Babelfont >3.0, which is a complete rewrite from the previous version.*
 
 Babelfont is a utility for loading fonts and examining fonts in a variety
 of formats. It can also be used to *write* fonts in some of these formats,
 making it possible to convert between font formats.
 
 Here are the formats which are currently supported:
 
-| Format         | Read    | Write |
-|----------------|---------|-------|
-| Glyphs 2       | *       | *     |
-| Glyphs 3       | *       | *     |
-| .glyphspackage | *       |       |
-| UFO            | *       |       |
-| Designspace    | *       |       |
-| Fontlab VFJ    | partial |       |
-| TTF            | partial | *     |
-| OTF            | partial |       |
-| Babelfont      | *       | *     |
+| Format          | Read    | Write |
+|-----------------|---------|-------|
+| Glyphs 2        | partial |       |
+| Glyphs 3        | *       | *     |
+| .glyphspackage  | *       |       |
+| UFO             | *       |       |
+| Designspace     | *       |       |
+| Fontlab VFJ     | partial |       |
+| Fontlab VFB     | partial |       |
+| TTF             | partial | *     |
+| OTF             | partial |       |
+| Fontforge SFD   | partial | *     |
+| Fontforge SFDir | partial | *     |
+| Babelfont       | *       | *     |
 
 Babelfont converts all of the above font formats into a intermediary
 set of objects, whose object hierarchy can be seen [here](https://simoncozens.github.io/babelfont). The allows
 the developer to examine any font (single master or variable), without
 needing to worry about the details of each font format.
 
 For example:
```

### Comparing `babelfont-3.0.4/README.md` & `babelfont-3.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 
 Babelfont is a utility for loading fonts and examining fonts in a variety
 of formats. It can also be used to *write* fonts in some of these formats,
 making it possible to convert between font formats.
 
 Here are the formats which are currently supported:
 
-| Format         | Read    | Write |
-|----------------|---------|-------|
-| Glyphs 2       | *       | *     |
-| Glyphs 3       | *       | *     |
-| .glyphspackage | *       |       |
-| UFO            | *       |       |
-| Designspace    | *       |       |
-| Fontlab VFJ    | partial |       |
-| TTF            | partial | *     |
-| OTF            | partial |       |
-| Babelfont      | *       | *     |
+| Format          | Read    | Write |
+|-----------------|---------|-------|
+| Glyphs 2        | partial |       |
+| Glyphs 3        | *       | *     |
+| .glyphspackage  | *       |       |
+| UFO             | *       |       |
+| Designspace     | *       |       |
+| Fontlab VFJ     | partial |       |
+| Fontlab VFB     | partial |       |
+| TTF             | partial | *     |
+| OTF             | partial |       |
+| Fontforge SFD   | partial | *     |
+| Fontforge SFDir | partial | *     |
+| Babelfont       | *       | *     |
 
 Babelfont converts all of the above font formats into a intermediary
 set of objects, whose object hierarchy can be seen [here](https://simoncozens.github.io/babelfont). The allows
 the developer to examine any font (single master or variable), without
 needing to worry about the details of each font format.
 
 For example:
```

### Comparing `babelfont-3.0.4/docs/Anchor.md` & `babelfont-3.0.5/docs/Anchor.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Axis.md` & `babelfont-3.0.5/docs/Axis.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Font.md` & `babelfont-3.0.5/docs/Font.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Gemfile.lock` & `babelfont-3.0.5/docs/Gemfile.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 GEM
   remote: https://rubygems.org/
   specs:
-    activesupport (6.1.2)
+    activesupport (7.1.3.2)
+      base64
+      bigdecimal
       concurrent-ruby (~> 1.0, >= 1.0.2)
+      connection_pool (>= 2.2.5)
+      drb
       i18n (>= 1.6, < 2)
       minitest (>= 5.1)
+      mutex_m
       tzinfo (~> 2.0)
-      zeitwerk (~> 2.3)
     addressable (2.7.0)
       public_suffix (>= 2.0.2, < 5.0)
+    base64 (0.2.0)
+    bigdecimal (3.1.7)
     colorator (1.1.0)
-    concurrent-ruby (1.1.8)
+    concurrent-ruby (1.2.3)
+    connection_pool (2.4.1)
+    drb (2.2.1)
     em-websocket (0.5.2)
       eventmachine (>= 0.12.9)
       http_parser.rb (~> 0.6.0)
     eventmachine (1.2.7)
     faraday (1.3.0)
       faraday-net_http (~> 1.0)
       multipart-post (>= 1.2, < 3)
@@ -23,15 +31,15 @@
     ffi (1.14.2)
     forwardable-extended (2.6.0)
     gemoji (3.0.1)
     html-pipeline (2.14.0)
       activesupport (>= 2)
       nokogiri (>= 1.4)
     http_parser.rb (0.6.0)
-    i18n (1.8.8)
+    i18n (1.14.4)
       concurrent-ruby (~> 1.0)
     jekyll (4.2.0)
       addressable (~> 2.4)
       colorator (~> 1.0)
       em-websocket (~> 0.5)
       i18n (~> 1.0)
       jekyll-sass-converter (~> 2.0)
@@ -62,56 +70,56 @@
       jekyll (>= 3.7, < 5.0)
     jekyll-watch (2.2.1)
       listen (~> 3.0)
     jemoji (0.12.0)
       gemoji (~> 3.0)
       html-pipeline (~> 2.2)
       jekyll (>= 3.0, < 5.0)
-    kramdown (2.3.0)
+    kramdown (2.4.0)
       rexml
     kramdown-parser-gfm (1.1.0)
       kramdown (~> 2.0)
     liquid (4.0.3)
     listen (3.4.1)
       rb-fsevent (~> 0.10, >= 0.10.3)
       rb-inotify (~> 0.9, >= 0.9.10)
     mercenary (0.4.0)
-    mini_portile2 (2.5.0)
-    minitest (5.14.3)
+    mini_portile2 (2.8.6)
+    minitest (5.22.3)
     multipart-post (2.1.1)
-    nokogiri (1.11.1)
-      mini_portile2 (~> 2.5.0)
+    mutex_m (0.2.0)
+    nokogiri (1.16.4)
+      mini_portile2 (~> 2.8.2)
       racc (~> 1.4)
     octokit (4.20.0)
       faraday (>= 0.9)
       sawyer (~> 0.8.0, >= 0.5.3)
     pathutil (0.16.2)
       forwardable-extended (~> 2.6)
     public_suffix (4.0.6)
-    racc (1.5.2)
+    racc (1.7.3)
     rake (13.0.3)
     rb-fsevent (0.10.4)
     rb-inotify (0.10.1)
       ffi (~> 1.0)
-    rexml (3.2.4)
+    rexml (3.2.6)
     rouge (3.26.0)
     ruby2_keywords (0.0.4)
     rubyzip (2.3.0)
     safe_yaml (1.0.5)
     sassc (2.4.0)
       ffi (~> 1.9)
     sawyer (0.8.2)
       addressable (>= 2.3.5)
       faraday (> 0.8, < 2.0)
     terminal-table (2.0.0)
       unicode-display_width (~> 1.1, >= 1.1.1)
-    tzinfo (2.0.4)
+    tzinfo (2.0.6)
       concurrent-ruby (~> 1.0)
     unicode-display_width (1.7.0)
-    zeitwerk (2.4.2)
 
 PLATFORMS
   ruby
 
 DEPENDENCIES
   jekyll
   jekyll-feed
```

### Comparing `babelfont-3.0.4/docs/Glyph.md` & `babelfont-3.0.5/docs/Glyph.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Guide.md` & `babelfont-3.0.5/docs/Guide.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Instance.md` & `babelfont-3.0.5/docs/Instance.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Layer.md` & `babelfont-3.0.5/docs/Layer.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Master.md` & `babelfont-3.0.5/docs/Master.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Names.md` & `babelfont-3.0.5/docs/Names.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/Shape.md` & `babelfont-3.0.5/docs/Shape.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/docs/index.md` & `babelfont-3.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/makedoc.py` & `babelfont-3.0.5/makedoc.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/poetry.lock` & `babelfont-3.0.5/poetry.lock`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/pyproject.toml` & `babelfont-3.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
-   "setuptools>=45",
-   "setuptools_scm[toml]>=6.2"
+   "setuptools>=69.5.1",
+   "setuptools_scm[toml]>=8.1.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
@@ -18,16 +18,17 @@
 readme = "README.md"
 
 dependencies = [
     "orjson >= 3.5.1",
     "fonttools >=4.40.0",
     "ufoLib2 >=0.11.1",
     "openstep-plist >=0.2.2",
-    "glyphsLib >=5.3.2",
+    "glyphsLib >=6.7.1",
     "fontfeatures >= 1.8.0",
+    "vfbLib >= 0.6.4",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "defcon"
 ]
```

### Comparing `babelfont-3.0.4/src/babelfont/Axis.py` & `babelfont-3.0.5/src/babelfont/Axis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from typing import Optional, Dict, Tuple
-from .BaseObject import BaseObject, I18NDictionary
+from typing import List, Optional, Dict, Tuple
+from .BaseObject import BaseObject, I18NDictionary, Number
 from dataclasses import dataclass, field
 import uuid
-from fontTools.varLib.models import normalizeValue
+from fontTools.varLib.models import normalizeValue, piecewiseLinearMap
+
+
+Tag = str
 
 
 @dataclass
 class _AxisFields:
     name: I18NDictionary = field(
         metadata={"description": "The display name for this axis."}
     )
-    tag: str = field(metadata={"description": "The four-letter axis tag."})
+    tag: Tag = field(metadata={"description": "The four-letter axis tag."})
     id: str = field(
         default_factory=lambda: str(uuid.uuid1()),
         repr=False,
         metadata={
             "description": """An ID used to refer to this axis in the Master,
 Layer and Instance `location` fields. (This is allows the user to change the
 axis tag without the locations becoming lost.) If not provided, one will be
@@ -38,15 +41,15 @@
         metadata={
             "description": """The default value of this axis (center of interpolation),
 in user space coordinates. Note that if the min/max/default values are not supplied,
 they are returned as `None` in the Python object, and should be computed from the
 master locations on export."""
         },
     )
-    map: [(int, int)] = field(
+    map: List[Tuple[int, int]] = field(
         default=None,
         metadata={
             "description": """The mapping between userspace and designspace coordinates."""
         },
     )
     hidden: bool = field(
         default=False,
@@ -66,25 +69,28 @@
 
     def __post_init__(self):
         # If they smacked my name with a bare string, replace with I18NDict
         if isinstance(self.name, str):
             self.name = I18NDictionary.with_default(self.name)
         super().__post_init__()
 
-    def normalize_value(self, value):
+    def normalize_value(self, value: Number) -> float:
+        """Return a normalized co-ordinate (-1.0 to 1.0) for the given value.
+        The value provided is expected to be in userspace coordinates."""
         return normalizeValue(
-            self.map_forward(value),
+            self.userspace_to_designspace(value),
             (
-                self.map_forward(self.min),
-                self.map_forward(self.default),
-                self.map_forward(self.max),
+                self.userspace_to_designspace(self.min),
+                self.userspace_to_designspace(self.default),
+                self.userspace_to_designspace(self.max),
             ),
         )
 
-    def denormalize_value(self, value):
+    def denormalize_value(self, value: float) -> Number:
+        """Return a userspace coordinate for the given normalized value."""
         if value == 0:
             return self.default
         elif value > 0:
             return self.default + (self.max - self.default) * value
         else:
             return self.default + (self.default - self.min) * value
 
@@ -112,33 +118,34 @@
 
     @property
     def defaultValue(self):
         return self.default
 
     @property
     def inverted_map(self) -> Optional[Tuple[float, float]]:
+        """Return the axis map as a list of tuples, where the first value is the
+        designspace coordinate and the second value is the userspace coordinate."""
         if not self.map:
             return None
         return [(v, k) for k, v in self.map]
 
     # Stolen from fontTools.designspaceLib
-
-    def map_forward(self, v):
-        from fontTools.varLib.models import piecewiseLinearMap
-
+    def map_forward(self, v: Number) -> Number:
+        """Map a location on this axis from userspace to designspace."""
         if not self.map:
             return v
         return piecewiseLinearMap(v, dict(self.map))
 
-    def map_backward(self, v):
-        from fontTools.varLib.models import piecewiseLinearMap
-
+    def map_backward(self, v: Number) -> Number:
+        """Map a location on this axis from designspace to userspace."""
         if not self.map:
             return v
         return piecewiseLinearMap(v, {v: k for k, v in self.map})
 
     # These are just better names
-    def userspace_to_designspace(self, v):
+    def userspace_to_designspace(self, v: Number) -> Number:
+        """Map a location on this axis from userspace to designspace."""
         return self.map_forward(v)
 
-    def designspace_to_userspace(self, v):
+    def designspace_to_userspace(self, v: Number) -> Number:
+        """Map a location on this axis from designspace to userspace."""
         return self.map_backward(v)
```

### Comparing `babelfont-3.0.4/src/babelfont/BaseObject.py` & `babelfont-3.0.5/src/babelfont/BaseObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import dataclass, fields, field
+from typing import Union
 import orjson
 from collections import namedtuple
 import datetime
 
 
 class IncompatibleMastersError(ValueError):
     pass
 
 
 Color = namedtuple("Color", "r,g,b,a", defaults=[0, 0, 0, 0])
 Position = namedtuple("Position", "x,y,angle", defaults=[0, 0, 0])
-
-
-@dataclass
-class OTValue:
-    table: str
-    field: str
-    value: any
+Number = Union[int, float]
 
 
 class I18NDictionary(dict):
     @classmethod
     def with_default(cls, s):
         inst = cls()
         inst.set_default(s)
```

### Comparing `babelfont-3.0.4/src/babelfont/Font.py` & `babelfont-3.0.5/src/babelfont/Font.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import functools
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import Dict, List
+from typing import Any, Dict, List, Optional, Tuple
 
 from fontTools.feaLib.variableScalar import VariableScalar
 from fontTools.varLib.models import VariationModel
 
-from .Axis import Axis
-from .BaseObject import BaseObject, IncompatibleMastersError, OTValue
+from .Axis import Axis, Tag
+from .BaseObject import BaseObject, IncompatibleMastersError, Number
 from .Features import Features
 from .Glyph import GlyphList
 from .Instance import Instance
 from .Master import Master
 from .Names import Names
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class _FontFields:
     upm: int = field(default=1000, metadata={"description": "The font's units per em."})
-    version: (int, int) = field(
+    version: Tuple[int, int] = field(
         default=(1, 0),
         metadata={
             "description": "Font version number as a tuple of integers (major, minor).",
             "json_type": "[int,int]",
         },
     )
-    axes: [Axis] = field(
+    axes: List[Axis] = field(
         default_factory=list,
         metadata={
             "separate_items": True,
             "description": "A list of axes, in the case of variable/multiple master font. May be empty.",
         },
     )
-    instances: [Instance] = field(
+    instances: List[Instance] = field(
         default_factory=list,
         metadata={
             "separate_items": True,
             "description": "A list of named/static instances.",
         },
     )
-    masters: [Master] = field(
+    masters: List[Master] = field(
         default_factory=list,
         metadata={
             "separate_items": True,
             "description": "A list of the font's masters.",
         },
     )
     glyphs: GlyphList = field(
@@ -86,16 +86,16 @@
             "description": """The font's date. When writing to Babelfont-JSON, this
 should be stored in the format `%Y-%m-%d %H:%M:%S`. *If not provided, defaults
 to the current date/time*.""",
             "json_type": "str",
         },
     )
     names: Names = field(default_factory=Names, metadata={"skip_serialize": True})
-    customOpenTypeValues: [OTValue] = field(
-        default_factory=list,
+    custom_opentype_values: Dict[Tuple[str, str], Any] = field(
+        default_factory=dict,
         metadata={
             "description": "Any values to be placed in OpenType tables on export to override defaults; these must be font-wide. Metrics which may vary by master should be placed in the `metrics` field of a Master."
         },
     )
     features: Features = field(
         default_factory=Features,
         metadata={
@@ -122,62 +122,80 @@
 
     def __repr__(self):
         return "<Font '%s' (%i masters)>" % (
             self.names.familyName.get_default(),
             len(self.masters),
         )
 
-    def save(self, filename, **kwargs):
+    def save(self, filename: str, **kwargs):
+        """Save the font to a file. The file type is determined by the extension.
+        Any additional keyword arguments are passed to the save method of the
+        appropriate converter."""
         from .convertors import Convert
 
         return Convert(filename).save(self, **kwargs)
 
-    def master(self, mid):
+    def master(self, mid: str) -> Optional[Master]:
+        """Locates a master by its ID. Returns `None` if not found."""
         return self._master_map[mid]
 
-    def map_forward(self, location):
+    def map_forward(self, location: dict[Tag, Number]) -> dict[Tag, Number]:
+        """Map a location (dictionary of `tag: number`) from userspace to designspace."""
         location2 = dict(location)
         for a in self.axes:
             if a.tag in location2:
                 location2[a.tag] = a.map_forward(location2[a.tag])
         return location2
 
-    def map_backward(self, location):
+    def map_backward(self, location: dict[Tag, Number]) -> dict[Tag, Number]:
+        """Map a location (dictionary of `tag: number`) from designspace to userspace."""
         location2 = dict(location)
         for a in self.axes:
             if a.tag in location2:
                 location2[a.tag] = a.map_backward(location2[a.tag])
         return location2
 
+    def userspace_to_designspace(self, v: dict[Tag, Number]) -> dict[Tag, Number]:
+        """Map a location (dictionary of `tag: number`) from userspace to designspace."""
+        return self.map_forward(v)
+
+    def designspace_to_userspace(self, v: dict[Tag, Number]) -> dict[Tag, Number]:
+        """Map a location (dictionary of `tag: number`) from designspace to userspace."""
+        return self.map_backward(v)
+
     @functools.cached_property
-    def default_master(self):
+    def default_master(self) -> Master:
+        """Return the default master. If there is only one master, return it.
+        If there are multiple masters, return the one with the default location.
+        If there is no default location, raise an error."""
         default_loc = {a.tag: a.userspace_to_designspace(a.default) for a in self.axes}
         for m in self.masters:
             if m.location == default_loc:
                 return m
         if len(self.masters) == 1:
             return self.masters[0]
         raise ValueError("Could not determine default master")
 
     @functools.cached_property
     def _master_map(self):
         return {m.id: m for m in self.masters}
 
     @functools.cached_property
-    def unicode_map(self):
+    def unicode_map(self) -> Dict[int, str]:
+        """Return a dictionary mapping Unicode codepoints to glyph names."""
         unicodes = {}
         for g in self.glyphs:
-            if not g.codepoints:
-                continue
             for u in g.codepoints:
-                if u:
+                if u is not None:
                     unicodes[u] = g.name
         return unicodes
 
-    def variation_model(self):
+    def variation_model(self) -> VariationModel:
+        """Return a `fontTools.varLib.models.VariationModel` object representing
+        the font's axes and masters. This is used for generating variable fonts."""
         return VariationModel(
             [m.normalized_location for m in self.masters],
             axisOrder=[a.tag for a in self.axes],
         )
 
     @functools.cached_property
     def _all_kerning(self):
@@ -213,15 +231,21 @@
                         continue
                     has_mark = a
                 if a not in _all_anchors_dict:
                     _all_anchors_dict[a] = {}
                 _all_anchors_dict[a][g] = self.get_variable_anchor(g, a)
         return _all_anchors_dict
 
-    def get_variable_anchor(self, glyph, anchorname):
+    def get_variable_anchor(
+        self, glyph, anchorname
+    ) -> Tuple[VariableScalar, VariableScalar]:
+        """Return a tuple of `VariableScalar` objects representing the x and y
+        coordinates of the anchor on the given glyph. The `VariableScalar` objects
+        are indexed by master location. If the anchor is not found on some master,
+        raise an `IncompatibleMastersError`."""
         x_vs = VariableScalar()
         x_vs.axes = self.axes
         y_vs = VariableScalar()
         y_vs.axes = self.axes
         for ix, m in enumerate(self.masters):
             layer = m.get_glyph_layer(glyph)
             if anchorname not in layer.anchors_dict:
@@ -230,9 +254,10 @@
                     % (anchorname, glyph, m)
                 )
             anchor = m.get_glyph_layer(glyph).anchors_dict[anchorname]
             x_vs.add_value(self.map_forward(m.location), anchor.x)
             y_vs.add_value(self.map_forward(m.location), anchor.y)
         return (x_vs, y_vs)
 
-    def exportedGlyphs(self):
+    def exported_glyphs(self) -> List[str]:
+        """Return a list of glyph names that are marked for export."""
         return [g.name for g in self.glyphs if g.exported]
```

### Comparing `babelfont-3.0.4/src/babelfont/Glyph.py` & `babelfont-3.0.5/src/babelfont/Glyph.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/Instance.py` & `babelfont-3.0.5/src/babelfont/Instance.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/Layer.py` & `babelfont-3.0.5/src/babelfont/Layer.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/Master.py` & `babelfont-3.0.5/src/babelfont/Master.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,21 @@
     location: dict = field(
         default=None,
         metadata={
             "description": """A dictionary mapping axis tags to coordinates
 in order to locate this master in the design space. The coordinates are in designspace units."""
         },
     )
+    sparse: bool = field(
+        default=False,
+        repr=False,
+        metadata={
+            "description": """If true, this master is sparse and may not have all glyphs"""
+        },
+    )
     guides: [Guide] = field(
         default_factory=list,
         repr=False,
         metadata={"separate_items": True, "description": "A list of guides."},
     )
     metrics: dict = field(
         default_factory=dict,
```

### Comparing `babelfont-3.0.4/src/babelfont/Names.py` & `babelfont-3.0.5/src/babelfont/Names.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,52 @@
 from .BaseObject import BaseObject, I18NDictionary
 from dataclasses import dataclass, asdict
 
+OPENTYPE_NAMES = [
+    "copyright",
+    "familyName",
+    "preferredSubfamilyName",
+    "uniqueID",
+    "fullName",  # XXX?
+    "version",
+    "postscriptName",
+    "trademark",
+    "manufacturer",
+    "designer",
+    "description",
+    "manufacturerURL",
+    "designerURL",
+    "license",
+    "licenseURL",
+    "reserved",
+    "typographicFamily",
+    "typographicSubfamily",
+    "compatibleFullName",
+    "sampleText",
+    "postscriptCIDname",  # XXX?
+    "WWSFamilyName",
+    "WWSSubfamilyName",
+]
+
 
 @dataclass
 class Names(BaseObject):
     """A table of global, localizable names for the font."""
 
     familyName: I18NDictionary = None
     designer: I18NDictionary = None
     designerURL: I18NDictionary = None
     manufacturer: I18NDictionary = None
     manufacturerURL: I18NDictionary = None
     license: I18NDictionary = None
     licenseURL: I18NDictionary = None
     version: I18NDictionary = None
     uniqueID: I18NDictionary = None
+    postscriptName: I18NDictionary = None
+    fullName: I18NDictionary = None
     description: I18NDictionary = None
     typographicFamily: I18NDictionary = None
     typographicSubfamily: I18NDictionary = None
     compatibleFullName: I18NDictionary = None
     sampleText: I18NDictionary = None
     WWSFamilyName: I18NDictionary = None
     WWSSubfamilyName: I18NDictionary = None
```

### Comparing `babelfont-3.0.4/src/babelfont/Node.py` & `babelfont-3.0.5/src/babelfont/Node.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/Shape.py` & `babelfont-3.0.5/src/babelfont/Shape.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/__init__.py` & `babelfont-3.0.5/src/babelfont/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from babelfont.Anchor import Anchor
 from babelfont.Axis import Axis
-from babelfont.BaseObject import Color, I18NDictionary, OTValue, Position
+from babelfont.BaseObject import Color, I18NDictionary, Position
 from babelfont.convertors import BaseConvertor, Convert
 from babelfont.Features import Features
 from babelfont.Font import Font
 from babelfont.Glyph import Glyph
 from babelfont.Guide import Guide
 from babelfont.Instance import Instance
 from babelfont.Layer import Layer
@@ -24,15 +24,14 @@
     "Layer",
     "Shape",
     "Transform",
     "Node",
     "Names",
     "Color",
     "Position",
-    "OTValue",
     "I18NDictionary",
     "Convert",
     "BaseConvertor",
     "Features",
     "load",
 ]
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/__init__.py` & `babelfont-3.0.5/src/babelfont/convertors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 import pkgutil
 import inspect
 import importlib
 import logging
 
 from babelfont.Font import Font
 
+logger = logging.getLogger(__name__)
+
 
 class BaseConvertor:
     filename: str
     scratch: object
     font: Font
     compile_only: bool
 
     suffix = ".XXX"
 
+    LOAD_FILTERS = []
+    COMPILE_FILTERS = []
+    SAVE_FILTERS = []
+
     def __init__(self):
         self.logger = logging.getLogger(self.__class__.__name__)
 
     @classmethod
     def can_load(cls, other, **kwargs):
         return other.filename.endswith(cls.suffix)
 
@@ -78,18 +84,30 @@
             cls.convertors.extend(classes)
 
     def __init__(self, filename):
         self._load_convertors()
         self.filename = filename
         self.scratch = {}
 
-    def load(self, **kwargs):
+    def load_convertor(self, **kwargs):
         for c in self.convertors:
             if c.can_load(self, **kwargs):
-                return c.load(self, **kwargs)
-        raise NotImplementedError
+                return c
 
-    def save(self, obj, **kwargs):
+    def save_convertor(self, **kwargs):
         for c in self.convertors:
             if c.can_save(self, **kwargs):
-                return c.save(obj, self, **kwargs)
-        raise NotImplementedError
+                return c
+
+    def load(self, **kwargs):
+        c = self.load_convertor(**kwargs)
+        if not c:
+            logger.error("Could not find a convertor from %s", self.filename)
+            raise NotImplementedError
+        return c.load(self, **kwargs)
+
+    def save(self, obj, **kwargs):
+        c = self.save_convertor(**kwargs)
+        if not c:
+            logger.error("Could not find a convertor to %s", self.filename)
+            raise NotImplementedError
+        return c.save(obj, self, **kwargs)
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/designspace.py` & `babelfont-3.0.5/src/babelfont/convertors/designspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 from typing import Dict, List
+import time
 import uuid
 
 import ufoLib2
 from fontTools import designspaceLib
 from fontTools.designspaceLib import DesignSpaceDocument
+from fontTools.misc import timeTools
 
 from babelfont import (
     Features,
     Font,
     Master,
     Instance,
     Glyph,
@@ -16,15 +18,14 @@
     Shape,
     Node,
     Anchor,
     Guide,
     Axis,
     I18NDictionary,
 )
-from babelfont.BaseObject import OTValue
 from babelfont.convertors import BaseConvertor
 
 log = logging.getLogger(__name__)
 
 UFO_KEY = "org.unifiedfontobject"
 
 metrics = {
@@ -56,15 +57,15 @@
     "hheaCaretSlopeRise": "openTypeHheaCaretSlopeRise",
     "hheaCaretSlopeRun": "openTypeHheaCaretSlopeRun",
     "hheaCaretOffset": "openTypeHheaCaretOffset",
 }
 
 # Unicode ranges / code page ranges are special
 
-custom_opentype_values = {
+ufo_custom_opentype_values = {
     "openTypeGaspRangeRecords": ("GASP", "gaspRange"),
     # XX more gasp here
     "openTypeHeadCreated": ("head", "created"),
     "openTypeHeadLowestRecPPEM": ("head", "lowestRecPPEM"),
     "openTypeHeadFlags": ("head", "flags"),
     "openTypeOS2WidthClass": ("OS/2", "usWidthClass"),
     "openTypeOS2WeightClass": ("OS/2", "usWeightClass"),
@@ -182,17 +183,14 @@
         master.font = self.font
         master.kerning = self._load_kerning(source)
         for key, value in font.lib.items():
             if not key.startswith("public."):
                 if UFO_KEY not in master._formatspecific:
                     master._formatspecific[UFO_KEY] = {}
                 master._formatspecific[UFO_KEY][key] = value
-
-        master.features = Features.from_fea(font.features.text)
-        self._load_groups(font.groups)
         assert master.valid
         return master
 
     def _load_groups(self, groups: Dict[str, List[str]]):
         for name, value in groups.items():
             self.font.features.classes[name] = value
 
@@ -302,22 +300,23 @@
         self.font.upm = firstfontinfo.unitsPerEm
         self.font.version = (firstfontinfo.versionMajor, firstfontinfo.versionMinor)
         self.font.note = firstfontinfo.note
         for ours, theirs in self.names_dict.items():
             their_value = getattr(firstfontinfo, theirs)
             if their_value:
                 getattr(self.font.names, ours).set_default(their_value)
-        for ufofield, (table, field) in custom_opentype_values.items():
+        for ufofield, (table, field) in ufo_custom_opentype_values.items():
             if getattr(firstfontinfo, ufofield) is not None:
                 value = getattr(firstfontinfo, ufofield)
                 if (table, field) in BITARRAY:
                     value = bitarray_to_int(value)
-                self.font.customOpenTypeValues.append(
-                    OTValue(table=table, field=field, value=value)
-                )
+                self.font.custom_opentype_values[(table, field)] = value
+
+        self.font.features = Features.from_fea(ufo.features.text, glyphNames=ufo.keys())
+        self._load_groups(ufo.groups)
 
     def _save(self):
         self.ds = DesignSpaceDocument()
         self.save_axes()
         self.save_sources()
         self.save_instances()
         # Lib
@@ -460,25 +459,29 @@
         for our_metric, their_metric in metrics.items():
             if our_metric in master.metrics:
                 metric_value = master.metrics[our_metric]
                 if their_metric in ["openTypeOS2WinDescent"] and metric_value < 0:
                     metric_value = -metric_value
                 setattr(ufo.info, their_metric, metric_value)
         if is_default:
-            for info_tag, (table, field) in custom_opentype_values.items():
-                for otv in self.font.customOpenTypeValues:
-                    if otv.table == table and otv.field == field:
-                        value = otv.value
-                        if (table, field) in BITARRAY:
-                            if info_tag == "openTypeOS2Selection":
-                                # "Bits 0 (italic), 5 (bold) and 6 (regular) must not be set here"
-                                value = value & 0b11111100
-                            value = int_to_bitarray(value)
+            for info_tag, (table, field) in ufo_custom_opentype_values.items():
+                if (table, field) in self.font.custom_opentype_values:
+                    value = self.font.custom_opentype_values[(table, field)]
+                    if (table, field) in BITARRAY:
+                        if info_tag == "openTypeOS2Selection":
+                            # "Bits 0 (italic), 5 (bold) and 6 (regular) must not be set here"
+                            value = value & 0b11111100
+                        value = int_to_bitarray(value)
+                    if info_tag == "openTypeHeadCreated":
+                        value = time.strftime(
+                            "%Y/%m/%d %H:%M:%S",
+                            time.gmtime(timeTools.epoch_diff + value),
+                        )
 
-                        setattr(ufo.info, info_tag, value)
+                    setattr(ufo.info, info_tag, value)
         # Guides
         if master.guides:
             ufo.info.guidelines = []
         for guide in master.guides:
             ufo.info.guidelines.append(
                 ufoLib2.objects.Guideline(
                     x=guide.pos[0],
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/fontforge.py` & `babelfont-3.0.5/src/babelfont/convertors/fontforge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import re
+import shlex
 import uuid
 import logging
 from pathlib import Path
 
-from babelfont.BaseObject import OTValue
+from fontTools.misc.timeTools import epoch_diff
+
 from babelfont.convertors import BaseConvertor
+from babelfont.Names import OPENTYPE_NAMES
 
 from babelfont import (
+    Anchor,
     Master,
     Instance,
     Glyph,
     Layer,
     Shape,
     Transform,
 )
@@ -40,189 +44,225 @@
         "PfmFamily",
         "AntiAlias",
         "FitToEm",
         "DisplaySize",
         "Validated",
         "Flags",
         "Lookup",
+        "GlifName",
+        "NameList",
     ]
 
     @classmethod
     def can_save(cls, convertor, **kwargs):
         return False
 
-    def _load(self):
+    def _setupfont(self):
         font = self.font
-        self.current_glyph = None
+        font.upm = 1024
         # I'm going to assume a single master font
         font.masters = [Master(name="Regular", id=str(uuid.uuid4()), font=font)]
         font.instances = [Instance(name="Regular", styleName="Regular", location={})]
 
+    def _load(self):
+        self._setupfont()
+        self.current_glyph = None
         self.info = open(Path(self.filename) / "font.props").read().splitlines()
         self._load_line("info")
         # Probe once for glyphorder
         self.glyph_order = {}
         for fontfile in Path(self.filename).glob("*.glyph"):
-            self._probe_glyphorder(fontfile)
+            self._probe_glyphorder(open(fontfile).readlines())
         for gid in sorted(self.glyph_order.keys()):
             self.font.glyphs.append(Glyph(name=self.glyph_order[gid]))
 
         for fontfile in Path(self.filename).glob("*.glyph"):
             self.info = open(fontfile).read().splitlines()
             self._load_line("glyph")
 
-        return font
+        return self.font
 
-    def _probe_glyphorder(self, file):
+    def _probe_glyphorder(self, lines):
         glyphname = ""
-        for line in open(file).readlines():
+        for line in lines:
             if m := re.match(r"StartChar: (.*)", line):
                 glyphname = m.group(1)
                 continue
             if m := re.match(r"Encoding: (\d+) (-?\d+) (\d+)", line):
                 gid = int(m.group(3))
                 if not glyphname:
-                    raise ValueError(f"Bad file {file} - no StartChar")
+                    raise ValueError(f"Bad file - no StartChar")
                 self.glyph_order[gid] = glyphname
-                break
 
     def _load_line(self, mode):
         while self.info:
             line = self.info.pop(0)
-            if line == "EndSplineFont" and mode == "info":
+            if line == "EndSplineFont":
+                break
+            if line.startswith("BeginChars") and mode == "info":
                 break
             if line == "EndChar" and mode == "glyph":
                 break
+            if not line:
+                continue
             if ": " not in line:
                 if hasattr(self, "_handle_" + line):
                     getattr(self, "_handle_" + line)()
                     continue
                 else:
                     raise ValueError("Bad font.props file - " + line)
             key, value = line.split(": ", 1)
             if key in self.IGNORE:
                 continue
             if hasattr(self, "_handle_" + key):
                 getattr(self, "_handle_" + key)(value)
             else:
-                log.warn("Unknown info key %s", key)
+                log.debug("Unknown info key %s", key)
+                pass
 
     def _handle_FamilyName(self, value):
         self.font.names.familyName.set_default(value)
 
     def _handle_FullName(self, value):
         self.font.names.compatibleFullName.set_default(value)
 
     def _handle_Copyright(self, value):
         self.font.names.copyright.set_default(value)
 
     def _handle_Comments(self, value):
         self.font.notes = value
 
     def _handle_Version(self, value):
-        self.font.names.version.set_default(value)
         self.font.version = [int(x) for x in value.split(".")]
 
     def _handle_Weight(self, value):
         self.font.names.typographicSubfamily.set_default(value)
 
     def _handle_Fontlog(self, value):
         self.font.names.description.set_default(value)
 
     def _handle_ItalicAngle(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("post", "italicAngle", float(value))
-        )
+        self.font.masters[0].metrics["italicAngle"] = float(value)
 
     def _handle_UnderlinePosition(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("post", "underlinePosition", int(value))
-        )
+        self.font.masters[0].metrics["underlinePosition"] = int(value)
 
     def _handle_UnderlineWidth(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("post", "underlineThickness", int(value))
-        )
+        self.font.masters[0].metrics["underlineThickness"] = int(value)
 
     def _handle_OS2TypoAscent(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "sTypoAscender", int(value))
-        )
+        self.font.masters[0].metrics["typoAscender"] = int(value)
 
     def _handle_OS2TypoDescent(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "sTypoDescender", int(value))
-        )
+        self.font.masters[0].metrics["typoDescender"] = int(value)
 
-    def _handle_OS2TypoLineGap(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "sTypoLineGap", int(value))
-        )
+    def _handle_OS2TypoLinegap(self, value):
+        self.font.masters[0].metrics["typoLineGap"] = int(value)
 
     def _handle_OS2WinAscent(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "usWinAscent", int(value))
-        )
+        self.font.masters[0].metrics["winAscent"] = int(value)
 
     def _handle_OS2WinDescent(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "usWinDescent", int(value))
-        )
+        self.font.masters[0].metrics["winDescent"] = int(value)
 
     def _handle_OS2Vendor(self, value):
-        self.font.customOpenTypeValues.append(OTValue("OS/2", "achVendID", value))
+        value = value.replace("'", "")
+        self.font.custom_opentype_values[("OS/2", "achVendID")] = value
 
-    def _handle_hheaAscent(self, value):
-        self.font.customOpenTypeValues.append(OTValue("hhea", "ascent", int(value)))
+    def _handle_HheadAscent(self, value):
+        self.font.masters[0].metrics["hheaAscender"] = int(value)
 
-    def _handle_hheaDescent(self, value):
-        self.font.customOpenTypeValues.append(OTValue("hhea", "descent", int(value)))
+    def _handle_HheadDescent(self, value):
+        self.font.masters[0].metrics["hheaDescender"] = int(value)
 
-    def _handle_OS2TypoLinegap(self, value):
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "sTypoLineGap", int(value))
-        )
+    def _handle_LineGap(self, value):
+        self.font.masters[0].metrics["hheaLineGap"] = int(value)
 
     def _handle_Ascent(self, value):
         self.font.masters[0].metrics["ascender"] = int(value)
 
     def _handle_Descent(self, value):
         self.font.masters[0].metrics["descender"] = -int(value)
 
+    def _handle_OS2SubXSize(self, value):
+        self.font.masters[0].metrics["subscriptXSize"] = int(value)
+
+    def _handle_OS2SubYSize(self, value):
+        self.font.masters[0].metrics["subscriptYSize"] = int(value)
+
+    def _handle_OS2SubXOff(self, value):
+        self.font.masters[0].metrics["subscriptXOffset"] = int(value)
+
+    def _handle_OS2SubYOff(self, value):
+        self.font.masters[0].metrics["subscriptYOffset"] = int(value)
+
+    def _handle_OS2SupXSize(self, value):
+        self.font.masters[0].metrics["superscriptXSize"] = int(value)
+
+    def _handle_OS2SupYSize(self, value):
+        self.font.masters[0].metrics["superscriptYSize"] = int(value)
+
+    def _handle_OS2SupXOff(self, value):
+        self.font.masters[0].metrics["superscriptXOffset"] = int(value)
+
+    def _handle_OS2SupYOff(self, value):
+        self.font.masters[0].metrics["superscriptYOffset"] = int(value)
+
+    def _handle_OS2StrikeYSize(self, value):
+        self.font.masters[0].metrics["strikeoutSize"] = int(value)
+
+    def _handle_OS2StrikeYPos(self, value):
+        self.font.masters[0].metrics["strikeoutPosition"] = int(value)
+
+    def _handle_OS2CapHeight(self, value):
+        self.font.masters[0].metrics["capHeight"] = int(value)
+
+    def _handle_OS2XHeight(self, value):
+        self.font.masters[0].metrics["xHeight"] = int(value)
+
+    def _handle_HheadAscent(self, value):
+        self.font.masters[0].metrics["hheaAscender"] = int(value)
+
     def _handle_LayerCount(self, value):
         # Ignore layers for now
         pass
 
     def _handle_Layer(self, value):
         # Ignore layers for now
         pass
 
     def _handle_FSType(self, value):
-        self.font.customOpenTypeValues.append(OTValue("OS/2", "fsType", int(value)))
+        self.font.custom_opentype_values[("OS/2", "fsType")] = int(value)
 
     def _handle_OS2_WeightWidthSlopeOnly(self, value):
-        # XXX
-        self.font.customOpenTypeValues.append(
-            OTValue("OS/2", "fsSelection", int(value))
-        )
+        pass
+
+    def _handle_TTFWeight(self, value):
+        self.font.custom_opentype_values[("OS/2", "usWeightClass")] = int(value)
+
+    def _handle_TTFWidth(self, value):
+        self.font.custom_opentype_values[("OS/2", "usWidthClass")] = int(value)
+
+    def _handle_Panose(self, value):
+        bits = [int(v) for v in value.split()]
+        self.font.custom_opentype_values[("OS/2", "bPanose")] = bits
 
     def _handle_OS2_UseTypoMetrics(self, value):
         if not value:
             return
-        for otval in self.font.customOpenTypeValues:
-            if otval.table == "OS/2" and otval.field == "fsSelection":
-                otval.value = otval.value | 7 << 1
-                return
-        self.font.customOpenTypeValues.append(OTValue("OS/2", "fsSelection", 7))
+        if ("OS/2", "fsSelection") in self.font.custom_opentype_values:
+            self.font.custom_opentype_values[("OS/2", "fsSelection")] |= 1 << 7
+        else:
+            self.font.custom_opentype_values[("OS/2", "fsSelection")] = 1 << 7
 
     def _handle_CreationTime(self, value):
-        self.font.customOpenTypeValues.append(OTValue("head", "created", int(value)))
+        self.font.custom_opentype_values[("head", "created")] = int(value) - epoch_diff
 
     def _handle_ModificationTime(self, value):
-        self.font.customOpenTypeValues.append(OTValue("head", "modified", int(value)))
+        self.font.custom_opentype_values[("head", "modified")] = int(value) - epoch_diff
 
     def _handle_ShortTable(self, value):
         # Ignore short table for now
         while self.info:
             line = self.info.pop(0)
             if line.startswith("EndShort"):
                 break
@@ -258,26 +298,53 @@
     def _handle_Encoding(self, value):
         if not self.current_glyph:
             return
         _old, unicode, gid = value.split()
         if unicode != "-1":
             self.current_glyph.codepoints.append(int(unicode))
 
+    def _handle_AltUni2(self, value):
+        for alternate in value.split():
+            codepoint, vs, _reserved = alternate.split(".")
+            if vs != "ffffffff":
+                log.warning(
+                    "Alternate codepoint with variation selector not current supported in %s",
+                    self.current_glyph.name,
+                )
+            self.current_glyph.codepoints.append(int(codepoint, 16))
+
     def _handle_Width(self, value):
         self.current_glyph.layers[0].width = int(value)
 
     def _handle_VWidth(self, value):
         self.current_glyph.layers[0].height = int(value)
 
     def _handle_GlyphClass(self, value):
         pass
 
+    def _handle_Back(self):
+        background = Layer(
+            name="background",
+            id=str(uuid.uuid1()),
+            _master=self.font.masters[0].id,
+            _font=self.font,
+            _glyph=self.current_glyph,
+            isBackground=True,
+            width=0,
+        )
+        # self.current_glyph.layers[0].background = background.id
+        # self.current_glyph.layers.append(background)
+        self._expect_splineset(background.getPen())
+
     def _handle_Fore(self):
         self._expect_splineset(self.current_glyph.layers[0].getPen())
 
+    def _handle_EndChars(self):
+        pass
+
     def _handle_Refer(self, value: str):
         gid, unicode, style, xx, xy, yx, yy, dx, dy, ttflag = value.split(None, 10)
         component = Shape(
             ref=self.glyph_order[int(gid)],
             transform=Transform(
                 float(xx), float(xy), float(yx), float(yy), float(dx), float(dy)
             ),
@@ -319,7 +386,50 @@
             else:
                 # Put back
                 self.info.insert(0, line)
                 break
         if paths:
             pen.closePath()
         return
+
+    def _handle_AnchorPoint(self, value: str):
+        name, x, y, typ, ligcomp = value.split()
+        name = name.replace('"', "")
+        if typ == "ligature":
+            name += "_%s" % ligcomp
+        if typ == "mark":
+            name = "_" + name
+        self.current_glyph.layers[0].anchors.append(
+            Anchor(
+                name=name,
+                x=float(x),
+                y=float(y),
+                _={"type": typ},
+            )
+        )
+
+    def _handle_LangName(self, value: str):
+        names = shlex.split(value)
+        lang = names.pop(0)
+        for nameid, name in enumerate(names):
+            if name == "":
+                continue
+            field = OPENTYPE_NAMES[nameid]
+            getattr(self.font.names, field).set_default(name)
+
+
+class FontForgeSFD(FontForgeSFDIR):
+    suffix = ".sfd"
+
+    def _load(self):
+        self._setupfont()
+        self.current_glyph = None
+
+        self.info = open(Path(self.filename)).read().splitlines()
+        self.glyph_order = {}
+        self._probe_glyphorder(self.info)
+        for gid in sorted(self.glyph_order.keys()):
+            self.font.glyphs.append(Glyph(name=self.glyph_order[gid]))
+        self._load_line("info")
+        while self.info:
+            self._load_line("glyph")
+        return self.font
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/fontlab/vfj.py` & `babelfont-3.0.5/src/babelfont/convertors/fontlab/vfj.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import math
 
 import orjson
 from fontTools.misc.transform import Transform
 
 from babelfont import Axis, Glyph, Layer, Master, Node, Shape, Guide
-from babelfont.BaseObject import Color, I18NDictionary, OTValue
+from babelfont.BaseObject import Color, I18NDictionary
 from babelfont.convertors import BaseConvertor
 
 
 class FontlabVFJ(BaseConvertor):
     suffix = ".vfj"
 
     def _load(self):
@@ -294,24 +294,22 @@
             "manufacturer",
             "manufacturerURL",
             "version",
         ]:
             setattr(self.font.names, tag, I18NDictionary.with_default(info.get(tag)))
         self.font.version = (info.get("versionMajor"), info.get("versionMinor"))
         if "vendor" in info:
-            self.font.customOpenTypeValues.append(
-                OTValue("OS/2", "achVendID", info["vendor"])
-            )
+            self.font.custom_opentype_values[("OS/2", "achVendID")] = info["vendor"]
         # Fontlab date format = "2020/08/28 15:33:36"
         if "date" in info:
             self.font.date = datetime.datetime.strptime(
                 info["creationDate"],
                 "%Y/%m/%d %H:%M:%S",
             )
         if "useTypoMetrics" in info:
-            self.font.customOpenTypeValues.append(OTValue("OS/2", "fsSelection", 0x7))
+            self.font.custom_opentype_values[("OS/2", "fsSelection")] = 0x7
         if "embedding" in info:
-            self.font.customOpenTypeValues.append(
-                OTValue("OS/2", "fsType", int(info["embedding"], 16))
+            self.font.custom_opentype_values[("OS/2", "fsType")] = int(
+                info["embedding"], 16
             )
         # codepageRange
         # unicodeRange
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphs2.py` & `babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphs2.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,22 @@
     Instance,
     Layer,
     Master,
     Node,
     Shape,
     Transform,
 )
-from babelfont.BaseObject import OTValue
-from babelfont.convertors import BaseConvertor
+from babelfont.convertors.glyphs.glyphs3 import GlyphsThree
 from babelfont.convertors.glyphs.utils import (
     _glyphs_metrics_to_ours,
     _stash,
 )
 
 
-class Glyphs2(BaseConvertor):
+class Glyphs2(GlyphsThree):
     suffix = ".glyphs"
 
     @classmethod
     def is_suitable_plist(cls, convertor):
         return (
             ".formatVersion" not in convertor.scratch["plist"]
             or convertor.scratch["plist"][".formatVersion"] < 3
@@ -76,15 +75,17 @@
 
         for ginstance in self.glyphs.get("instances", []):
             self.font.instances.append(self._load_instance(ginstance))
 
         self._fixup_axis_mappings()
 
         self._load_metadata()
-        self._load_features()
+        _stash(self.font, self.glyphs)
+
+        self.interpret_features()
         return self.font
 
     def _load_axes(self):
         self.axis_name_map = {}
         if "Axes" in self.customParameters:
             for ax in self.customParameters["Axes"]:
                 self.font.axes.append(Axis(name=ax["Name"], tag=ax["Tag"]))
@@ -264,15 +265,15 @@
         for shape in layer.get("components", []):
             l.shapes.append(self._load_component(shape))
         for anchor in layer.get("anchors", []):
             l.anchors.append(self._load_anchor(anchor))
 
         returns = [l]
         if "background" in layer:
-            (background,) = self._load_layer(layer["background"], width=l.width)
+            (background,) = self._load_layer(layer["background"], glyph, width=l.width)
             # If it doesn't have an ID, we need to generate one
             background.id = background.id or str(uuid.uuid1())
             background.isBackground = True
 
             l.background = background.id
             returns.append(background)
         # TODO backgroundImage, metricTop/Bottom/etc, vertOrigin, vertWidth.
@@ -320,29 +321,29 @@
             ax.map.append(
                 (
                     int(loc["Location"]),
                     instance_location[ax.tag],
                 )
             )
 
-        _maybesetformatspecific(i, ginstance, "customParameters")
+        _stash(i, ginstance, ["customParameters"])
         return i
 
     def _load_path(self, path):
         shape = Shape()
         shape.nodes = []
         for n in path["nodes"]:
             m = re.match(r"(\S+) (\S+) (\S+)( SMOOTH)?(.*)", n)
             ntype = m[3][0].lower()
             if m[4]:
                 ntype = ntype + "s"
             n = Node(x=float(m[1]), y=float(m[2]), type=ntype)
             shape.nodes.append(n)
         shape.closed = bool(path["closed"])
-        _maybesetformatspecific(shape, path, "attr")
+        _stash(shape, path, ["attr"])
         return shape
 
     def _load_component(self, shape):
         glyphname = shape.get("ref", shape.get("name"))
         transform = shape.get("transform")
         if isinstance(transform, str):
             m = re.match(r"^\{(\S+), (\S+), (\S+), (\S+), (\S+), (\S+)\}", transform)
@@ -353,24 +354,27 @@
             translate = Transform().translate(*shape.get("pos", (0, 0)))
             scale = Transform().scale(*shape.get("scale", (1, 1)))
             rotation = Transform().rotate(math.radians(shape.get("angle", 0)))
             # Compute transform...
             transform = translate.transform(scale).transform(rotation)
 
         c.transform = transform
-        for entry in [
-            "alignment",
-            "anchorTo",
-            "attr",
-            "locked",
-            "orientation",
-            "piece",
-            "userData",
-        ]:
-            _maybesetformatspecific(c, shape, entry)
+        _stash(
+            c,
+            shape,
+            [
+                "alignment",
+                "anchorTo",
+                "attr",
+                "locked",
+                "orientation",
+                "piece",
+                "userData",
+            ],
+        )
         return c
 
     def _load_kern_groups(self, glyphs):
         kerngroups = {}
         for g in glyphs:
             l_class = g.get("leftKerningGroup", g["glyphname"])
             r_class = g.get("rightKerningGroup", g["glyphname"])
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphs3.py` & `babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphs3.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     custom_parameter_metrics,
 )
 from babelfont.Master import CORE_METRICS
 
 
 class GlyphsThree(BaseConvertor):
     suffix = ".glyphs"
+    LOAD_FILTERS = ["glyphData"]
 
     @classmethod
     def is_suitable_plist(cls, convertor):
         return (
             ".formatVersion" in convertor.scratch["plist"]
             and convertor.scratch["plist"][".formatVersion"] >= 3
         )
@@ -101,15 +102,16 @@
             axis.default = axis.designspace_to_userspace(axis.default)
             axis.min = axis.designspace_to_userspace(axis.min)
             axis.max = axis.designspace_to_userspace(axis.max)
 
         self.interpret_linked_kerning()
         assert self.font.default_master
         self.interpret_kern_groups()
-        self.interpret_metric_custom_parameters()
+        self.interpret_master_custom_parameters()
+        self.interpret_font_custom_parameters()
         self.interpret_features()
         return font
 
     def load_metadata(self):
         glyphs = self.scratch["plist"]
         self.font.upm = glyphs.pop("unitsPerEm")
         self.font.version = (glyphs.pop("versionMajor"), glyphs.pop("versionMinor"))
@@ -122,24 +124,34 @@
                 props[prop["key"]] = prop["value"]
             else:
                 props[prop["key"]] = {p["language"]: p["value"] for p in prop["values"]}
 
         if props:
             interestingProps = {
                 "copyrights": "copyright",
-                "designer": "designer",
+                "designers": "designer",
                 "designerURL": "designerURL",
+                "trademarks": "trademark",
+                "descriptions": "description",
+                "licenses": "license",
+                "licenseURL": "licenseURL",
+                "manufacturers": "manufacturer",
+                "manufacturerURL": "manufacturerURL",
             }  # Etc
             for glyphsname, attrname in interestingProps.items():
                 thing = props.get(glyphsname, "")
                 if isinstance(thing, dict):
                     getattr(self.font.names, attrname).copy_in(thing)
                 else:
                     getattr(self.font.names, attrname).set_default(thing)
             # Do other properties here
+            if "vendorID" in props:
+                self.font.custom_opentype_values[("OS/2", "achVendID")] = props[
+                    "vendorID"
+                ]
 
         self.font.note = glyphs.pop("note", "")
         self.font.date = datetime.datetime.strptime(
             glyphs.pop("date"), "%Y-%m-%d %H:%M:%S +0000"
         )
 
     def load_axis(self, gaxis):
@@ -308,16 +320,16 @@
         _stash(shape, path)
         if len(shape.nodes):
             # Bring it to front
             shape.nodes = shape.nodes[-1:] + shape.nodes[:-1]
         return shape
 
     def get_codepoint(self, gglyph):
-        cp = gglyph.get("unicode")
-        if cp and not isinstance(cp, list):
+        cp = gglyph.get("unicode", None)
+        if cp is not None and not isinstance(cp, list):
             cp = [cp]
         if cp:
             return [int(x) for x in cp]
 
     def interpret_kern_groups(self):
         for g in self.font.glyphs:
             left_group = _g(g, "kernLeft", pop=True)
@@ -354,14 +366,18 @@
             for right, value in level2.items()
         }
 
     def interpret_metrics(self):
         metrics = _g(self.font, "metrics", [])  # Keep stashed
         metric_types = [_metrics_dict_to_name(k) for k in metrics]
         for master in self.font.masters:
+            # Glyphs has these values as defaults:
+            master.metrics["underlinePosition"] = -100
+            master.metrics["underlineThickness"] = 50
+
             metric_values = _g(master, "metricValues", [], pop=True)
             master.metrics["italicAngle"] = 0
             for k, v in zip(metric_types, metric_values):
                 pos = v.get("pos", 0)
                 master.metrics[k] = pos
                 if v.get("over"):
                     master.metrics["%s overshoot" % _glyphs_metrics_to_ours(k)] = v[
@@ -395,42 +411,79 @@
                 ax = axes_by_tag[axistag]
                 ax.map = []
                 for designspace, userspace in axismap.items():
                     ax.map.append((userspace, float(designspace)))
             return
 
         for instance in self.font.instances:
+            # instance.location is in designspace
+            # The Axis Location custom parameter is in userspace, use
+            # this to make the map
             c = (
                 _custom_parameter(
                     instance._formatspecific.get("com.glyphsapp", {}), "Axis Location"
                 )
                 or []
             )
+            # If there isn't an Axis Location, use the weightclass and widthclass
+            if not c:
+                weightclass = instance._formatspecific.get("com.glyphsapp", {}).get(
+                    "weightClass", 400
+                )
+                if weightclass is not None:
+                    c.append({"Axis": "Weight", "Location": weightclass})
+                widthclass = instance._formatspecific.get("com.glyphsapp", {}).get(
+                    "widthClass", 5
+                )
+                if widthclass is not None:
+                    c.append({"Axis": "Width", "Location": widthclass})
             for loc in c:
-                ax = axes_by_name[loc["Axis"]]
+                ax = axes_by_name.get(loc["Axis"])
+                if not ax:
+                    # Maybe we don't have a weight or width but we don't have
+                    # an axis location either so we synthesised those locations
+                    continue
                 if not ax.map:
                     ax.map = []
                 ax.map.append(
                     (
+                        int(loc["Location"]),  # The instances location in user space
                         instance.location[ax.tag],
-                        int(loc["Location"]),
                     )
                 )
 
-    def interpret_metric_custom_parameters(self):
+    def interpret_master_custom_parameters(self):
         for master in self.font.masters:
             cps = _g(master, "customParameters", [])
             new_cps = []
             for param in cps:
                 if param["name"] in CORE_METRICS:
                     master.metrics[param["name"]] = param["value"]
                 else:
                     new_cps.append(param)
             _stash(master, {"customParameters": new_cps})
 
+    def interpret_font_custom_parameters(self):
+        cps = _g(self.font, "customParameters", [])
+        new_cps = []
+        for param in cps:
+            if param["name"] == "panose":
+                self.font.custom_opentype_values[("OS/2", "panose")] = param["value"]
+            # elif param["name"] == "fsType":
+            #     self.font.custom_opentype_values[("OS/2", "fsType")] = int(
+            #         param["value"]
+            #     )
+            elif param["name"] == "fsSelection":
+                self.font.custom_opentype_values[("OS/2", "fsSelection")] = int(
+                    param["value"]
+                )
+            else:
+                new_cps.append(param)
+        _stash(self.font, {"customParameters": new_cps})
+
     def interpret_features(self):
         self.font.features = Features()
 
         def code_with_notes(feature):
             code = feature["code"]
             if "disabled" in feature:
                 code = "# Disabled\n# " + code.replace("\n", "\n# ")
@@ -443,17 +496,16 @@
 
         for glyphclass in _g(self.font, "classes", [], pop=True):
             # Beware of tokens XXX
             self.font.features.classes[glyphclass["name"]] = glyphclass["code"].split()
         for prefix in _g(self.font, "featurePrefixes", [], pop=True):
             self.font.features.prefixes[prefix["name"]] = code_with_notes(prefix)
         for feature in _g(self.font, "features", [], pop=True):
-            self.font.features.features.append(
-                (feature["tag"], code_with_notes(feature))
-            )
+            tag = feature.get("tag", feature.get("name"))
+            self.font.features.features.append((tag, code_with_notes(feature)))
 
     def _save(self):
         font = self.font
         out = _moveformatspecific(font)
         self.glyphs = out
         out["versionMajor"], out["versionMinor"] = font.version
         out[".formatVersion"] = 3
@@ -597,16 +649,18 @@
             glayer["shapes"] = [self.save_shape(s) for s in layer.shapes]
         if layer._master and layer._master != layer.id:
             glayer["associatedMasterId"] = layer._master
         if layer.anchors:
             glayer["anchors"] = [self.save_anchor(a) for a in layer.anchors]
         if layer.background:
             glayer["background"] = self.save_layer(layer._background_layer())
-            del glayer["background"]["width"]
-            del glayer["background"]["layerId"]
+            if "width" in glayer["background"]:
+                del glayer["background"]["width"]
+            if "layerId" in glayer["background"]:
+                del glayer["background"]["layerId"]
         return glayer
 
     def save_shape(self, shape):
         gshape = _moveformatspecific(shape)
         if shape.is_path:
             gshape["closed"] = shape.closed
             outputnodes = []
@@ -671,16 +725,15 @@
             )
         if not props:
             del out["properties"]
 
     def save_custom_parameters(self, out):
         if "customParameters" not in out:
             out["customParameters"] = []
-        for otvalue in self.font.customOpenTypeValues:
-            table, field, value = otvalue.table, otvalue.field, otvalue.value
+        for (table, field), value in self.font.custom_opentype_values.items():
             if table == "OS/2" and field == "fsType":
                 out["customParameters"].append(
                     {"name": "fsType", "value": to_bitfield(int(value))}
                 )
             if table == "OS/2" and field == "fsSelection":
                 if value & 0x7:
                     out["customParameters"].append(
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/glyphs/glyphspackage.py` & `babelfont-3.0.5/src/babelfont/convertors/glyphs/glyphspackage.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/convertors/glyphs/utils.py` & `babelfont-3.0.5/src/babelfont/convertors/glyphs/utils.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/convertors/gsobject.py` & `babelfont-3.0.5/src/babelfont/convertors/gsobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     Master,
     Glyph,
     Layer,
     Guide,
     Anchor,
     Shape,
     Node,
-    OTValue,
     Axis,
     Instance,
 )
 import uuid
 from glyphsLib.glyphdata import get_glyph
 
 
@@ -119,17 +118,17 @@
         location = gmaster.axes
         metrics = self.gsfont.metrics()
         master = Master(name=gmaster.name, id=gmaster.id, font=self.font)
         metric_types = [m.name or m.typeName() for m in metrics]
         for k, v in zip(metric_types, gmaster.metrics()):
             master.metrics[_glyphs_metrics_to_ours(k)] = v.position
             if v.overshoot:
-                master.metrics[
-                    "%s overshoot" % _glyphs_metrics_to_ours(k)
-                ] = v.overshoot
+                master.metrics["%s overshoot" % _glyphs_metrics_to_ours(k)] = (
+                    v.overshoot
+                )
 
         master.location = {k.tag: v for k, v in zip(self.font.axes, location)}
         master.guides = [self._load_guide(x) for x in gmaster.guides]
         kerntable = self.gsfont.kerning.get(master.id, {})
         master.kerning = self._load_kerning(kerntable)
         # XXX support RTL kerning etc.
 
@@ -319,17 +318,15 @@
         cp = self.font.default_master._formatspecific.get("com.glyphsapp", {}).get(
             "customParameters", {}
         )
         for param in cp:
             ot_param = opentype_custom_parameters.get(param.name)
             if not ot_param:
                 continue
-            self.font.customOpenTypeValues.append(
-                OTValue(ot_param[0], ot_param[1], param.value)
-            )
+            self.font.custom_opentype_values[ot_param] = param.value
 
         self.font.note = self.gsfont.note
         self.font.date = self.gsfont.date
 
         _maybesetformatspecific(self.font, self.gsfont, ".appVersion")
         _maybesetformatspecific(self.font, self.gsfont, ".formatVersion")
         _maybesetformatspecific(self.font, self.gsfont, "DisplayStrings")
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/nfsf.py` & `babelfont-3.0.5/src/babelfont/convertors/nfsf.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/convertors/truetype.py` & `babelfont-3.0.5/src/babelfont/convertors/truetype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import uuid
 from datetime import datetime
 from itertools import chain
+from typing import Dict
 
 from fontFeatures import Attachment
 from fontFeatures.ttLib import unparse
-from fontTools.cu2qu.ufo import glyphs_to_quadratic
 from fontTools.fontBuilder import FontBuilder
 from fontTools.misc.fixedTools import otRound
 from fontTools.misc.timeTools import epoch_diff, timestampSinceEpoch
 from fontTools.pens.recordingPen import RecordingPen
 from fontTools.pens.ttGlyphPen import TTGlyphPen
 from fontTools.ttLib import TTFont
 from fontTools.ttLib.tables._g_l_y_f import GlyphCoordinates
+from fontTools.ttLib.tables.O_S_2f_2 import Panose
 from fontTools.ttLib.tables.TupleVariation import TupleVariation
+from fontTools.ttLib.ttGlyphSet import _TTGlyph
 from fontTools.varLib.iup import iup_delta_optimize
 
+from babelfont import (
+    Anchor,
+    Axis,
+    Features,
+    Glyph,
+    Instance,
+    Layer,
+    Master,
+    Node,
+    Shape,
+)
 from babelfont.convertors import BaseConvertor
 from babelfont.fontFilters.featureWriters import build_all_features
-from babelfont import Master, Glyph, Layer, Anchor, Shape, Node, Axis, Instance
 
 
 def _categorize_glyph(font, glyphname):
     if "GDEF" not in font:
         return None
     if not font["GDEF"].table.GlyphClassDef:
         return None
@@ -34,14 +46,29 @@
         return "ligature"
     if classdefs[glyphname] == 3:
         return "mark"
     if classdefs[glyphname] == 4:
         return "component"
 
 
+def compile_panose(data):
+    panose = Panose()
+    panose.bFamilyType = data[0]
+    panose.bSerifStyle = data[1]
+    panose.bWeight = data[2]
+    panose.bProportion = data[3]
+    panose.bContrast = data[4]
+    panose.bStrokeVariation = data[5]
+    panose.bArmStyle = data[6]
+    panose.bLetterForm = data[7]
+    panose.bMidline = data[8]
+    panose.bXHeight = data[9]
+    return panose
+
+
 class TrueType(BaseConvertor):
     suffix = ".ttf"
 
     def _decompose_mixed_layer(self, layer, exportable):
         if (layer.paths and layer.components) or any(
             c.ref not in exportable for c in layer.components
         ):
@@ -147,190 +174,115 @@
         layer = Layer(width=width, id=str(uuid.uuid1()))
         layer._master = self.font.masters[0].id
         layer._font = self.font
         layer._glyph = glyph
         ttglyph.draw(layer.getPen())
         return [layer]
 
-    def _load_contour(self, ttglyph, index):
-        shape = Shape()
-        shape.nodes = []
-        endPt = ttglyph.endPtsOfContours[index]
-        if index > 0:
-            startPt = ttglyph.endPtsOfContours[index - 1] + 1
-        else:
-            startPt = 0
-        points = []
-        for j in range(startPt, endPt + 1):
-            coords = (ttglyph.coordinates[j][0], ttglyph.coordinates[j][1])
-            flags = ttglyph.flags[j] == 1
-            t = "o"
-            if flags == 1:
-                if (j == startPt and ttglyph.flags[endPt] == 1) or (
-                    j != startPt and points[-1].type != "o"
-                ):
-                    t = "l"
-                else:
-                    t = "q"
-            else:
-                if len(points) > 1 and points[-1].type == "o":
-                    # Double offcurve. Insert implicit oncurve.
-                    prevpoint = points[-1]
-                    intermediate = Node(
-                        x=(coords[0] + prevpoint.x) / 2,
-                        y=(coords[1] + prevpoint.y) / 2,
-                        type="q",
-                    )
-                    points.append(intermediate)
-            p = Node(x=coords[0], y=coords[1], type=t)
-            points.append(p)
-        shape.nodes = points
-        return shape
-
-    def _load_component(self, c):
-        baseGlyph, transformation = c.getComponentInfo()
-        component = Shape(ref=baseGlyph, transform=transformation)
-        return component
+    SAVE_FILTERS = [
+        "renameGlyphs:production=True",
+        "decomposeMixedGlyphs",
+        "dropUnexportedGlyphs",
+        "zeroMarkWidths",
+        "cubicToQuadratic",
+        "fillOpentypeValues",
+    ]
 
     def _save(self):
         f = self.font
         fb = FontBuilder(f.upm, isTTF=True)
+        fb.setupGlyphOrder(list(f.glyphs.keys()))
+        fb.setupCharacterMap(f.unicode_map)
 
         metrics = {}
-        all_outlines = {}
-
-        # Find all exportable glyphs
-        exportable = [k for k, v in f.glyphs.items() if v.exported]
-
-        fb.setupGlyphOrder(exportable)
-        fb.setupCharacterMap(
-            {k: v for k, v in f.unicode_map.items() if v in exportable}
-        )
-
-        for g in exportable:
-            all_outlines[g] = []
+        for g in f.glyphs.keys():
             layer = f.default_master.get_glyph_layer(g)
-            metrics[g] = (layer.width, layer.lsb)
+            metrics[g] = (layer.width or 0, layer.lsb or 0)
 
         fb.setupHorizontalMetrics(metrics)
 
-        for m in f.masters:
-            glyf = {}
-            m.ttglyphset = {}
+        ttglyphsets: Dict[str, Dict[str, _TTGlyph]] = {m.id: {} for m in f.masters}
+        # We need to do this in order of single components first
+        done = set()
 
-        done = {}
-
-        def do_a_glyph(g):
+        def convert_glyph(g):
             if g in done:
                 return
-            layer = f.default_master.get_glyph_layer(g)
-            self._decompose_mixed_layer(layer, exportable)
-            for c in layer.components:
-                do_a_glyph(c.ref)
-
             for m in f.masters:
                 layer = m.get_glyph_layer(g)
-                self._decompose_mixed_layer(layer, exportable)
-                all_outlines[g].append(layer)
-            try:
-                glyphs_to_quadratic(all_outlines[g], reverse_direction=True)
-                for ix, m in enumerate(f.masters):
-                    layer = m.get_glyph_layer(g)
-                    pen = TTGlyphPen(m.ttglyphset)
+                if layer:
+                    for c in layer.components:
+                        convert_glyph(c.ref)
+                    pen = TTGlyphPen(ttglyphsets[m.id])
                     layer.draw(pen)
 
-                    m.ttglyphset[g] = pen.glyph()
+                    ttglyphsets[m.id][g] = pen.glyph()
+            done.add(g)
 
-            except Exception:
-                print(
-                    "Problem converting glyph %s to quadratic. (Probably incompatible) "
-                    % g
-                )
-                for m in f.masters:
-                    m.ttglyphset[g] = TTGlyphPen(m.ttglyphset).glyph()
-            done[g] = True
-
-        for g in exportable:
-            do_a_glyph(g)
-
-        fb.updateHead(
-            fontRevision=f.version[0] + f.version[1] / 10 ** len(str(f.version[1])),
-            created=timestampSinceEpoch(f.date.timestamp()),
-            lowestRecPPEM=10,
-        )
-        fb.setupGlyf(f.default_master.ttglyphset)
-        fb.setupHorizontalHeader(
-            ascent=int(f.default_master.ascender),
-            descent=int(f.default_master.descender),
-        )
+        for g in f.glyphs.keys():
+            convert_glyph(g)
 
+        try:
+            fb.setupGlyf(ttglyphsets[f.default_master.id])
+        except ValueError:
+            fb.font["head"].glyphDataFormat = 1
+            self.logger.warning(
+                "Using Boring Expansion, eh? Setting glyf data format to 1"
+            )
+            fb.setupGlyf(ttglyphsets[f.default_master.id])
+        fb.setupHorizontalHeader()
         f.names.typographicSubfamily = f.default_master.name
         f.names.typographicFamily = f.names.familyName
-        fb.setupNameTable(f.names.as_nametable_dict())
-
-        fb.setupOS2(
-            sTypoAscender=int(f.default_master.ascender),
-            sTypoDescender=int(f.default_master.descender),
-            sCapHeight=int(f.default_master.capHeight),
-            sxHeight=int(f.default_master.xHeight),
-        )
+        fb.setupNameTable(f.names.as_nametable_dict(), mac=False)
+        fb.setupOS2()
 
         if f.axes:
             model = f.variation_model()
             axis_map = {}
             variations = {}
-            for g in exportable:
-                variations[g] = self.calculate_a_gvar(f, model, g, metrics[g][0])
+            self.logger.info("Calculating gvar table")
+            for g in f.glyphs.keys():
+                variations[g] = self.calculate_a_gvar(f, model, g, ttglyphsets)
 
             for ax in f.axes:
                 ax.name = ax.name.as_fonttools_dict
                 axis_map[ax.tag] = ax
             for instance in f.instances:
                 instance.location = {
                     k: axis_map[k].map_backward(v) for k, v in instance.location.items()
                 }
             fb.setupFvar(f.axes, f.instances)
 
             fb.setupGvar(variations)
             fb.setupAvar(f.axes)
-        # Move glyph categories to fontfeatures
-        # if f.features:
-        #     for g in f.glyphs.values():
-        #         if g.exported:
-        #             f.features.classes[g.name] = g.category
-
-        #     build_all_features(f, fb.font)
+        build_all_features(f, fb.font)
         fb.setupPost()
-
-        for otvalue in f.customOpenTypeValues:
-            table, field, value = otvalue.table, otvalue.field, otvalue.value
+        # Set OS/2 version to 4 for ufo2ft compatibility
+        fb.font["OS/2"].version = 4
+        fb.font["maxp"].maxZones = 1
+
+        for (table, field), value in f.custom_opentype_values.items():
+            if field == "panose":
+                value = compile_panose(value)
             setattr(fb.font[table], field, value)
-
+            self.logger.debug("Setting %s.%s to %s", table, field, value)
         fb.font.save(self.filename)
 
-        # Rename to production
-        rename_map = {g.name: g.production_name or g.name for g in f.glyphs}
-        if rename_map:
-            font = TTFont(self.filename)
-            font.setGlyphOrder([rename_map.get(n, n) for n in font.getGlyphOrder()])
-            if "post" in font and font["post"].formatType == 2.0:
-                font["post"].extraNames = []
-                font["post"].compile(font)
-            font.save(self.filename)
-
-    def calculate_a_gvar(self, f, model, g, default_width):
-        master_layer = f.default_master.get_glyph_layer(g)
-        if g not in f.default_master.ttglyphset:
+    def calculate_a_gvar(
+        self, f, model, g, ttglyphsets: Dict[str, Dict[str, _TTGlyph]]
+    ):
+        if g not in ttglyphsets[f.default_master.id]:
             return None
-        default_g = f.default_master.ttglyphset[g]
+        default_g = ttglyphsets[f.default_master.id][g]
         all_coords = []
         for m in f.masters:
             layer = m.get_glyph_layer(g)
-            basecoords = GlyphCoordinates(m.ttglyphset[g].coordinates)
-            if m.ttglyphset[g].isComposite():
+            masterglyph = ttglyphsets[m.id][g]
+            basecoords = GlyphCoordinates(masterglyph.coordinates)
+            if masterglyph.isComposite():
                 component_point = GlyphCoordinates(
                     [
                         (otRound(layer_comp.pos[0]), otRound(layer_comp.pos[1]))
                         for layer_comp in layer.components
                     ]
                 )
                 basecoords.extend(component_point)
@@ -363,24 +315,33 @@
             )
             if None in delta_opt:
                 var = TupleVariation(sup, delta_opt)
             gvar_entry.append(var)
         return gvar_entry
 
     def _load_features(self):
-        self.font.features = unparse(self.tt)
+        features = unparse(self.tt)
         # Load anchors
-        for routine in self.font.features.routines:
+        for routine in features.routines:
             for rule in routine.rules:
                 if isinstance(rule, Attachment):
                     for glyphname, pos in rule.bases.items():
                         self._add_anchor(glyphname, pos, rule.base_name)
                     for glyphname, pos in rule.marks.items():
                         self._add_anchor(glyphname, pos, rule.mark_name)
 
+        self.font.features = Features()
+        for feature, routines in features.features.items():
+            self.font.features.features.append(
+                (str(feature), "\n".join(x.asFea() for x in routines))
+            )
+        for routine in features.routines:
+            self.font.features.prefixes[routine.name] = routine.asFea()
+        self.font.features.classes = features.namedClasses
+
     def _add_anchor(self, glyphname, pos, name):
         # Would be nice if this was variable.
         layer = self.font.default_master.get_glyph_layer(glyphname)
         layer.anchors.append(Anchor(name=name, x=pos[0], y=pos[1]))
 
     # import numpy as np
     # def calculate_a_gvar(self, f, model, g, default_width):
@@ -408,18 +369,18 @@
     #         gvar_entry.append(TupleVariation(sup, list(map(tuple, deltaset))))
     #     return gvar_entry
 
 
 class OpenType(TrueType):
     suffix = ".otf"
 
-    def _load_layers(self, g):
+    def _load_layers(self, g, _glyph):
         ttglyph = self.tt.getGlyphSet()[g]
         width = self.tt["hmtx"][g][0]
-        layer = Layer(width=width, id=str(uuid.uuid1()))
+        layer = Layer(width=width, id=self.font.masters[0].id)
         layer._master = self.font.masters[0].id
         layer._font = self.font
         pen = RecordingPen()
         ttglyph.draw(pen)
         contours = pen.value
         lastcontour = []
         startPt = (0, 0)
```

### Comparing `babelfont-3.0.4/src/babelfont/convertors/ufo.py` & `babelfont-3.0.5/src/babelfont/convertors/ufo.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/src/babelfont/fontFilters/anchorPropagation.py` & `babelfont-3.0.5/src/babelfont/fontFilters/anchorPropagation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+import logging
+
 from babelfont.Font import Font
 from babelfont.Layer import Layer
 from babelfont.Anchor import Anchor
 
+logger = logging.getLogger(__name__)
+
+
 def propagate_anchors(font: Font):
+    logger.info("Propagating anchors")
     processed = set()
 
     for glyph in font.glyphs:
         for layer in glyph.layers:
             _propagate_anchors(layer, glyph.name, processed)
 
+
 def _propagate_anchors(layer: Layer, glyphname: str, processed: set):
     if layer.id in processed:
         return
     processed.add(layer.id)
-    
+
     base_components = []
     mark_components = []
     anchor_names = set()
     to_add = {}
     for component in layer.components:
         component_layer = component.component_layer
         if not component_layer:
             continue
         _propagate_anchors(component_layer, component.ref, processed)
         if any(a.name.startswith("_") for a in component_layer.anchors):
             mark_components.append(component)
         else:
             base_components.append(component)
             anchor_names |= {a.name for a in component_layer.anchors}
-    
+
     if mark_components and not base_components and _is_ligature_mark(layer):
         try:
             component = _component_closest_to_origin(mark_components)
         except Exception as e:
             raise ValueError(
                 "Error while determining which component of composite "
                 "'{}' is the lowest: {}".format(glyphname, str(e))
@@ -49,12 +56,12 @@
             _get_anchor_data(to_add, base_components, anchor_name)
 
     for component in mark_components:
         _adjust_anchors(to_add, layer, component)
 
     # we sort propagated anchors to append in a deterministic order
     for name, (x, y) in sorted(to_add.items()):
-        layer.anchors.append( Anchor(name=name, x=x, y=y))
+        layer.anchors.append(Anchor(name=name, x=x, y=y))
 
 
 def _is_ligature_mark(glyph):
     return not glyph.name.startswith("_") and "_" in glyph.name
```

### Comparing `babelfont-3.0.4/src/babelfont.egg-info/PKG-INFO` & `babelfont-3.0.5/src/babelfont.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: babelfont
-Version: 3.0.4
+Version: 3.0.5
 Summary: Load, examine and save fonts in a variety of formats
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 Requires-Dist: orjson>=3.5.1
 Requires-Dist: fonttools>=4.40.0
 Requires-Dist: ufoLib2>=0.11.1
 Requires-Dist: openstep-plist>=0.2.2
-Requires-Dist: glyphsLib>=5.3.2
+Requires-Dist: glyphsLib>=6.7.1
 Requires-Dist: fontfeatures>=1.8.0
+Requires-Dist: vfbLib>=0.6.4
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: defcon; extra == "dev"
 
 # Babelfont: Load, examine and save fonts in a variety of formats
 
 *This describes Babelfont >3.0, which is a complete rewrite from the previous version.*
 
 Babelfont is a utility for loading fonts and examining fonts in a variety
 of formats. It can also be used to *write* fonts in some of these formats,
 making it possible to convert between font formats.
 
 Here are the formats which are currently supported:
 
-| Format         | Read    | Write |
-|----------------|---------|-------|
-| Glyphs 2       | *       | *     |
-| Glyphs 3       | *       | *     |
-| .glyphspackage | *       |       |
-| UFO            | *       |       |
-| Designspace    | *       |       |
-| Fontlab VFJ    | partial |       |
-| TTF            | partial | *     |
-| OTF            | partial |       |
-| Babelfont      | *       | *     |
+| Format          | Read    | Write |
+|-----------------|---------|-------|
+| Glyphs 2        | partial |       |
+| Glyphs 3        | *       | *     |
+| .glyphspackage  | *       |       |
+| UFO             | *       |       |
+| Designspace     | *       |       |
+| Fontlab VFJ     | partial |       |
+| Fontlab VFB     | partial |       |
+| TTF             | partial | *     |
+| OTF             | partial |       |
+| Fontforge SFD   | partial | *     |
+| Fontforge SFDir | partial | *     |
+| Babelfont       | *       | *     |
 
 Babelfont converts all of the above font formats into a intermediary
 set of objects, whose object hierarchy can be seen [here](https://simoncozens.github.io/babelfont). The allows
 the developer to examine any font (single master or variable), without
 needing to worry about the details of each font format.
 
 For example:
```

### Comparing `babelfont-3.0.4/src/babelfont.egg-info/SOURCES.txt` & `babelfont-3.0.5/src/babelfont.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -57,35 +57,46 @@
 src/babelfont/convertors/designspace.py
 src/babelfont/convertors/fontforge.py
 src/babelfont/convertors/gsobject.py
 src/babelfont/convertors/nfsf.py
 src/babelfont/convertors/truetype.py
 src/babelfont/convertors/ufo.py
 src/babelfont/convertors/fontlab/__init__.py
+src/babelfont/convertors/fontlab/vfb.py
 src/babelfont/convertors/fontlab/vfj.py
 src/babelfont/convertors/glyphs/__init__.py
 src/babelfont/convertors/glyphs/glyphs2.py
 src/babelfont/convertors/glyphs/glyphs3.py
 src/babelfont/convertors/glyphs/glyphspackage.py
 src/babelfont/convertors/glyphs/utils.py
+src/babelfont/data/GlyphData.xml
+src/babelfont/data/__init__.py
 src/babelfont/fontFilters/__init__.py
 src/babelfont/fontFilters/anchorPropagation.py
 src/babelfont/fontFilters/background.py
+src/babelfont/fontFilters/cu2qu.py
+src/babelfont/fontFilters/decomposeMixed.py
+src/babelfont/fontFilters/dropUnexported.py
 src/babelfont/fontFilters/featureWriters.py
+src/babelfont/fontFilters/fillOpentype.py
+src/babelfont/fontFilters/glyphDataXML.py
 src/babelfont/fontFilters/marks.py
+src/babelfont/fontFilters/rename.py
 tests/test_dataclasses.py
 tests/test_features.py
 tests/test_glyphs2.py
 tests/test_glyphs3.py
 tests/test_glyphs3_roundtrip.py
 tests/test_interchange.py
 tests/test_otf_loader.py
+tests/test_rename.py
 tests/test_ufo_roundtrip.py
 tests/test_vfj_loader.py
 tests/data/Castoro Roman.vfj
+tests/data/Designspace.glyphs
 tests/data/Glyphs2ManyAxes.glyphs
 tests/data/GlyphsFileFormatv3.glyphs
 tests/data/GlyphsFileFormatv3.vfj
 tests/data/LICENSE_MutatorSans
 tests/data/LICENSE_UbuTestData.txt
 tests/data/NewFont-Regular.ttf
 tests/data/Nunito-Regular.otf
```

### Comparing `babelfont-3.0.4/tests/data/Castoro Roman.vfj` & `babelfont-3.0.5/tests/data/Castoro Roman.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Glyphs2ManyAxes.glyphs` & `babelfont-3.0.5/tests/data/Glyphs2ManyAxes.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/GlyphsFileFormatv3.glyphs` & `babelfont-3.0.5/tests/data/GlyphsFileFormatv3.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/GlyphsFileFormatv3.vfj` & `babelfont-3.0.5/tests/data/GlyphsFileFormatv3.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/LICENSE_MutatorSans` & `babelfont-3.0.5/tests/data/LICENSE_MutatorSans`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/LICENSE_UbuTestData.txt` & `babelfont-3.0.5/tests/data/LICENSE_UbuTestData.txt`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/NewFont-Regular.ttf` & `babelfont-3.0.5/tests/data/NewFont-Regular.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Nunito-Regular.otf` & `babelfont-3.0.5/tests/data/Nunito-Regular.otf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Nunito-Regular.ttf` & `babelfont-3.0.5/tests/data/Nunito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/SimpleTwoAxis.vfj` & `babelfont-3.0.5/tests/data/SimpleTwoAxis.vfj`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/SimpleTwoAxis3.glyphs` & `babelfont-3.0.5/tests/data/SimpleTwoAxis3.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.glyphs` & `babelfont-3.0.5/tests/data/Test1.glyphs`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.ufo/fontinfo.plist` & `babelfont-3.0.5/tests/data/Test1.ufo/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.ufo/glyphs/A_.glif` & `babelfont-3.0.5/tests/data/Test1.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.ufo/glyphs/B_.glif` & `babelfont-3.0.5/tests/data/Test1.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif` & `babelfont-3.0.5/tests/data/Test1.ufo/glyphs/dotaccentcomb.glif`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Test1.ufo/lib.plist` & `babelfont-3.0.5/tests/data/Test1.ufo/lib.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/Ysabeau[wght].ttf` & `babelfont-3.0.5/tests/data/Ysabeau[wght].ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceGenTestItalic.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceGenTestRegular.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestBasic.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestBasic.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestFamilyName.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestFileName.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestFileName.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestInactive.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestInactive.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestInstanceOrder.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/DesignspaceTestTwoAxes.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/fontinfo.plist`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.shoulder.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/_part.stem.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/a.sc.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/dieresis.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph` & `babelfont-3.0.5/tests/data/glyphsLib/GlyphsUnitTestSans.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/TestReencode.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/TestReencode.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace` & `babelfont-3.0.5/tests/data/glyphsLib/master_ufo/GlyphsUnitTestSans.designspace`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf` & `babelfont-3.0.5/tests/data/testotfs/03e3f463c3a985bc42096620cc415342818454fb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf` & `babelfont-3.0.5/tests/data/testotfs/051d92f8bc6ff724511b296c27623f824de256e9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf` & `babelfont-3.0.5/tests/data/testotfs/065b01e54f35f0d849fd43bd5b936212739a50cb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf` & `babelfont-3.0.5/tests/data/testotfs/074a5ae6b19de8f29772fdd5df2d3d833f81f5e6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf` & `babelfont-3.0.5/tests/data/testotfs/07f054357ff8638bac3711b422a1e31180bba863.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf` & `babelfont-3.0.5/tests/data/testotfs/15dfc433a135a658b9f4b1a861b5cdd9658ccbb9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf` & `babelfont-3.0.5/tests/data/testotfs/1735326da89f0818cd8c51a0600e9789812c0f94.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf` & `babelfont-3.0.5/tests/data/testotfs/191826b9643e3f124d865d617ae609db6a2ce203.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf` & `babelfont-3.0.5/tests/data/testotfs/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf` & `babelfont-3.0.5/tests/data/testotfs/1a5face3fcbd929d228235c2f72bbd6f8eb37424.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf` & `babelfont-3.0.5/tests/data/testotfs/1c04a16f32a39c26c851b7fc014d2e8d298ba2b8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf` & `babelfont-3.0.5/tests/data/testotfs/1c2fb74c1b2aa173262734c1f616148f1648cfd6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf` & `babelfont-3.0.5/tests/data/testotfs/1ed7e9064f008f62de6ff0207bb4dd29409597a5.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf` & `babelfont-3.0.5/tests/data/testotfs/21b7fb9c1eeae260473809fbc1fe330f66a507cd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf` & `babelfont-3.0.5/tests/data/testotfs/226bc2deab3846f1a682085f70c67d0421014144.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf` & `babelfont-3.0.5/tests/data/testotfs/24b8d24d00ae86f49791b746da4c9d3f717a51a8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf` & `babelfont-3.0.5/tests/data/testotfs/2681c1c72d6484ed3410417f521b1b819b4e2392.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf` & `babelfont-3.0.5/tests/data/testotfs/270b89df543a7e48e206a2d830c0e10e5265c630.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf` & `babelfont-3.0.5/tests/data/testotfs/28f497629c04ceb15546c9a70e0730125ed6698d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf` & `babelfont-3.0.5/tests/data/testotfs/298c9e1d955f10f6f72c6915c3c6ff9bf9695cec.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf` & `babelfont-3.0.5/tests/data/testotfs/2a670df15b73a5dc75a5cc491bde5ac93c5077dc.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf` & `babelfont-3.0.5/tests/data/testotfs/2c25beb56d9c556622d56b0b5d02b4670c034f89.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf` & `babelfont-3.0.5/tests/data/testotfs/2de1ab4907ab688c0cfc236b0bf51151db38bf2e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf` & `babelfont-3.0.5/tests/data/testotfs/341421e629668b1a1242245d39238ca48432d35d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf` & `babelfont-3.0.5/tests/data/testotfs/3493e92eaded2661cadde752a39f9d58b11f0326.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf` & `babelfont-3.0.5/tests/data/testotfs/37033cc5cf37bb223d7355153016b6ccece93b28.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf` & `babelfont-3.0.5/tests/data/testotfs/373e67bf41ca264e260a9716162b71a23549e885.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf` & `babelfont-3.0.5/tests/data/testotfs/3998336402905b8be8301ef7f47cf7e050cbb1bd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf` & `babelfont-3.0.5/tests/data/testotfs/3c96e7a303c58475a8c750bf4289bbe73784f37d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf` & `babelfont-3.0.5/tests/data/testotfs/3cae6bfe5b57c07ba81ddbd54c02fe4f3a1e3bf6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf` & `babelfont-3.0.5/tests/data/testotfs/3cc01fede4debd4b7794ccb1b16cdb9987ea7571.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf` & `babelfont-3.0.5/tests/data/testotfs/3d0b77a2360aa6faa1385aaa510509ab70dfbeff.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf` & `babelfont-3.0.5/tests/data/testotfs/43ef465752be9af900745f72fe29cb853a1401a5.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf` & `babelfont-3.0.5/tests/data/testotfs/45855bc8d46332b39c4ab9e2ee1a26b1f896da6b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf` & `babelfont-3.0.5/tests/data/testotfs/46669c8860cbfea13562a6ca0d83130ee571137b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf` & `babelfont-3.0.5/tests/data/testotfs/49c9f7485c1392fa09a1b801bc2ffea79275f22e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf` & `babelfont-3.0.5/tests/data/testotfs/4afb0e8b9a86bb9bd73a1247de4e33fbe3c1fd93.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf` & `babelfont-3.0.5/tests/data/testotfs/4cbbc461be066fccc611dcc634af6e8cb2705537.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf` & `babelfont-3.0.5/tests/data/testotfs/4cce528e99f600ed9c25a2b69e32eb94a03b4ae8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf` & `babelfont-3.0.5/tests/data/testotfs/4d4206e30b2dbf1c1ef492a8eae1c9e7829ebad8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf` & `babelfont-3.0.5/tests/data/testotfs/4fac3929fc3332834e93673780ec0fe94342d193.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf` & `babelfont-3.0.5/tests/data/testotfs/5028afb650b1bb718ed2131e872fbcce57828fff.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf` & `babelfont-3.0.5/tests/data/testotfs/53374c7ca3657be37efde7ed02ae34229a56ae1f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf` & `babelfont-3.0.5/tests/data/testotfs/53a91c20e33a596f2be17fb68b382d6b7eb85d5c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf` & `babelfont-3.0.5/tests/data/testotfs/54674a3111d209fb6be0ed31745314b7a8d2c244.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf` & `babelfont-3.0.5/tests/data/testotfs/55c88ebbe938680b08f92c3de20713183e0c7481.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf` & `babelfont-3.0.5/tests/data/testotfs/56cfd0e18d07f41c38e9598545a6d369127fc6f9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf` & `babelfont-3.0.5/tests/data/testotfs/573d3a3177c9a8646e94c8a0d7b224334340946a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf` & `babelfont-3.0.5/tests/data/testotfs/57a9d9f83020155cbb1d2be1f43d82388cbecc88.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf` & `babelfont-3.0.5/tests/data/testotfs/59a585a63b3df608fbeef00956c8c108deec7de6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf` & `babelfont-3.0.5/tests/data/testotfs/5af5361ed4d1e8305780b100e1730cb09132f8d1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf` & `babelfont-3.0.5/tests/data/testotfs/5bb74492f5e0ffa1fbb72e4c881be035120b6513.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf` & `babelfont-3.0.5/tests/data/testotfs/5dfad7735c6a67085f1b90d4d497e32907db4c78.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf` & `babelfont-3.0.5/tests/data/testotfs/604026ae5aaca83c49cd8416909d71ba3e1c1194.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf` & `babelfont-3.0.5/tests/data/testotfs/641ca9d7808b01cafa9a666c13811c9b56eb9c52.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf` & `babelfont-3.0.5/tests/data/testotfs/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf` & `babelfont-3.0.5/tests/data/testotfs/6991b13ce889466be6de3f66e891de2bc0f117ee.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf` & `babelfont-3.0.5/tests/data/testotfs/6ff0fbead4462d9f229167b4e6839eceb8465058.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf` & `babelfont-3.0.5/tests/data/testotfs/706c5d7b625f207bc0d874c67237aad6f1e9cd6f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf` & `babelfont-3.0.5/tests/data/testotfs/738d9f3b8c2dfd03875bf35a61d28fd78faf17c8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf` & `babelfont-3.0.5/tests/data/testotfs/73e84dac2fc6a2d1bc9250d1414353661088937d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf` & `babelfont-3.0.5/tests/data/testotfs/757ebd573617a24aa9dfbf0b885c54875c6fe06b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf` & `babelfont-3.0.5/tests/data/testotfs/7a37dc4d5bf018456aea291cee06daf004c0221c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf` & `babelfont-3.0.5/tests/data/testotfs/7d18685e1529e4ceaad5b6095dfab2f9789e5bce.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf` & `babelfont-3.0.5/tests/data/testotfs/7e14e7883ed152baa158b80e207b66114c823a8b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf` & `babelfont-3.0.5/tests/data/testotfs/8099955657a54e9ee38a6ba1d6f950ce58e3cc25.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf` & `babelfont-3.0.5/tests/data/testotfs/8116e5d8fedfbec74e45dc350d2416d810bed8c4.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf` & `babelfont-3.0.5/tests/data/testotfs/813c2f8e5512187fd982417a7fb4286728e6f4a8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf` & `babelfont-3.0.5/tests/data/testotfs/81c368a33816fb20e9f647e8f24e2180f4720263.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf` & `babelfont-3.0.5/tests/data/testotfs/8228d035fcd65d62ec9728fb34f42c63be93a5d3.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf` & `babelfont-3.0.5/tests/data/testotfs/82f4f3b57bb55344e72e70231380202a52af5805.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf` & `babelfont-3.0.5/tests/data/testotfs/8454d22037f892e76614e1645d066689a0200e61.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf` & `babelfont-3.0.5/tests/data/testotfs/85414f2552b654585b7a8d13dcc3e8fd9f7970a3.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf` & `babelfont-3.0.5/tests/data/testotfs/856ff9562451293cbeff6f396d4e3877c4f0a436.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf` & `babelfont-3.0.5/tests/data/testotfs/85fe0be440c64ac77699e21c2f1bd933a919167e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf` & `babelfont-3.0.5/tests/data/testotfs/86cdd983c4e4c4d7f27dd405d6ceb7d4b9ed3d35.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf` & `babelfont-3.0.5/tests/data/testotfs/87f85d17d26f1fe9ad28d7365101958edaefb967.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf` & `babelfont-3.0.5/tests/data/testotfs/881642af1667ae30a54e58de8be904566d00508f.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf` & `babelfont-3.0.5/tests/data/testotfs/8a9fea2a7384f2116e5b84a9b31f83be7850ce21.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf` & `babelfont-3.0.5/tests/data/testotfs/8d9c4b193808b8bde94389ba7831c1fc6f9e794e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf` & `babelfont-3.0.5/tests/data/testotfs/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf` & `babelfont-3.0.5/tests/data/testotfs/94a5d6fb15a27521fba9ea4aee9cb39b2d03322a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf` & `babelfont-3.0.5/tests/data/testotfs/96490dd2ff81233b335a650e7eb660e0e7b2eeea.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf` & `babelfont-3.0.5/tests/data/testotfs/98b7887cff91f722b92a8ff800120954606354f9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf` & `babelfont-3.0.5/tests/data/testotfs/9fc3e6960b3520e5304033ef5fd540285f72f14d.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/HBTest-VF.ttf` & `babelfont-3.0.5/tests/data/testotfs/HBTest-VF.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/MORXTwentyeight.ttf` & `babelfont-3.0.5/tests/data/testotfs/MORXTwentyeight.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/TRAK.ttf` & `babelfont-3.0.5/tests/data/testotfs/TRAK.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf` & `babelfont-3.0.5/tests/data/testotfs/a014549f766436cf55b2ceb40e462038938ee899.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf` & `babelfont-3.0.5/tests/data/testotfs/a02a7f0ad42c2922cb37ad1358c9df4eb81f1bca.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf` & `babelfont-3.0.5/tests/data/testotfs/a34a7b00f22ffb5fd7eef6933b81c7e71bc2cdfb.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf` & `babelfont-3.0.5/tests/data/testotfs/a6c76d1bafde4a0b1026ebcc932d2e5c6fd02442.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf` & `babelfont-3.0.5/tests/data/testotfs/a706511c65fb278fda87eaf2180ca6684a80f423.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf` & `babelfont-3.0.5/tests/data/testotfs/a919b33197965846f21074b24e30250d67277bce.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf` & `babelfont-3.0.5/tests/data/testotfs/a98e908e2ed21b22228ea59ebcc0f05034c86f2e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf` & `babelfont-3.0.5/tests/data/testotfs/ab14b4eb9d7a67e293f51d30d719add06c9d6e06.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf` & `babelfont-3.0.5/tests/data/testotfs/ab40c89624a6104e5d0a2308e448a989302f515b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf` & `babelfont-3.0.5/tests/data/testotfs/ad01ab2ea1cb1a4d3a2783e2675112ef11ae6404.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf` & `babelfont-3.0.5/tests/data/testotfs/af3086380b743099c54a3b11b96766039ea62fcd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf` & `babelfont-3.0.5/tests/data/testotfs/af85624080af5627fb050f570d148a62f04fda74.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf` & `babelfont-3.0.5/tests/data/testotfs/b151cfcdaa77585d77f17a42158e0873fc8e2633.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf` & `babelfont-3.0.5/tests/data/testotfs/b6031119874ae9ff1dd65383a335e361c0962220.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf` & `babelfont-3.0.5/tests/data/testotfs/b722a7d09e60421f3efbc706ad348ab47b88567b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf` & `babelfont-3.0.5/tests/data/testotfs/bb0c53752e85c3d28973ebc913287b8987d3dfe8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf` & `babelfont-3.0.5/tests/data/testotfs/bb9473d2403488714043bcfb946c9f78b86ad627.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf` & `babelfont-3.0.5/tests/data/testotfs/bf39b0e91ef9807f15a9e283a21a14a209fd2cfc.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf` & `babelfont-3.0.5/tests/data/testotfs/bf962d3202883a820aed019d9b5c1838c2ff69c6.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf` & `babelfont-3.0.5/tests/data/testotfs/c4e48b0886ef460f532fb49f00047ec92c432ec0.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf` & `babelfont-3.0.5/tests/data/testotfs/cc5f3d2d717fb6bd4dfae1c16d48a2cb8e12233b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf` & `babelfont-3.0.5/tests/data/testotfs/d23d76ea0909c14972796937ba072b5a40c1e257.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf` & `babelfont-3.0.5/tests/data/testotfs/d3129450fafe5e5c98cfc25a4e71809b1b4d2855.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf` & `babelfont-3.0.5/tests/data/testotfs/d629e7fedc0b350222d7987345fe61613fa3929a.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf` & `babelfont-3.0.5/tests/data/testotfs/d9b8bc10985f24796826c29f7ccba3d0ae11ec02.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf` & `babelfont-3.0.5/tests/data/testotfs/dcf774ca21062e7439f98658b18974ea8b956d0c.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf` & `babelfont-3.0.5/tests/data/testotfs/df768b9c257e0c9c35786c47cae15c46571d56be.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf` & `babelfont-3.0.5/tests/data/testotfs/e39391c77a6321c2ac7a2d644de0396470cd4bfe.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf` & `babelfont-3.0.5/tests/data/testotfs/e68a88939e0f06e34d2bc911f09b70890289c8fd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf` & `babelfont-3.0.5/tests/data/testotfs/ea3f63620511b2097200d23774ffef197e829e69.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf` & `babelfont-3.0.5/tests/data/testotfs/ee39587d13b2afa5499cc79e45780aa79293bbd4.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf` & `babelfont-3.0.5/tests/data/testotfs/ef86fe710cfea877bbe0dbb6946a1f88d0661031.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf` & `babelfont-3.0.5/tests/data/testotfs/f22416c692720a7d46fadf4af99f4c9e094f00b9.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf` & `babelfont-3.0.5/tests/data/testotfs/f443753e8ffe8e8aae606cfba158e00334b6efb1.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf` & `babelfont-3.0.5/tests/data/testotfs/f518eb6f6b5eec2946c9fbbbde44e45d46f5e2ac.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf` & `babelfont-3.0.5/tests/data/testotfs/f75c4b05a0a4d67c1a808081ae3d74a9c66509e8.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf` & `babelfont-3.0.5/tests/data/testotfs/f79eb71df4e4c9c273b67b89a06e5ff9e3c1f834.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf` & `babelfont-3.0.5/tests/data/testotfs/f9b1dd4dcb515e757789a22cb4241107746fd3d0.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf` & `babelfont-3.0.5/tests/data/testotfs/fbb6c84c9e1fe0c39e152fbe845e51fd81f6748e.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf` & `babelfont-3.0.5/tests/data/testotfs/fcbaa518d3cce441ed37ae3b1fed6a19e9b54efd.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf` & `babelfont-3.0.5/tests/data/testotfs/fcdcffbdf1c4c97c05308d7600e4c283eb47dbca.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf` & `babelfont-3.0.5/tests/data/testotfs/ffa0f5d2d9025486d8469d8b1fdd983e7632499b.ttf`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/test_features.py` & `babelfont-3.0.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/test_glyphs3_roundtrip.py` & `babelfont-3.0.5/tests/test_glyphs3_roundtrip.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.4/tests/test_otf_loader.py` & `babelfont-3.0.5/tests/test_otf_loader.py`

 * *Files identical despite different names*

