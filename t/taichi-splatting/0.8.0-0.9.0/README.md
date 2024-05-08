# Comparing `tmp/taichi-splatting-0.8.0.tar.gz` & `tmp/taichi-splatting-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichi-splatting-0.8.0.tar", last modified: Sun Feb 11 08:53:17 2024, max compression
+gzip compressed data, was "taichi-splatting-0.9.0.tar", last modified: Sat Feb 24 13:51:52 2024, max compression
```

## Comparing `taichi-splatting-0.8.0.tar` & `taichi-splatting-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2095 2023-12-17 15:27:43.000000 taichi-splatting-0.8.0/.gitignore
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3601 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/BENCHMARK.md
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    11357 2023-12-17 15:27:05.000000 taichi-splatting-0.8.0/LICENSE
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      122 2023-12-19 14:10:11.000000 taichi-splatting-0.8.0/NOTICE
--rw-r--r--   0 oliver    (1000) oliver    (1000)    17774 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/PKG-INFO
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4449 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/README.md
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.554978 taichi-splatting-0.8.0/benchmarks/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    52877 2024-02-03 12:39:16.000000 taichi-splatting-0.8.0/benchmarks/4090-2048px.png
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2836 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/benchmark-2070.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2937 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/benchmark-3090.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2994 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/benchmark-4090.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3706 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/make_charts.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    37422 2024-02-03 12:39:16.000000 taichi-splatting-0.8.0/benchmarks/overall.png
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.558978 taichi-splatting-0.8.0/benchmarks/raw/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6295 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/raw/benchmark-2070.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6373 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/raw/benchmark-3090.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6377 2024-02-03 12:39:22.000000 taichi-splatting-0.8.0/benchmarks/raw/benchmark-4090.csv
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    36478 2024-02-03 12:39:16.000000 taichi-splatting-0.8.0/benchmarks/speedup.png
--rw-rw-r--   0 oliver    (1000) oliver    (1000)  3872931 2024-02-03 13:46:13.000000 taichi-splatting-0.8.0/benchmarks/test.png
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.558978 taichi-splatting-0.8.0/profiles/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10073 2024-02-03 12:39:16.000000 taichi-splatting-0.8.0/profiles/bicycle_2048.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1387 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/pyproject.toml
--rw-rw-r--   0 oliver    (1000) oliver    (1000)       38 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/setup.cfg
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.558978 taichi-splatting-0.8.0/taichi_splatting/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      424 2024-01-31 11:07:33.000000 taichi-splatting-0.8.0/taichi_splatting/__init__.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/benchmarks/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-07 09:29:16.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2511 2024-01-16 14:16:00.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_projection.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3511 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_rasterizer.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1876 2024-01-16 14:16:00.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_sh.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2776 2024-02-11 07:19:34.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_tilemapper.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1099 2024-02-03 13:46:13.000000 taichi-splatting-0.8.0/taichi_splatting/benchmarks/util.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1467 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2419 2024-01-19 10:16:28.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/full_cumsum.cu
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      764 2024-01-21 02:42:40.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/module.cpp
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2626 2024-01-21 02:42:40.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/radix_sort_pairs.cu
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2748 2024-01-19 10:16:28.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/segmented_sort_pairs.cu
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1797 2024-01-21 02:42:40.000000 taichi-splatting-0.8.0/taichi_splatting/cuda_lib/sort_pairs.cu
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2415 2024-02-03 13:46:13.000000 taichi-splatting-0.8.0/taichi_splatting/data_types.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/examples/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-02-03 13:46:13.000000 taichi-splatting-0.8.0/taichi_splatting/examples/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6132 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/examples/fit_image_gaussians.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4467 2024-02-11 07:19:34.000000 taichi-splatting-0.8.0/taichi_splatting/examples/renderer2d.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1090 2024-02-11 07:19:34.000000 taichi-splatting-0.8.0/taichi_splatting/examples/vis_split.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/mapper/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-21 02:43:40.000000 taichi-splatting-0.8.0/taichi_splatting/mapper/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7127 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/mapper/bump_mapper.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5623 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/mapper/segmented_tile_mapper.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7260 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/mapper/tile_mapper.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/misc/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-12 14:13:48.000000 taichi-splatting-0.8.0/taichi_splatting/misc/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      439 2024-01-12 14:13:48.000000 taichi-splatting-0.8.0/taichi_splatting/misc/autograd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2379 2024-01-12 14:13:48.000000 taichi-splatting-0.8.0/taichi_splatting/misc/depth_variance.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1143 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/misc/encode_depth.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1706 2024-01-13 00:45:26.000000 taichi-splatting-0.8.0/taichi_splatting/misc/indexing.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4272 2024-02-09 11:39:15.000000 taichi-splatting-0.8.0/taichi_splatting/misc/parameter_class.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4472 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/misc/renderer2d.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.562978 taichi-splatting-0.8.0/taichi_splatting/perspective/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      188 2024-01-10 07:40:01.000000 taichi-splatting-0.8.0/taichi_splatting/perspective/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1648 2024-01-14 13:08:21.000000 taichi-splatting-0.8.0/taichi_splatting/perspective/culling.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1927 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/perspective/params.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2691 2024-01-12 14:13:48.000000 taichi-splatting-0.8.0/taichi_splatting/perspective/plane_culling.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4219 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/perspective/projection.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/taichi_splatting/rasterizer/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      155 2024-01-10 07:44:51.000000 taichi-splatting-0.8.0/taichi_splatting/rasterizer/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9261 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/rasterizer/backward.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5018 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/rasterizer/forward.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6892 2024-02-11 07:26:30.000000 taichi-splatting-0.8.0/taichi_splatting/rasterizer/function.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1573 2024-01-12 14:13:48.000000 taichi-splatting-0.8.0/taichi_splatting/rasterizer/tiling.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3510 2024-02-11 07:27:05.000000 taichi-splatting-0.8.0/taichi_splatting/renderer.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5536 2024-01-20 07:31:38.000000 taichi-splatting-0.8.0/taichi_splatting/spherical_harmonics.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3128 2024-02-10 04:40:01.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/concurrent.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      680 2023-12-31 09:43:52.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/conversions.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      183 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/f32.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      183 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/f64.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9935 2024-01-14 13:08:21.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/generic.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3570 2024-01-21 10:12:28.000000 taichi-splatting-0.8.0/taichi_splatting/taichi_lib/grid_query.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/taichi_splatting/tests/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2023-12-28 09:54:32.000000 taichi-splatting-0.8.0/taichi_splatting/tests/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3025 2024-02-03 13:46:13.000000 taichi-splatting-0.8.0/taichi_splatting/tests/random_data.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      461 2024-01-21 02:42:40.000000 taichi-splatting-0.8.0/taichi_splatting/tests/test_benchmarks.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2903 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/tests/test_conic.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2812 2024-01-10 14:21:15.000000 taichi-splatting-0.8.0/taichi_splatting/tests/test_projection.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1777 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/tests/test_spherical_harmonics.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1847 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/tests/util.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/taichi_splatting/torch_ops/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2023-12-28 10:02:56.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4046 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/projection.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    46941 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/rsh.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1415 2024-01-24 10:56:32.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/spherical_harmonics.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1330 2024-02-04 14:04:14.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/transforms.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      343 2023-12-28 10:04:33.000000 taichi-splatting-0.8.0/taichi_splatting/torch_ops/util.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-11 08:53:17.566978 taichi-splatting-0.8.0/taichi_splatting.egg-info/
--rw-r--r--   0 oliver    (1000) oliver    (1000)    17774 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/PKG-INFO
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3067 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/SOURCES.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/dependency_links.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      350 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/entry_points.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)       40 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/requires.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)       17 2024-02-11 08:53:17.000000 taichi-splatting-0.8.0/taichi_splatting.egg-info/top_level.txt
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2095 2023-12-17 15:27:43.000000 taichi-splatting-0.9.0/.gitignore
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4073 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/BENCHMARK.md
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    11357 2023-12-17 15:27:05.000000 taichi-splatting-0.9.0/LICENSE
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      122 2023-12-19 14:10:11.000000 taichi-splatting-0.9.0/NOTICE
+-rw-r--r--   0 oliver    (1000) oliver    (1000)    18100 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/PKG-INFO
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4783 2024-02-23 13:00:52.000000 taichi-splatting-0.9.0/README.md
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.668348 taichi-splatting-0.9.0/benchmarks/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    52877 2024-02-03 12:39:16.000000 taichi-splatting-0.9.0/benchmarks/4090-2048px.png
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2836 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/benchmark-2070.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2937 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/benchmark-3090.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2994 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/benchmark-4090.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3706 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/make_charts.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    37422 2024-02-03 12:39:16.000000 taichi-splatting-0.9.0/benchmarks/overall.png
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.672348 taichi-splatting-0.9.0/benchmarks/raw/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6295 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/raw/benchmark-2070.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6373 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/raw/benchmark-3090.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6377 2024-02-03 12:39:22.000000 taichi-splatting-0.9.0/benchmarks/raw/benchmark-4090.csv
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    36478 2024-02-03 12:39:16.000000 taichi-splatting-0.9.0/benchmarks/speedup.png
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)  3872931 2024-02-03 13:46:13.000000 taichi-splatting-0.9.0/benchmarks/test.png
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.672348 taichi-splatting-0.9.0/profiles/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10073 2024-02-03 12:39:16.000000 taichi-splatting-0.9.0/profiles/bicycle_2048.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1388 2024-02-24 13:32:19.000000 taichi-splatting-0.9.0/pyproject.toml
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)       38 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/setup.cfg
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.676348 taichi-splatting-0.9.0/taichi_splatting/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      667 2024-02-24 13:36:31.000000 taichi-splatting-0.9.0/taichi_splatting/__init__.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.676348 taichi-splatting-0.9.0/taichi_splatting/benchmarks/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-07 09:29:16.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2511 2024-01-16 14:16:00.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_projection.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3551 2024-02-19 14:43:33.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_rasterizer.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1876 2024-01-16 14:16:00.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_sh.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2776 2024-02-11 07:19:34.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_tilemapper.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1099 2024-02-03 13:46:13.000000 taichi-splatting-0.9.0/taichi_splatting/benchmarks/util.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.676348 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1467 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2419 2024-01-19 10:16:28.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/full_cumsum.cu
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      764 2024-01-21 02:42:40.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/module.cpp
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2626 2024-01-21 02:42:40.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/radix_sort_pairs.cu
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2748 2024-01-19 10:16:28.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/segmented_sort_pairs.cu
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1797 2024-01-21 02:42:40.000000 taichi-splatting-0.9.0/taichi_splatting/cuda_lib/sort_pairs.cu
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2415 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/data_types.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.676348 taichi-splatting-0.9.0/taichi_splatting/examples/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-02-03 13:46:13.000000 taichi-splatting-0.9.0/taichi_splatting/examples/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7491 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/examples/fit_image_gaussians.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4467 2024-02-11 07:19:34.000000 taichi-splatting-0.9.0/taichi_splatting/examples/renderer2d.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1090 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/examples/vis_split.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.680348 taichi-splatting-0.9.0/taichi_splatting/mapper/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-21 02:43:40.000000 taichi-splatting-0.9.0/taichi_splatting/mapper/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7127 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/mapper/bump_mapper.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5623 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/mapper/segmented_tile_mapper.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7260 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/mapper/tile_mapper.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.680348 taichi-splatting-0.9.0/taichi_splatting/misc/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2024-01-12 14:13:48.000000 taichi-splatting-0.9.0/taichi_splatting/misc/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      439 2024-01-12 14:13:48.000000 taichi-splatting-0.9.0/taichi_splatting/misc/autograd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2379 2024-01-12 14:13:48.000000 taichi-splatting-0.9.0/taichi_splatting/misc/depth_variance.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1143 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/misc/encode_depth.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1706 2024-01-13 00:45:26.000000 taichi-splatting-0.9.0/taichi_splatting/misc/indexing.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4412 2024-02-24 04:20:25.000000 taichi-splatting-0.9.0/taichi_splatting/misc/parameter_class.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1925 2024-02-24 12:37:44.000000 taichi-splatting-0.9.0/taichi_splatting/misc/radius.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4472 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/misc/renderer2d.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.680348 taichi-splatting-0.9.0/taichi_splatting/perspective/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      188 2024-01-10 07:40:01.000000 taichi-splatting-0.9.0/taichi_splatting/perspective/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1648 2024-01-14 13:08:21.000000 taichi-splatting-0.9.0/taichi_splatting/perspective/culling.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1927 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/perspective/params.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2691 2024-01-12 14:13:48.000000 taichi-splatting-0.9.0/taichi_splatting/perspective/plane_culling.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4560 2024-02-24 11:54:50.000000 taichi-splatting-0.9.0/taichi_splatting/perspective/projection.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.680348 taichi-splatting-0.9.0/taichi_splatting/rasterizer/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      205 2024-02-24 13:37:02.000000 taichi-splatting-0.9.0/taichi_splatting/rasterizer/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9740 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/rasterizer/backward.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5018 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/rasterizer/forward.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6950 2024-02-24 13:36:49.000000 taichi-splatting-0.9.0/taichi_splatting/rasterizer/function.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1573 2024-01-12 14:13:48.000000 taichi-splatting-0.9.0/taichi_splatting/rasterizer/tiling.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4955 2024-02-24 13:31:18.000000 taichi-splatting-0.9.0/taichi_splatting/renderer.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5536 2024-02-24 03:20:55.000000 taichi-splatting-0.9.0/taichi_splatting/spherical_harmonics.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.680348 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      227 2024-02-24 13:24:09.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3128 2024-02-10 04:40:01.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/concurrent.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      680 2023-12-31 09:43:52.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/conversions.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      183 2023-12-28 10:04:33.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/f32.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      183 2023-12-28 10:04:33.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/f64.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9886 2024-02-24 13:22:48.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/generic.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3570 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/taichi_lib/grid_query.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/taichi_splatting/tests/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2023-12-28 09:54:32.000000 taichi-splatting-0.9.0/taichi_splatting/tests/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3025 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/tests/random_data.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      461 2024-01-21 02:42:40.000000 taichi-splatting-0.9.0/taichi_splatting/tests/test_benchmarks.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2903 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/tests/test_conic.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2825 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/tests/test_projection.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1777 2023-12-28 10:04:33.000000 taichi-splatting-0.9.0/taichi_splatting/tests/test_spherical_harmonics.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1553 2024-02-24 04:24:08.000000 taichi-splatting-0.9.0/taichi_splatting/tests/util.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/taichi_splatting/torch_ops/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2023-12-28 10:02:56.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4046 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/projection.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    46941 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/rsh.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1415 2024-01-24 10:56:32.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/spherical_harmonics.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1330 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/transforms.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      530 2024-02-23 13:23:22.000000 taichi-splatting-0.9.0/taichi_splatting/torch_ops/util.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2024-02-24 13:51:52.684348 taichi-splatting-0.9.0/taichi_splatting.egg-info/
+-rw-r--r--   0 oliver    (1000) oliver    (1000)    18100 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/PKG-INFO
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3099 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/SOURCES.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/dependency_links.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      351 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/entry_points.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)       40 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/requires.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)       17 2024-02-24 13:51:52.000000 taichi-splatting-0.9.0/taichi_splatting.egg-info/top_level.txt
```

### Comparing `taichi-splatting-0.8.0/.gitignore` & `taichi-splatting-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/BENCHMARK.md` & `taichi-splatting-0.9.0/BENCHMARK.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 Charts showing overall averages across benchmark scenes. (details below!)
 
 <img src="benchmarks/overall.png" width="100%">
 <img src="benchmarks/speedup.png" width="100%">
 
 ## Method
 
+### Implementations shown
+
+* gaussian-splatting - original (cuda) implementation for gaussian-splatting paper [diff_gaussian_rasterizer](https://github.com/graphdeco-inria/diff-gaussian-rasterization) 
+* taichi(original) - original taichi implementation [taichi_3d_gaussian_splatting](https://github.com/wanmeihuali/taichi_3d_gaussian_splatting) 
+* taichi-splatting(16) - our implementation with tile_size=16
+* taichi-splatting(32) - our implementation with tile_size=32
+
 ### Assets required
 
 The benchmark uses reconstructions from the official gaussian-splatting implementation. These can be found from the official [gaussian-splatting](https://github.com/graphdeco-inria/gaussian-splatting) page. Under [Pre-trained models](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/datasets/pretrained/models.zip).
 
 Though it can also be run on any other reconstructions, this is a good common benchmark.
```

### Comparing `taichi-splatting-0.8.0/LICENSE` & `taichi-splatting-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/PKG-INFO` & `taichi-splatting-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taichi-splatting
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Taichi Gaussian Splatting library
 Maintainer-email: Oliver Batchelor <oliver.batchelor@canterbury.ac.nz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,14 +254,22 @@
 
 ## Executables
 
 ### fit_image_gaussians
 
 There exists a toy optimizer for fitting a set of randomly initialized gaussians to some 2D images `fit_image_gaussians` - useful for testing rasterization without the rest of the dependencies.
 
+Fitting an image (fixed points): \
+`fit_image_gaussians <image file> --show  --n 20000` 
+
+Fitting an image (split and prune to target): \
+`fit_image_gaussians <image file> --show --n 1000 --target 20000` 
+
+See `--help` for other options.
+
 ### benchmarks
 
 There exist benchmarks to evaluate performance on individual components in isolation under `taichi_splatting/benchmarks/`
 
 ### tests 
 
 Tests (gradient tests and tests comparing to torch-based reference implementations) can be run with pytest, or individually under 
@@ -289,15 +297,15 @@
 * Spherical harmonics with autograd
 * Gradient tests for most parts (float64)
 * Fit to image training example/test
 * Depth and depth-covariance rendering
 
 * Compute point visibility in backward pass (useful for model pruning)
 * Example training on images with split/prune operations
-
+* Novel heuristics for split and prune operations computed optionally in backward pass 
 
 
 ### Todo
 
 * Depth covariance example
 
 * 3D training code (likely different repository)
```

### Comparing `taichi-splatting-0.8.0/README.md` & `taichi-splatting-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,22 @@
 
 ## Executables
 
 ### fit_image_gaussians
 
 There exists a toy optimizer for fitting a set of randomly initialized gaussians to some 2D images `fit_image_gaussians` - useful for testing rasterization without the rest of the dependencies.
 
+Fitting an image (fixed points): \
+`fit_image_gaussians <image file> --show  --n 20000` 
+
+Fitting an image (split and prune to target): \
+`fit_image_gaussians <image file> --show --n 1000 --target 20000` 
+
+See `--help` for other options.
+
 ### benchmarks
 
 There exist benchmarks to evaluate performance on individual components in isolation under `taichi_splatting/benchmarks/`
 
 ### tests 
 
 Tests (gradient tests and tests comparing to torch-based reference implementations) can be run with pytest, or individually under 
@@ -72,15 +80,15 @@
 * Spherical harmonics with autograd
 * Gradient tests for most parts (float64)
 * Fit to image training example/test
 * Depth and depth-covariance rendering
 
 * Compute point visibility in backward pass (useful for model pruning)
 * Example training on images with split/prune operations
-
+* Novel heuristics for split and prune operations computed optionally in backward pass 
 
 
 ### Todo
 
 * Depth covariance example
 
 * 3D training code (likely different repository)
```

### Comparing `taichi-splatting-0.8.0/benchmarks/4090-2048px.png` & `taichi-splatting-0.9.0/benchmarks/4090-2048px.png`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/benchmark-2070.csv` & `taichi-splatting-0.9.0/benchmarks/benchmark-2070.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/benchmark-3090.csv` & `taichi-splatting-0.9.0/benchmarks/benchmark-3090.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/benchmark-4090.csv` & `taichi-splatting-0.9.0/benchmarks/benchmark-4090.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/make_charts.py` & `taichi-splatting-0.9.0/benchmarks/make_charts.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/overall.png` & `taichi-splatting-0.9.0/benchmarks/overall.png`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/raw/benchmark-2070.csv` & `taichi-splatting-0.9.0/benchmarks/raw/benchmark-2070.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/raw/benchmark-3090.csv` & `taichi-splatting-0.9.0/benchmarks/raw/benchmark-3090.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/raw/benchmark-4090.csv` & `taichi-splatting-0.9.0/benchmarks/raw/benchmark-4090.csv`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/speedup.png` & `taichi-splatting-0.9.0/benchmarks/speedup.png`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/benchmarks/test.png` & `taichi-splatting-0.9.0/benchmarks/test.png`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/profiles/bicycle_2048.txt` & `taichi-splatting-0.9.0/profiles/bicycle_2048.txt`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/pyproject.toml` & `taichi-splatting-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "taichi-splatting"  
-version = "0.8.0"  
+version = "0.9.0"  
 description = "A Taichi Gaussian Splatting library"  
 readme = "README.md" 
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 
 maintainers = [
   {name = "Oliver Batchelor", email = "oliver.batchelor@canterbury.ac.nz" } 
@@ -31,15 +31,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [options]
 dependency_links = ["https://pypi.taichi.graphics/simple/"]
 
 [project.scripts]  # Optional
-fit_image_gaussians = "taichi_splatting.scripts.fit_image_gaussians:main"
+fit_image_gaussians = "taichi_splatting.examples.fit_image_gaussians:main"
 bench_projection = "taichi_splatting.benchmarks.bench_projection:main"
 bench_rasterizer = "taichi_splatting.benchmarks.bench_rasterizer:main"
 bench_tilemapper = "taichi_splatting.benchmarks.bench_tilemapper:main"
 
 bench_sh = "taichi_splatting.benchmarks.bench_sh:main"
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_projection.py` & `taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_projection.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_rasterizer.py` & `taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_rasterizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,22 +76,22 @@
 
   gaussians.feature.requires_grad_(True)
   gaussians2d.requires_grad_(True)
 
   benchmarked('backward (all)', backward, profile=args.profile, iters=args.iters)  
 
   
-  def compute_weight():
+  def compute_split_heuristics():
     raster = rasterize_with_tiles(gaussians2d=gaussians2d, features=gaussians.feature, 
       tile_overlap_ranges=tile_ranges.view(-1, 2), overlap_to_point=overlap_to_point,
-      image_size=args.image_size, config=config, compute_weight=True)
+      image_size=args.image_size, config=config, compute_split_heuristics=True)
     
     raster.image.sum().backward()
 
-  benchmarked('backward (compute_weight)', compute_weight, profile=args.profile, iters=args.iters)  
+  benchmarked('backward (compute_split_heuristics)', compute_split_heuristics, profile=args.profile, iters=args.iters)  
 
 
 def main():
   args = parse_args()
   bench_rasterizer(args)
 
 if __name__ == '__main__':
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_sh.py` & `taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_sh.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/benchmarks/bench_tilemapper.py` & `taichi-splatting-0.9.0/taichi_splatting/benchmarks/bench_tilemapper.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/benchmarks/util.py` & `taichi-splatting-0.9.0/taichi_splatting/benchmarks/util.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/__init__.py` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/full_cumsum.cu` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/full_cumsum.cu`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/module.cpp` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/module.cpp`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/radix_sort_pairs.cu` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/radix_sort_pairs.cu`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/segmented_sort_pairs.cu` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/segmented_sort_pairs.cu`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/cuda_lib/sort_pairs.cu` & `taichi-splatting-0.9.0/taichi_splatting/cuda_lib/sort_pairs.cu`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/data_types.py` & `taichi-splatting-0.9.0/taichi_splatting/data_types.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/examples/fit_image_gaussians.py` & `taichi-splatting-0.9.0/taichi_splatting/examples/fit_image_gaussians.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import math
+from pathlib import Path
 import cv2
 import argparse
+import numpy as np
 import taichi as ti
 
 import torch
 from taichi_splatting.data_types import Gaussians2D, RasterConfig
+from taichi_splatting.mapper.tile_mapper import map_to_tiles
 from taichi_splatting.misc.encode_depth import encode_depth32
 from taichi_splatting.misc.renderer2d import project_gaussians2d, split_gaussians2d, uniform_split_gaussians2d
 
-from taichi_splatting.rasterizer.function import rasterize
+from taichi_splatting.rasterizer.function import rasterize, rasterize_with_tiles
 
 from taichi_splatting.misc.parameter_class import ParameterClass
 from taichi_splatting.tests.random_data import random_2d_gaussians
 
 from taichi_splatting.torch_ops.util import check_finite
 from torch.profiler import profile, record_function, ProfilerActivity
 
@@ -20,81 +23,76 @@
 
 
 def parse_args():
   parser = argparse.ArgumentParser()
   parser.add_argument('image_file', type=str)
   parser.add_argument('--seed', type=int, default=0)
   parser.add_argument('--tile_size', type=int, default=16)
-  parser.add_argument('--n', type=int, default=20000)
 
+  parser.add_argument('--n', type=int, default=1000)
+  parser.add_argument('--target', type=int, default=None)
+  parser.add_argument('--max_epoch', type=int, default=200)
+  parser.add_argument('--split_rate', type=float, default=0.1, help='Rate of points to split each epoch (proportional to number of points)')
+
+  parser.add_argument('--write_frames', type=Path, default=None)
 
   parser.add_argument('--debug', action='store_true')
   parser.add_argument('--show', action='store_true')
 
-  parser.add_argument('--split', action='store_true', help="Enable splitting of gaussians")
-
-  parser.add_argument('--grad-threshold', type=float, default=2e-7)
-  parser.add_argument('--vis-threshold', type=float, default=4)
-
   parser.add_argument('--profile', action='store_true')
-  parser.add_argument('--epoch', type=int, default=100, help='Number of iterations per measurement/profiling')
+  parser.add_argument('--epoch', type=int, default=20, help='Number of iterations per measurement/profiling')
   
   return parser.parse_args()
 
-def inverse_sigmoid(x):
-  return math.log(x / (1 - x))
-
 
 def display_image(name, image):
     image = (image.detach().clamp(0, 1) * 255).to(torch.uint8)
     image = image.cpu().numpy()
 
     cv2.imshow(name, image)
     cv2.waitKey(1)
     
 
 def psnr(a, b):
   return 10 * torch.log10(1 / torch.nn.functional.mse_loss(a, b))  
 
 
-def train_epoch(opt, gaussians, ref_image, epoch_size=100, config:RasterConfig = RasterConfig()):
+def train_epoch(opt, gaussians, ref_image, epoch_size=100, config:RasterConfig = RasterConfig(), grad_alpha=0.9):
     h, w = ref_image.shape[:2]
 
-    gradient = torch.zeros(gaussians.batch_size, device=gaussians.position.device)
-    visibility = torch.zeros(gaussians.batch_size, device=gaussians.position.device)
+    contrib = torch.zeros((gaussians.batch_size[0], 2), device=gaussians.position.device)
 
-    for _ in range(epoch_size):
+    for i in range(epoch_size):
       opt.zero_grad()
 
-      gaussians2d = project_gaussians2d(gaussians)
-      gaussians2d.retain_grad()
-
-      # gaussians.feature.retain_grad()
-      
+      gaussians2d = project_gaussians2d(gaussians)  
       depths = encode_depth32(gaussians.depth)
+
       raster = rasterize(gaussians2d=gaussians2d, 
         encoded_depths=depths,
         features=gaussians.feature, 
         image_size=(w, h), 
         config=config,
-        compute_weight=True)
+        compute_split_heuristics=True)
 
-      loss = torch.nn.functional.l1_loss(raster.image, ref_image) 
+      loss = torch.nn.functional.l1_loss(raster.image, ref_image) #+ (1e-4 * gaussians.log_scaling).pow(2).sum()
       loss.backward()
 
-
-      visibility += raster.point_weight
-      check_finite(gaussians)
+      check_finite(gaussians, 'gaussians', warn=True)
       opt.step()
 
       with torch.no_grad():
         gaussians.log_scaling.clamp_(min=-1, max=4)
-        gradient += gaussians2d.grad[:, 0:2].norm(dim=-1) 
 
-    return raster.image, gradient, visibility 
+        contrib =  raster.point_split_heuristics if i == 0 \
+            else (1 - grad_alpha) * contrib + grad_alpha * raster.point_split_heuristics
+
+
+      visibility, gradient = contrib.unbind(dim=1)
+    return raster.image, visibility, gradient 
 
 
 def main():
   device = torch.device('cuda:0')
 
   cmd_args = parse_args()
   
@@ -103,86 +101,120 @@
 
   ti.init(arch=ti.cuda, log_level=ti.INFO, 
           debug=cmd_args.debug, device_memory_GB=0.1)
 
   print(f'Image size: {w}x{h}')
 
   if cmd_args.show:
-    cv2.namedWindow('rendered', cv2.WINDOW_NORMAL)
     cv2.namedWindow('gradient', cv2.WINDOW_NORMAL)
+    cv2.namedWindow('err', cv2.WINDOW_NORMAL)
+    cv2.namedWindow('rendered', cv2.WINDOW_NORMAL)
 
-    cv2.resizeWindow('rendered', w, h)
     cv2.resizeWindow('gradient', w, h)
+    cv2.resizeWindow('err', w, h)
+    cv2.resizeWindow('rendered', w, h)
+
 
   torch.manual_seed(cmd_args.seed)
 
   gaussians = random_2d_gaussians(cmd_args.n, (w, h), scale_factor=0.1).to(torch.device('cuda:0'))
   learning_rates = dict(
-    position=0.2,
+    position=0.1,
     log_scaling=0.05,
     rotation=0.005,
     alpha_logit=0.1,
     feature=0.01
   )
   
 
   params = ParameterClass.create(gaussians.to_tensordict(), learning_rates, base_lr=1.0)
+  keys = set(params.keys())
+  trainable = set(params.optimized_keys())
 
-  print(list(params.keys()))
+  print(f'attributes - trainable: {trainable} other: {keys - trainable}')
 
   ref_image = torch.from_numpy(ref_image).to(dtype=torch.float32, device=device) / 255
-  config = RasterConfig(tile_size=cmd_args.tile_size, gaussian_scale=3.)
+  config = RasterConfig(tile_size=cmd_args.tile_size, gaussian_scale=3.0)
 
 
 
   def timed_epoch(*args, **kwargs):
     start = time.time()
     image, grad, vis = train_epoch(*args, **kwargs)
     torch.cuda.synchronize()
     end = time.time()
 
-    cpsnr = psnr(ref_image, image)
-    print(f'{cmd_args.epoch / (end - start):.1f} iters/sec CPSNR {cpsnr:.2f}')
-    return image, grad, vis
+    return image, grad, vis, end - start
 
 
-  train = with_benchmark(train_epoch) if cmd_args.profile else timed_epoch
+  train = with_benchmark(timed_epoch) if cmd_args.profile else timed_epoch
 
-  while True:
-    image, gradient, visibility = train(params.optimizer, params, ref_image, epoch_size=cmd_args.epoch, config=config)
+  
+  split_rate = cmd_args.split_rate
+
+  for epoch in range(cmd_args.max_epoch):
+    epoch_size = cmd_args.epoch
 
+    image, gradient, visibility, epoch_time = train(params.optimizer, params, ref_image, 
+                                        epoch_size=epoch_size, config=config)
+    
 
     with torch.no_grad():
 
       if cmd_args.show:
         gaussians2d = project_gaussians2d(params)
         depths = encode_depth32(params.depth)
-        raster =  rasterize(gaussians2d, depths, gradient.unsqueeze(-1), image_size=(w, h), config=config, compute_weight=True)
+        raster =  rasterize(gaussians2d, depths, gradient.contiguous().unsqueeze(-1), image_size=(w, h), config=config, compute_split_heuristics=True)
 
+        err = torch.abs(ref_image - image)
         
-        display_image('gradient', (0.5 * raster.image / (cmd_args.epoch * cmd_args.grad_threshold) ))
+        display_image('gradient', (0.5 * raster.image / raster.image.mean() ))
         display_image('rendered', image)
+        display_image('err',  0.25 * err / err.mean(dim=(0, 1), keepdim=True))
 
+    
+      if cmd_args.write_frames:
+        filename = cmd_args.write_frames / f'{epoch:04d}.png'
+        filename.parent.mkdir(exist_ok=True, parents=True)
+        print(f'Writing {filename}')
+        cv2.imwrite(str(filename), 
+                    (image.detach().clamp(0, 1) * 255).cpu().numpy())
 
-      if cmd_args.split:
-        gaussians = Gaussians2D(**params.tensors, batch_size=params.batch_size)
-        grad_thresh = cmd_args.epoch * cmd_args.grad_threshold
-        vis_threshold = cmd_args.epoch * cmd_args.vis_threshold 
+      cpsnr = psnr(ref_image, image)
+      print(f'{epoch}: {epoch_size / epoch_time:.1f} iters/sec CPSNR {cpsnr:.2f}')
 
-        transparent = (visibility < vis_threshold) & (gradient < grad_thresh)
-        split_mask = torch.zeros_like(transparent, dtype=torch.bool)
+      if cmd_args.target:
+        gaussians = Gaussians2D(**params.tensors, batch_size=params.batch_size)
 
-        split_mask = (gradient > grad_thresh) & (visibility > 2 * vis_threshold)
+        split_ratio = np.clip(cmd_args.target / gaussians.batch_size[0], 
+                              a_min=0.25, a_max=4)
         
+        if min(split_ratio, 1/split_ratio) > 0.98:
+          factor = math.pow(split_rate, 1/(cmd_args.max_epoch - epoch))
+
+          split_rate *= factor
+
+
+        grad_thresh = torch.quantile(gradient, 1 - (split_rate * split_ratio))
+        vis_thresh = torch.quantile(visibility, split_rate * 1/split_ratio )
+
+    
+        prune_mask = (visibility <= vis_thresh)  & (gradient <  grad_thresh)
+        split_mask = torch.zeros_like(prune_mask, dtype=torch.bool)
+
+        split_mask = (gradient > grad_thresh) & (visibility > vis_thresh)
         splits = split_gaussians2d(gaussians[split_mask], scaling=0.8)
 
-        params = params[~(split_mask | transparent)]
+        params = params[~(split_mask | prune_mask)]
         params = params.append_tensors(splits.to_tensordict())
+        # # # params = params[~prune_mask]
+
+        print(f" split {split_mask.sum()}, pruned {prune_mask.sum()} {params.batch_size} points")
 
-        print(f"Split {split_mask.sum()}, pruned {transparent.sum()} total {params.batch_size} points") 
+        
 
 
 def with_benchmark(f):
   def g(*args , **kwargs):
     with profile(activities=[ProfilerActivity.CUDA], record_shapes=True) as prof:
       with record_function("model_inference"):
         result = f(*args, **kwargs)
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/examples/renderer2d.py` & `taichi-splatting-0.9.0/taichi_splatting/examples/renderer2d.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/examples/vis_split.py` & `taichi-splatting-0.9.0/taichi_splatting/examples/vis_split.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/mapper/bump_mapper.py` & `taichi-splatting-0.9.0/taichi_splatting/mapper/bump_mapper.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/mapper/segmented_tile_mapper.py` & `taichi-splatting-0.9.0/taichi_splatting/mapper/segmented_tile_mapper.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/mapper/tile_mapper.py` & `taichi-splatting-0.9.0/taichi_splatting/mapper/tile_mapper.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/misc/depth_variance.py` & `taichi-splatting-0.9.0/taichi_splatting/misc/depth_variance.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/misc/encode_depth.py` & `taichi-splatting-0.9.0/taichi_splatting/misc/encode_depth.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/misc/indexing.py` & `taichi-splatting-0.9.0/taichi_splatting/misc/indexing.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/misc/parameter_class.py` & `taichi-splatting-0.9.0/taichi_splatting/misc/parameter_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 from functools import cached_property
-from typing import Dict
+from beartype.typing import Dict
 from beartype import beartype
 from beartype.typing import Callable, List, Dict, Optional
 from tensordict import TensorDict
 import torch.optim as optim
 import torch
 
 
@@ -24,16 +24,15 @@
     param_groups: list of parameter dicts, see torch.optim for details 
     param_state: dict of optimizer state to insert into the optimizer
   """
 
   def __init__(self, tensors:TensorDict, param_groups:List, param_state:Optional[Dict]=None):
 
     self.tensors = tensors
-    self.optimizer = optim.Adam(param_groups, foreach=True)
-    self.state_keys = ("exp_avg", "exp_avg_sq")
+    self.optimizer = optim.Adam(param_groups, foreach=True, betas=(0.7, 0.999))
 
     if param_state is not None:
       for k, v in param_state.items():
         self.optimizer.state[self.tensors[k]] = v
 
 
   @beartype
@@ -55,58 +54,65 @@
 
 
   def step(self):
     self.optimizer.step()
 
   def keys(self):
     return self.tensors.keys()
-  
 
+  def optimized_keys(self):
+    return {group["name"] for group in self.optimizer.param_groups}
+    
   def items(self):
     return self.tensors.items()
 
 
   def __getattr__(self, name):
     if name  not in self.tensors.keys():
       raise AttributeError(f'ParameterClass has no attribute {name}')
     
     return self.tensors[name]
 
 
+  def to(self, device):
+    return ParameterClass(
+      as_parameters(self.tensors.to(device), self.optimized_keys()), 
+      self.optimizer.param_groups, 
+      self.get_state()
+    )
+
   def to_dict(self):
     return self.tensors.to_dict()
   
   @property
   def batch_size(self):
     return self.tensors.batch_size
 
-  @cached_property
-  def _optimized_keys(self):
-    return {group["name"] for group in self.optimizer.param_groups}
+
     
   def _updated_state(self, f:Callable):
     def modify_state(state):
-      return {k : f(v) if k in self.state_keys else state[k]
+      return {k : f(v) if torch.is_tensor(v) and v.dim() > 0 else state[k]
                 for k, v in state.items()}
 
     return {name:modify_state(self.optimizer.state[param])
               for name, param in self.tensors.items()
                 if param in self.optimizer.state}
     
 
   def get_state(self):
     return self._updated_state(lambda x: x)
 
 
   def _updated_tensors(self, tensors):
-    params = as_parameters(tensors, self._optimized_keys)
-    updated_groups = [ replace_dict(group, params=[params[group["name"]]])
+    tensors = as_parameters(tensors, self.optimized_keys())
+    updated_groups = [ replace_dict(group, params=[tensors[group["name"]]])
       for group in self.optimizer.param_groups]
     
-    return replace_dict(tensors, **params), updated_groups
+    return tensors, updated_groups
 
   def __getitem__(self, idx):
     tensors, updated_groups = self._updated_tensors(self.tensors[idx])
     state = self._updated_state(lambda x: x[idx])
     return ParameterClass(tensors, updated_groups, state)
   
   def append_tensors(self, tensors):
@@ -123,17 +129,18 @@
         torch.cat([self.tensors, params.tensors]))
     
     state = concat_states(self.get_state(), params.get_state())
     return ParameterClass(tensors, updated_groups, state)
 
 
 def as_parameters(tensors, keys):
-    param_dict = {k: torch.nn.Parameter(x, requires_grad=True) 
-                        for k, x in tensors.items()
-                        if k in keys}
+    param_dict = {
+      k: torch.nn.Parameter(x.detach(), requires_grad=True) 
+            if k in keys else x 
+        for k, x in tensors.items()}
 
     cls = type(tensors)
     return cls.from_dict(param_dict) 
 
 
 def replace_dict(d, **kwargs):
   d = copy.copy(d)
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/misc/renderer2d.py` & `taichi-splatting-0.9.0/taichi_splatting/misc/renderer2d.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/perspective/culling.py` & `taichi-splatting-0.9.0/taichi_splatting/perspective/culling.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/perspective/params.py` & `taichi-splatting-0.9.0/taichi_splatting/perspective/params.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/perspective/plane_culling.py` & `taichi-splatting-0.9.0/taichi_splatting/perspective/plane_culling.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/perspective/projection.py` & `taichi-splatting-0.9.0/taichi_splatting/perspective/projection.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 from beartype.typing import Tuple
 from beartype import beartype
 import taichi as ti
 import torch
 from taichi_splatting.misc.autograd import restore_grad
 
 from .params import CameraParams
-from taichi_splatting.taichi_lib.generic import make_library
+from taichi_splatting.taichi_lib import get_library
 from taichi_splatting.taichi_lib.conversions import torch_taichi
 
+# Ignore this from taichi/pytorch integration 
+# taichi/lang/kernel_impl.py:763: UserWarning: The .grad attribute of a Tensor 
+# that is not a leaf Tensor is being accessed. Its .grad attribute won't be populated 
+# during autograd.backward()
+
+import warnings
+warnings.filterwarnings('ignore', '(.*)that is not a leaf Tensor is being accessed(.*)') 
+
 
 @cache
 def project_to_image_function(torch_dtype=torch.float32, 
                               blur_cov:float = 0.3):
   dtype = torch_taichi[torch_dtype]
 
-  lib = make_library(dtype)
+  lib = get_library(dtype)
   Gaussian3D, Gaussian2D = lib.Gaussian3D, lib.Gaussian2D
 
 
 
   @ti.kernel
   def project_perspective_kernel(  
     gaussians: ti.types.ndarray(Gaussian3D.vec, ndim=1),  # (N, 3 + feature_vec.n1) # input
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/rasterizer/backward.py` & `taichi-splatting-0.9.0/taichi_splatting/rasterizer/backward.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from functools import cache
 import taichi as ti
 from taichi_splatting.data_types import RasterConfig
 from taichi_splatting.rasterizer import tiling
-from taichi_splatting.taichi_lib.concurrent import add, block_reduce_i32, is_warp_leader, warp_add_vector, warp_reduce_f32
+from taichi_splatting.taichi_lib.concurrent import block_reduce_i32, warp_add_vector
 
 from taichi_splatting.taichi_lib.f32 import conic_pdf_with_grad, Gaussian2D
 from taichi.math import ivec2, vec2
 
 
 @cache
 def backward_kernel(config: RasterConfig,
                     points_requires_grad: bool,
                     features_requires_grad: bool, 
-                    compute_weight: bool,
+                    compute_split_heuristics: bool,
                     feature_size: int):
   
 
   feature_vec = ti.types.vector(feature_size, dtype=ti.f32)
   tile_size = config.tile_size
   tile_area = tile_size * tile_size
 
   thread_pixels = config.pixel_stride[0] * config.pixel_stride[1]
   block_area = tile_area // thread_pixels
+  
 
   # each thread is responsible for a small tile of pixels
   pixel_tile = tuple([ (i, 
             (i % config.pixel_stride[0],
             i // config.pixel_stride[0]))
               for i in range(thread_pixels) ])
 
@@ -52,15 +53,15 @@
       # input gradients
       grad_image_feature: ti.types.ndarray(feature_vec, ndim=2),  # (H, W, F)
 
       # output gradients
       grad_points: ti.types.ndarray(Gaussian2D.vec, ndim=1),  # (M, 6)
       grad_features: ti.types.ndarray(feature_vec, ndim=1),  # (M, F)
 
-      point_weight: ti.types.ndarray(ti.f32, ndim=1),  # (M)
+      point_split_heuristics: ti.types.ndarray(vec2, ndim=1),  # (M)
   ):
 
     camera_height, camera_width = image_feature.shape
 
     # round up
     tiles_wide = (camera_width + tile_size - 1) // tile_size 
     tiles_high = (camera_height + tile_size - 1) // tile_size
@@ -74,34 +75,36 @@
 
       # open the shared memory
       tile_point_id = ti.simt.block.SharedArray((block_area, ), dtype=ti.i32)
       tile_point = ti.simt.block.SharedArray((block_area, ), dtype=Gaussian2D.vec)
       tile_feature = ti.simt.block.SharedArray((block_area, ), dtype=feature_vec)
 
       tile_grad_point = (ti.simt.block.SharedArray((block_area, ), dtype=Gaussian2D.vec)
-        if points_requires_grad else None)
+        if ti.static(points_requires_grad) else None)
       
       tile_grad_feature = (ti.simt.block.SharedArray((block_area,), dtype=feature_vec)
-        if features_requires_grad else None)
+        if ti.static(features_requires_grad) else None)
 
-      tile_weight = (ti.simt.block.SharedArray((block_area,), dtype=ti.f32) 
-        if compute_weight else None)
+      tile_split_heuristics = (ti.simt.block.SharedArray((block_area,), dtype=ti.math.vec2) 
+        if ti.static(compute_split_heuristics) else None)
 
       
       last_point_pixel = thread_index(0)
       T_i = thread_vector(1.0)
       grad_pixel_feature = thread_features(0.0)
+      #pixel_feature = thread_features(0.0)
 
       for i, offset in ti.static(pixel_tile):
         pixel = ivec2(offset) + pixel_base
 
         if pixel.y < camera_height and pixel.x < camera_width:
           last_point_pixel[i] = image_last_valid[pixel.y, pixel.x]
           T_i[i] = 1.0 - image_alpha[pixel.y, pixel.x]
           grad_pixel_feature[i, :] = grad_image_feature[pixel.y, pixel.x]
+          #pixel_feature[i, :] = image_feature[pixel.y, pixel.x]
 
       last_point_thread = last_point_pixel.max()
       w_i = thread_features(0.0)
 
       #  T_i = \prod_{j=1}^{i-1} (1 - a_j) \\
       #  \frac{dC}{da_i} = c_i T(i) - \frac{1}{1 - a_i} \\
       #  \sum_{j=i+1}^{n} c_j a_j T(j) \\
@@ -116,17 +119,16 @@
       start_offset, _ = tile_overlap_ranges[tile_id]
       tile_point_count = end_offset - start_offset
 
       num_point_groups = (tile_point_count + ti.static(block_area - 1)) // block_area
 
       # Loop through the range in groups of block_area
       for point_group_id in range(num_point_groups):
-
         ti.simt.block.sync() 
-
+        
         # load points and features into block shared memory
         group_offset_base = point_group_id * block_area
 
         block_end_idx = end_offset - group_offset_base
         block_start_idx = ti.max(block_end_idx - block_area, 0)
 
         load_index = block_end_idx - tile_idx - 1
@@ -139,35 +141,35 @@
 
           if ti.static(points_requires_grad):
             tile_grad_point[tile_idx] = Gaussian2D.vec(0.0)
 
           if ti.static(features_requires_grad):
             tile_grad_feature[tile_idx] = feature_vec(0.0)
           
-          if ti.static(compute_weight):
-            tile_weight[tile_idx] = 0.0
+          if ti.static(compute_split_heuristics):
+            tile_split_heuristics[tile_idx] = vec2(0.0)
 
         ti.simt.block.sync()
 
         point_group_size = ti.min(
           block_area, tile_point_count - group_offset_base)
                     
         for in_group_idx in range(point_group_size):
           point_index = end_offset - (group_offset_base + in_group_idx)
 
-          if not ti.simt.warp.any_nonzero(ti.u32(0xffffffff), ti.i32(point_index <= last_point_thread)):
-            continue
+          # if not ti.simt.warp.any_nonzero(ti.u32(0xffffffff), ti.i32(point_index <= last_point_thread)):
+          #   continue
 
           # Could factor this out and only compute grad if needed
           # however, it does not seem to make any difference
           uv, uv_conic, point_alpha = Gaussian2D.unpack(tile_point[in_group_idx])
 
           grad_point = Gaussian2D.vec(0.0)
           grad_feature = feature_vec(0.0)
-          weight = 0.0
+          contribution = vec2(0.0)
 
           has_grad = False
           for i, offset in ti.static(pixel_tile):
             pixel = ti.cast(pixel_base, ti.f32) + vec2(offset) + 0.5
 
             gaussian_alpha, dp_dmean, dp_dconic = conic_pdf_with_grad(pixel, uv, uv_conic)
             
@@ -179,60 +181,65 @@
               alpha = ti.min(alpha, ti.static(config.clamp_max_alpha))
               T_i[i] /= (1. - alpha)
 
               feature = tile_feature[in_group_idx]
               weight = alpha * T_i[i]
 
               grad_feature += weight * grad_pixel_feature[i, :]
+              feature_diff = (feature * T_i[i] - w_i[i, :] / (1. - alpha))
+              
+  
+              # \frac{dC}{da_i} = c_i T(i) - \frac{1}{1 - a_i} w_i
+              alpha_grad_from_feature = feature_diff * grad_pixel_feature[i, :]
 
-              if ti.static(points_requires_grad):
-                # \frac{dC}{da_i} = c_i T(i) - \frac{1}{1 - a_i} w_i
-                alpha_grad_from_feature = (feature * T_i[i] - w_i[i, :] / (1. - alpha)
-                                          ) * grad_pixel_feature[i, :]
-
-                # w_{i-1} = w_i + c_i a_i T(i)
-                w_i[i, :] += feature * weight
-                alpha_grad: ti.f32 = alpha_grad_from_feature.sum()
-
-                grad_point += alpha_grad * Gaussian2D.to_vec(
-                    point_alpha * dp_dmean, 
-                    point_alpha * dp_dconic,
-                    gaussian_alpha)
-
-
+              # w_{i-1} = w_i + c_i a_i T(i)
+              w_i[i, :] += feature * weight
+              alpha_grad: ti.f32 = alpha_grad_from_feature.sum()
+
+              grad_point += alpha_grad * Gaussian2D.to_vec(
+                  point_alpha * dp_dmean, 
+                  point_alpha * dp_dconic,
+                  gaussian_alpha)
+
+
+              if ti.static(compute_split_heuristics):
+                contribution += vec2(
+                  # (((pixel_feature[i, :] - feature) * weight)**2).sum(),
+                  (feature_diff**2).sum() * weight,
+                  # ((alpha_grad_from_feature)**2).sum()
+                  ti.abs(alpha_grad * point_alpha * dp_dmean).sum()
+                )
 
           if ti.simt.warp.any_nonzero(ti.u32(0xffffffff), ti.i32(has_grad)):
 
             # Accumulating gradients in block shared memory does not appear to be faster
             # on it's own, but combined with warp sums it seems to be fast
             if ti.static(points_requires_grad):
               warp_add_vector(tile_grad_point[in_group_idx], grad_point)
             
             if ti.static(features_requires_grad):
               warp_add_vector(tile_grad_feature[in_group_idx], grad_feature)
 
-            if ti.static(compute_weight):
-              weight = warp_reduce_f32(weight, add)
-              if is_warp_leader():
-                ti.atomic_add(tile_weight[in_group_idx], weight)
+            if ti.static(compute_split_heuristics):
+              warp_add_vector(tile_split_heuristics[in_group_idx], contribution)
         # end of point group loop
 
         ti.simt.block.sync()
 
         # finally accumulate gradients in global memory
         if load_index >= block_start_idx:
           point_offset = tile_point_id[tile_idx] 
           if ti.static(points_requires_grad):
             ti.atomic_add(grad_points[point_offset], tile_grad_point[tile_idx])
 
           if ti.static(features_requires_grad):
             ti.atomic_add(grad_features[point_offset], tile_grad_feature[tile_idx])
 
-          if ti.static(compute_weight):
-            ti.atomic_add(point_weight[point_offset], tile_weight[tile_idx])
+          if ti.static(compute_split_heuristics):
+            ti.atomic_add(point_split_heuristics[point_offset], tile_split_heuristics[tile_idx])
 
       # end of point group id loop
     # end of pixel loop
 
   return _backward_kernel
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/rasterizer/forward.py` & `taichi-splatting-0.9.0/taichi_splatting/rasterizer/forward.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/rasterizer/function.py` & `taichi-splatting-0.9.0/taichi_splatting/rasterizer/function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 
 from functools import cache
-from typing import Optional
-from taichi_splatting.misc.autograd import restore_grad
 from taichi_splatting.mapper.tile_mapper import map_to_tiles
-# from taichi_splatting.mapper.segmented_tile_mapper import map_to_tiles
 
 
 from .forward import RasterConfig, forward_kernel
 from .backward import backward_kernel
 
 from numbers import Integral
 from beartype.typing import Tuple, NamedTuple
@@ -15,92 +12,90 @@
 import torch
 from beartype import beartype
 
 
 RasterOut = NamedTuple('RasterOut', 
     [('image', torch.Tensor), 
      ('image_weight', torch.Tensor),
-     ('point_weight', torch.Tensor) ])
+     ('point_split_heuristics', torch.Tensor) ])
 
 @cache
 def render_function(config:RasterConfig,
                     points_requires_grad:bool,
                     features_requires_grad:bool, 
-                    compute_weight:bool,
+                    compute_split_heuristics:bool,
                     feature_size:int):
   
     
   forward = forward_kernel(config, feature_size=feature_size)
   backward = backward_kernel(config, points_requires_grad,
                              features_requires_grad, 
-                             compute_weight, feature_size)
+                             compute_split_heuristics, feature_size)
 
   class _module_function(torch.autograd.Function):
     @staticmethod
     def forward(ctx, gaussians: torch.Tensor, features: torch.Tensor,
                 overlap_to_point: torch.Tensor, tile_overlap_ranges: torch.Tensor,
                 image_size: Tuple[Integral, Integral]
                 ) -> torch.Tensor:
         
       shape = (image_size[1], image_size[0])
       image_feature = torch.empty((*shape, features.shape[1]),
                                   dtype=torch.float32, device=features.device)
       image_alpha = torch.empty(shape, dtype=torch.float32, device=features.device)
       image_last_valid = torch.empty(shape, dtype=torch.int32, device=features.device)
 
-      point_weight = torch.zeros(gaussians.shape[0] if compute_weight else 0, 
+      point_split_heuristics = torch.zeros( (gaussians.shape[0], 2) if compute_split_heuristics else (0, 2), 
                                  dtype=torch.float32, device=features.device)
 
       forward(gaussians, features, 
         tile_overlap_ranges, overlap_to_point,
         image_feature, image_alpha, image_last_valid)
 
       # Non differentiable parameters
       ctx.overlap_to_point = overlap_to_point
       ctx.tile_overlap_ranges = tile_overlap_ranges
       ctx.image_last_valid = image_last_valid
       ctx.image_alpha = image_alpha
       ctx.image_size = image_size
-      ctx.point_weight = point_weight
-
-      ctx.mark_non_differentiable(image_alpha, image_last_valid)
-      ctx.mark_non_differentiable(point_weight)
+      ctx.point_split_heuristics = point_split_heuristics
 
+      ctx.mark_non_differentiable(image_alpha, image_last_valid, point_split_heuristics, overlap_to_point, tile_overlap_ranges)
       ctx.save_for_backward(gaussians, features, image_feature)
             
-      return image_feature, image_alpha, point_weight
+      return image_feature, image_alpha, point_split_heuristics
 
     @staticmethod
     def backward(ctx, grad_image_feature:torch.Tensor, 
-                 grad_alpha:torch.Tensor, grad_point_weight:torch.Tensor):
+                 grad_alpha:torch.Tensor, grad_point_split_heuristics:torch.Tensor):
         gaussians, features, image_feature = ctx.saved_tensors
 
         grad_gaussians = torch.zeros_like(gaussians)
         grad_features = torch.zeros_like(features)
   
-        with restore_grad(grad_gaussians, grad_features):
+        # with restore_grad(gaussians, features):
 
-          backward(gaussians, features, 
-            ctx.tile_overlap_ranges, ctx.overlap_to_point,
-            image_feature, ctx.image_alpha, ctx.image_last_valid,
-            grad_image_feature.contiguous(),
-            grad_gaussians, grad_features, ctx.point_weight)
+        backward(gaussians, features, 
+          ctx.tile_overlap_ranges, ctx.overlap_to_point,
+          image_feature, ctx.image_alpha, ctx.image_last_valid,
+          grad_image_feature.contiguous(),
+          grad_gaussians, grad_features, ctx.point_split_heuristics)
 
-          return grad_gaussians, grad_features, None, None, None, None
+        return grad_gaussians, grad_features, None, None, None, None
   return _module_function
 
 
 
 
 
 @beartype
 def rasterize_with_tiles(gaussians2d: torch.Tensor, features: torch.Tensor,
               overlap_to_point: torch.Tensor, tile_overlap_ranges: torch.Tensor,
               image_size: Tuple[Integral, Integral], config: RasterConfig,
-              compute_weight:bool=False
+              compute_split_heuristics:bool=False
               ) -> RasterOut:
   """
   Rasterize an image given 2d gaussians, features and tile overlap information.
   Consider using rasterize instead to also compute tile overlap information.
 
   Parameters:
       gaussians2d: (N, 6)  packed gaussians, N is the number of gaussians
@@ -109,61 +104,61 @@
       tile_overlap_ranges: (TH * TW, 2) M is the number of tiles, 
         maps tile index to range of overlap indices (0..K]
       overlap_to_point: (K, )  K is the number of overlaps, 
         maps overlap index to point index (0..N]
 
       image_size: (2, ) tuple of ints, (width, height)
       config: Config - configuration parameters for rasterization
-      compute_weight: bool - whether to compute the visibility for each point in the image
+      compute_split_heuristics: bool - whether to compute the visibility for each point in the image
 
     Returns:
       RasterOut - namedtuple with fields:
         image: (H, W, F) torch tensor, where H, W are the image height and width, F is the number of features
         image_weight: (H, W) torch tensor, where H, W are the image height and width
-        point_weight: (N, ) torch tensor, where N is the number of gaussians  
+        point_split_heuristics: (N, ) torch tensor, where N is the number of gaussians  
   """
   _module_function = render_function(config, gaussians2d.requires_grad,
                                       features.requires_grad,
-                                      compute_weight, 
+                                      compute_split_heuristics, 
                                       features.shape[1])
 
-  image, image_weight, point_weight = _module_function.apply(gaussians2d, features, 
+  image, image_weight, point_split_heuristics = _module_function.apply(gaussians2d, features, 
           overlap_to_point, tile_overlap_ranges, 
           image_size)
   
-  return RasterOut(image, image_weight, point_weight)
+  return RasterOut(image, image_weight, point_split_heuristics)
 
 
 def rasterize(gaussians2d:torch.Tensor, encoded_depths:torch.Tensor, 
                           features:torch.Tensor, image_size:Tuple[Integral, Integral],
-                          config:RasterConfig, compute_weight:bool=False) -> RasterOut:
+                          config:RasterConfig, compute_split_heuristics:bool=False) -> RasterOut:
     
     
   """
   Rasterize an image given 2d gaussians, features. 
 
   Parameters:
       gaussians2d: (N, 6)  packed gaussians, N is the number of gaussians
       encoded_depths: (N )  encoded depths, N is the number of gaussians
       features: (N, F)   features, F is the number of features
 
       image_size: (2, ) tuple of ints, (width, height)
       config: Config - configuration parameters for rasterization
-      compute_weight: bool - whether to compute the visibility for each point in the image
+      compute_split_heuristics: bool - whether to compute the visibility for each point in the image
 
     Returns:
       RasterOut - namedtuple with fields:
         image: (H, W, F) torch tensor, where H, W are the image height and width, F is the number of features
         image_weight: (H, W) torch tensor, where H, W are the image height and width
-        point_weight: (N, ) torch tensor, where N is the number of gaussians  
+        point_split_heuristics: (N, ) torch tensor, where N is the number of gaussians  
   """
 
   assert gaussians2d.shape[0] == encoded_depths.shape[0] == features.shape[0], \
     f"Size mismatch: got {gaussians2d.shape}, {encoded_depths.shape}, {features.shape}"
 
   # render with padding to tile_size, later crop back to original size
   overlap_to_point, tile_overlap_ranges = map_to_tiles(gaussians2d, encoded_depths, 
     image_size=image_size, config=config)
   
   return rasterize_with_tiles(gaussians2d, features, 
     tile_overlap_ranges=tile_overlap_ranges.view(-1, 2), overlap_to_point=overlap_to_point,
-    image_size=image_size, config=config, compute_weight=compute_weight)
+    image_size=image_size, config=config, compute_split_heuristics=compute_split_heuristics)
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/rasterizer/tiling.py` & `taichi-splatting-0.9.0/taichi_splatting/rasterizer/tiling.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/spherical_harmonics.py` & `taichi-splatting-0.9.0/taichi_splatting/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/taichi_lib/concurrent.py` & `taichi-splatting-0.9.0/taichi_splatting/taichi_lib/concurrent.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/taichi_lib/conversions.py` & `taichi-splatting-0.9.0/taichi_splatting/taichi_lib/conversions.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/taichi_lib/generic.py` & `taichi-splatting-0.9.0/taichi_splatting/taichi_lib/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,27 @@
   def unpack_vec_g2d(vec:vec_g2d) -> Gaussian2D:
     return vec[0:2], vec[2:5], vec[5]
 
   @ti.func
   def get_position_g3d(vec:vec_g3d) -> vec3:
     return vec[0:3]
 
+  @ti.func
+  def get_position_g2d(vec:vec_g2d) -> vec2:
+    return vec[0:2]
+
+  @ti.func
+  def get_conic_g2d(vec:vec_g2d) -> vec3:
+    return vec[2:5]
+
+
+  @ti.func
+  def get_cov_g2d(vec:vec_g2d) -> vec3:
+    conic = get_conic_g2d(vec)
+    return inverse_cov(conic)
 
   @ti.func
   def from_vec_g3d(vec:vec_g3d) -> Gaussian3D:
     return Gaussian3D(vec[0:3], vec[3:6], vec[6:10], vec[10])
 
   @ti.func
   def from_vec_g2d(vec:vec_g2d) -> Gaussian2D:
@@ -98,14 +111,18 @@
 
   # Taichi structs don't have static methods, but they can be added afterward
   Gaussian2D.vec = vec_g2d
   Gaussian2D.to_vec = to_vec_g2d
   Gaussian2D.from_vec = from_vec_g2d
   Gaussian2D.unpack = unpack_vec_g2d
 
+  Gaussian2D.get_position = get_position_g2d
+  Gaussian2D.get_conic = get_conic_g2d
+  Gaussian2D.get_cov = get_cov_g2d
+
 
   Gaussian3D.vec = vec_g3d
   Gaussian3D.to_vec = to_vec_g3d
   Gaussian3D.from_vec = from_vec_g3d
   Gaussian3D.unpack = unpack_vec_g3d
   Gaussian3D.unpack_activate = unpack_activate_g3d
   Gaussian3D.get_position = get_position_g3d
@@ -281,53 +298,40 @@
 
 
   @ti.func
   def conic_pdf(xy: vec2, uv: vec2, uv_conic: vec3) -> dtype:
       dx, dy = xy - uv
       a, b, c = uv_conic
 
-      p = ti.exp(-0.5 * (dx**2 * a + dy**2 * c) - dx * dy * b)
+      inner = 0.5 * (dx**2 * a + dy**2 * c) + dx * dy * b
+      p = ti.exp(-inner)
       return p
 
 
   @ti.func
   def conic_pdf_with_grad(xy: vec2, uv: vec2, uv_conic: vec3):
       d = xy - uv
       a, b, c = uv_conic
 
       dx2 = d.x**2
       dy2 = d.y**2
       dxdy = d.x * d.y
       
-      p = ti.exp(-0.5 * (dx2 * a + dy2 * c) - dxdy * b)
+      inner = 0.5 * (dx2 * a + dy2 * c) + dxdy * b
+      p = ti.exp(-inner)
+      
       dp_duv = vec2(
-          (b * d.y - 0.5 * a * (2 * uv.x - 2 * xy.x)) * p,
-          (b * d.x - 0.5 * c * (2 * uv.y - 2 * xy.y)) * p
+          (b * d.y + a * d.x) * p,
+          (b * d.x + c * d.y) * p
       )
       dp_dconic = vec3(-0.5 * dx2 * p, -dxdy * p, -0.5 * dy2 * p)
 
       return p, dp_duv, dp_dconic
 
 
-  @ti.func
-  def conic_grad(p: ti.f32, xy: vec2, uv: vec2, uv_conic: vec3):
-      d = xy - uv
-      a, b, c = uv_conic
-
-      dx2 = d.x**2
-      dy2 = d.y**2
-      dxdy = d.x * d.y
-      
-      dp_duv = vec2(
-          (b * d.y - 0.5 * a * (2 * uv.x - 2 * xy.x)) * p,
-          (b * d.x - 0.5 * c * (2 * uv.y - 2 * xy.y)) * p
-      )
-      dp_dconic = vec3(-0.5 * dx2 * p, -dxdy * p, -0.5 * dy2 * p)
-
-      return dp_duv, dp_dconic
 
 
   @ti.func
   def cov_inv_basis(uv_cov: vec3, scale: dtype) -> mat2:
       basis = ti.Matrix.cols(cov_axes(uv_cov))
       return (basis * scale).inverse()
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/taichi_lib/grid_query.py` & `taichi-splatting-0.9.0/taichi_splatting/taichi_lib/grid_query.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/tests/random_data.py` & `taichi-splatting-0.9.0/taichi_splatting/tests/random_data.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/tests/test_conic.py` & `taichi-splatting-0.9.0/taichi_splatting/tests/test_conic.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/tests/test_projection.py` & `taichi-splatting-0.9.0/taichi_splatting/tests/test_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def random_inputs(device='cpu', max_points=1000, dtype=torch.float32):
   def f(seed:int = 0):
     torch.manual_seed(seed)
     camera = random_camera()
     n = torch.randint(size=(1,), low=1, high=max_points).item()
 
     gaussians = random_3d_gaussians(n=n, camera_params=camera)
-    check_finite(gaussians)
+    check_finite(gaussians, 'gaussians')
 
     return (x.to(device=device, dtype=dtype) for x in [gaussians, camera])
   return f
 
 
 def compare(name, x, y, **kwargs):
   if not torch.allclose(x, y, **kwargs):
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/tests/test_spherical_harmonics.py` & `taichi-splatting-0.9.0/taichi_splatting/tests/test_spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/tests/util.py` & `taichi-splatting-0.9.0/taichi_splatting/tests/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 
 
 from beartype.typing import Sequence
 import torch
 from tqdm import tqdm
 
-# Ignore this from taichi/pytorch integration 
-# taichi/lang/kernel_impl.py:763: UserWarning: The .grad attribute of a Tensor 
-# that is not a leaf Tensor is being accessed. Its .grad attribute won't be populated 
-# during autograd.backward()
 
-import warnings
-warnings.filterwarnings('ignore') 
 
 
 def eval_with_grad(f, *args):
   args = [args.detach().clone().requires_grad_(True) for args in args]
 
   # multiply by one to make the argument not a leaf tensor 
   # avoids an issue with taichi/pytorch autograd integration
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting/torch_ops/projection.py` & `taichi-splatting-0.9.0/taichi_splatting/torch_ops/projection.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/torch_ops/rsh.py` & `taichi-splatting-0.9.0/taichi_splatting/torch_ops/rsh.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/torch_ops/spherical_harmonics.py` & `taichi-splatting-0.9.0/taichi_splatting/torch_ops/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting/torch_ops/transforms.py` & `taichi-splatting-0.9.0/taichi_splatting/torch_ops/transforms.py`

 * *Files identical despite different names*

### Comparing `taichi-splatting-0.8.0/taichi_splatting.egg-info/PKG-INFO` & `taichi-splatting-0.9.0/taichi_splatting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taichi-splatting
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Taichi Gaussian Splatting library
 Maintainer-email: Oliver Batchelor <oliver.batchelor@canterbury.ac.nz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,14 +254,22 @@
 
 ## Executables
 
 ### fit_image_gaussians
 
 There exists a toy optimizer for fitting a set of randomly initialized gaussians to some 2D images `fit_image_gaussians` - useful for testing rasterization without the rest of the dependencies.
 
+Fitting an image (fixed points): \
+`fit_image_gaussians <image file> --show  --n 20000` 
+
+Fitting an image (split and prune to target): \
+`fit_image_gaussians <image file> --show --n 1000 --target 20000` 
+
+See `--help` for other options.
+
 ### benchmarks
 
 There exist benchmarks to evaluate performance on individual components in isolation under `taichi_splatting/benchmarks/`
 
 ### tests 
 
 Tests (gradient tests and tests comparing to torch-based reference implementations) can be run with pytest, or individually under 
@@ -289,15 +297,15 @@
 * Spherical harmonics with autograd
 * Gradient tests for most parts (float64)
 * Fit to image training example/test
 * Depth and depth-covariance rendering
 
 * Compute point visibility in backward pass (useful for model pruning)
 * Example training on images with split/prune operations
-
+* Novel heuristics for split and prune operations computed optionally in backward pass 
 
 
 ### Todo
 
 * Depth covariance example
 
 * 3D training code (likely different repository)
```

### Comparing `taichi-splatting-0.8.0/taichi_splatting.egg-info/SOURCES.txt` & `taichi-splatting-0.9.0/taichi_splatting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 taichi_splatting/mapper/tile_mapper.py
 taichi_splatting/misc/__init__.py
 taichi_splatting/misc/autograd.py
 taichi_splatting/misc/depth_variance.py
 taichi_splatting/misc/encode_depth.py
 taichi_splatting/misc/indexing.py
 taichi_splatting/misc/parameter_class.py
+taichi_splatting/misc/radius.py
 taichi_splatting/misc/renderer2d.py
 taichi_splatting/perspective/__init__.py
 taichi_splatting/perspective/culling.py
 taichi_splatting/perspective/params.py
 taichi_splatting/perspective/plane_culling.py
 taichi_splatting/perspective/projection.py
 taichi_splatting/rasterizer/__init__.py
```

