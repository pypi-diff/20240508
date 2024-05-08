# Comparing `tmp/evnn_pytorch-0.1.0.tar.gz` & `tmp/evnn_pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evnn_pytorch-0.1.0.tar", last modified: Sat Mar 18 10:09:59 2023, max compression
+gzip compressed data, was "evnn_pytorch-0.2.0.tar", last modified: Wed May  8 14:17:08 2024, max compression
```

## Comparing `evnn_pytorch-0.1.0.tar` & `evnn_pytorch-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.169053 evnn_pytorch-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2510 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     6649 2023-03-18 10:09:59.168053 evnn_pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5653 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.167053 evnn_pytorch-0.1.0/evnn_pytorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6649 2023-03-18 10:09:59.000000 evnn_pytorch-0.1.0/evnn_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      596 2023-03-18 10:09:59.000000 evnn_pytorch-0.1.0/evnn_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-18 10:09:59.000000 evnn_pytorch-0.1.0/evnn_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-18 10:09:59.000000 evnn_pytorch-0.1.0/evnn_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.166053 evnn_pytorch-0.1.0/frameworks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.167053 evnn_pytorch-0.1.0/frameworks/pytorch/
--rw-r--r--   0 root         (0) root         (0)      972 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-18 10:09:58.000000 evnn_pytorch-0.1.0/frameworks/pytorch/_version.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/base_rnn.py
--rw-r--r--   0 root         (0) root         (0)    14636 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/egru.cc
--rw-r--r--   0 root         (0) root         (0)    17160 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/egru.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/support.cc
--rw-r--r--   0 root         (0) root         (0)     1601 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/frameworks/pytorch/support.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.168053 evnn_pytorch-0.1.0/lib/
--rw-r--r--   0 root         (0) root         (0)     2475 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/blas.h
--rw-r--r--   0 root         (0) root         (0)      999 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/device_assert.h
--rw-r--r--   0 root         (0) root         (0)    14283 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/egru_backward_cpu.cc
--rw-r--r--   0 root         (0) root         (0)    18172 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/egru_backward_gpu.cu.cc
--rw-r--r--   0 root         (0) root         (0)    11838 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/egru_forward_cpu.cc
--rw-r--r--   0 root         (0) root         (0)    15515 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/egru_forward_gpu.cu.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 10:09:59.168053 evnn_pytorch-0.1.0/lib/evnn/
--rw-r--r--   0 root         (0) root         (0)    12716 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/evnn/egru.h
--rw-r--r--   0 root         (0) root         (0)    12300 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/evnn/egru_cpu.h
--rw-r--r--   0 root         (0) root         (0)     1288 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/evnn.h
--rw-r--r--   0 root         (0) root         (0)     4093 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/lib/inline_ops.h
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-18 10:09:59.169053 evnn_pytorch-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4266 2023-03-18 10:09:56.000000 evnn_pytorch-0.1.0/setup.py
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    11357 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/LICENSE
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)      117 2024-05-02 13:54:41.000000 evnn_pytorch-0.2.0/MANIFEST.in
+-rw-r--r--   0 kkhan     (1019) kkhan     (1019)     6790 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/PKG-INFO
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     5839 2024-05-08 11:29:21.000000 evnn_pytorch-0.2.0/README.md
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/
+-rw-r--r--   0 kkhan     (1019) kkhan     (1019)     6790 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)      616 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)        1 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)        6 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)       30 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/evnn_pytorch.egg-info/top_level.txt
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/frameworks/
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/frameworks/pytorch/
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)      972 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/frameworks/pytorch/__init__.py
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)       21 2024-05-08 14:17:08.000000 evnn_pytorch-0.2.0/frameworks/pytorch/_version.py
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     4389 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/frameworks/pytorch/base_rnn.py
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    14636 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/frameworks/pytorch/egru.cc
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    17521 2024-05-02 12:19:07.000000 evnn_pytorch-0.2.0/frameworks/pytorch/egru.py
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)      926 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/frameworks/pytorch/support.cc
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     1601 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/frameworks/pytorch/support.h
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/lib/
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     2475 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/blas.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)      999 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/device_assert.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    14283 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/egru_backward_cpu.cc
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    18172 2024-05-02 13:54:56.000000 evnn_pytorch-0.2.0/lib/egru_backward_gpu.cu
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    11838 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/egru_forward_cpu.cc
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    15515 2024-05-02 13:54:56.000000 evnn_pytorch-0.2.0/lib/egru_forward_gpu.cu
+drwxrwxr-x   0 kkhan     (1019) kkhan     (1019)        0 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/lib/evnn/
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    12716 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/evnn/egru.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)    12300 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/evnn/egru_cpu.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     1288 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/evnn.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     4093 2024-04-30 16:18:46.000000 evnn_pytorch-0.2.0/lib/inline_ops.h
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)       38 2024-05-08 14:17:08.722561 evnn_pytorch-0.2.0/setup.cfg
+-rw-rw-r--   0 kkhan     (1019) kkhan     (1019)     5062 2024-05-08 12:56:41.000000 evnn_pytorch-0.2.0/setup.py
```

### Comparing `evnn_pytorch-0.1.0/LICENSE` & `evnn_pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/PKG-INFO` & `evnn_pytorch-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: evnn_pytorch
-Version: 0.1.0
+Version: 0.2.0
 Summary: EVNN: a torch extension for custom event based RNN models.
 Home-page: https://tu-dresden.de/ing/elektrotechnik/iee/hpsn
 Author: TUD and RUB
 Author-email: khaleelulla.khan_nazeer@tu-dresden.de
 License: Apache 2.0
 Keywords: pytorch machine learning rnn lstm gru custom op
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
 
 # EvNN: Event-based Neural Networks
 
 EvNN is a CUDA and C++ implementation of event-based RNN layers with built-in [DropConnect](http://proceedings.mlr.press/v28/wan13.html) and [Zoneout](https://arxiv.org/abs/1606.01305) regularization. These layers are exposed through C++ and Pytorch APIs for easy integration into your own projects or machine learning frameworks. The code framework and base layers are adopted from [Haste](https://github.com/lmnt-com/haste/) Library.
 
 ## EGRU: Event-based Gated Recurrent Unit
 
@@ -48,46 +47,50 @@
 What's included in this project?
 - a PyTorch API (`evnn_pytorch`) for event based neural networks
 
 
 ## Install
 Here's what you'll need to get started:
 - a [CUDA Compute Capability](https://developer.nvidia.com/cuda-gpus) 3.7+ GPU (required only if using GPU)
-- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 10.0+ (required only if using GPU)
+- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.0+ (required only if using GPU)
 - [PyTorch](https://pytorch.org) 1.3+ for PyTorch integration (GPU optional)
-- [BLAS](https://netlib.org/blas/) or any BLAS-like library for CPU computation.
-- [Eigen 3](http://eigen.tuxfamily.org/) to build the C++ examples (optional)
+- [OpenBLAS](https://www.openblas.net/) or any BLAS-like library for CPU computation.
 
 Once you have the prerequisites, you can install with pip or by building the source code.
 
 <!-- ### Using pip
 ```
 pip install evnn_pytorch
 ``` -->
 
 ### Building from source
 > **Note**
 > 
 > Currenty supported only on Linux, use Docker for building on Windows.
 
+Build and install it with `pip`:
 ```bash
-make evnn_pytorch # Build PyTorch API
+pip install .
 ```
+### Building in Docker
 
-If you built the PyTorch API, install it with `pip`:
+Build docker image:
 ```bash
-pip install evnn_pytorch-*.whl
+docker build -t evnn -f docker/Dockerfile .
 ```
 
-If the CUDA Toolkit that you're building against is not in `/usr/local/cuda`, you must specify the
-`$CUDA_HOME` environment variable before running make:
+Example usage:
 ```bash
-CUDA_HOME=/usr/local/cuda-10.2 make
+docker run --rm --gpus=all evnn python -m unittest discover -p "*_test.py" -s /evnn_src/validation -v
 ```
 
+> **Note**
+> 
+> The build script tries to automatically detect GPU compute capability. In case the GPU is not available during compilation, for example when building with docker or when using compute cluster login nodes for compiling, Use enviroment variable `EVNN_CUDA_COMPUTE` to set the required compute capability.
+
 ## Performance
 
 Code for the experiments and benchmarks presented in the paper are published in ``benchmarks`` directory.
 Note that these benchmarks have additional dependencies as documented in `benchmarks/requirements.txt`
 
 ## Documentation
```

### Comparing `evnn_pytorch-0.1.0/README.md` & `evnn_pytorch-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,46 +24,50 @@
 What's included in this project?
 - a PyTorch API (`evnn_pytorch`) for event based neural networks
 
 
 ## Install
 Here's what you'll need to get started:
 - a [CUDA Compute Capability](https://developer.nvidia.com/cuda-gpus) 3.7+ GPU (required only if using GPU)
-- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 10.0+ (required only if using GPU)
+- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.0+ (required only if using GPU)
 - [PyTorch](https://pytorch.org) 1.3+ for PyTorch integration (GPU optional)
-- [BLAS](https://netlib.org/blas/) or any BLAS-like library for CPU computation.
-- [Eigen 3](http://eigen.tuxfamily.org/) to build the C++ examples (optional)
+- [OpenBLAS](https://www.openblas.net/) or any BLAS-like library for CPU computation.
 
 Once you have the prerequisites, you can install with pip or by building the source code.
 
 <!-- ### Using pip
 ```
 pip install evnn_pytorch
 ``` -->
 
 ### Building from source
 > **Note**
 > 
 > Currenty supported only on Linux, use Docker for building on Windows.
 
+Build and install it with `pip`:
 ```bash
-make evnn_pytorch # Build PyTorch API
+pip install .
 ```
+### Building in Docker
 
-If you built the PyTorch API, install it with `pip`:
+Build docker image:
 ```bash
-pip install evnn_pytorch-*.whl
+docker build -t evnn -f docker/Dockerfile .
 ```
 
-If the CUDA Toolkit that you're building against is not in `/usr/local/cuda`, you must specify the
-`$CUDA_HOME` environment variable before running make:
+Example usage:
 ```bash
-CUDA_HOME=/usr/local/cuda-10.2 make
+docker run --rm --gpus=all evnn python -m unittest discover -p "*_test.py" -s /evnn_src/validation -v
 ```
 
+> **Note**
+> 
+> The build script tries to automatically detect GPU compute capability. In case the GPU is not available during compilation, for example when building with docker or when using compute cluster login nodes for compiling, Use enviroment variable `EVNN_CUDA_COMPUTE` to set the required compute capability.
+
 ## Performance
 
 Code for the experiments and benchmarks presented in the paper are published in ``benchmarks`` directory.
 Note that these benchmarks have additional dependencies as documented in `benchmarks/requirements.txt`
 
 ## Documentation
```

### Comparing `evnn_pytorch-0.1.0/evnn_pytorch.egg-info/PKG-INFO` & `evnn_pytorch-0.2.0/evnn_pytorch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
-Name: evnn-pytorch
-Version: 0.1.0
+Name: evnn_pytorch
+Version: 0.2.0
 Summary: EVNN: a torch extension for custom event based RNN models.
 Home-page: https://tu-dresden.de/ing/elektrotechnik/iee/hpsn
 Author: TUD and RUB
 Author-email: khaleelulla.khan_nazeer@tu-dresden.de
 License: Apache 2.0
 Keywords: pytorch machine learning rnn lstm gru custom op
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
 
 # EvNN: Event-based Neural Networks
 
 EvNN is a CUDA and C++ implementation of event-based RNN layers with built-in [DropConnect](http://proceedings.mlr.press/v28/wan13.html) and [Zoneout](https://arxiv.org/abs/1606.01305) regularization. These layers are exposed through C++ and Pytorch APIs for easy integration into your own projects or machine learning frameworks. The code framework and base layers are adopted from [Haste](https://github.com/lmnt-com/haste/) Library.
 
 ## EGRU: Event-based Gated Recurrent Unit
 
@@ -48,46 +47,50 @@
 What's included in this project?
 - a PyTorch API (`evnn_pytorch`) for event based neural networks
 
 
 ## Install
 Here's what you'll need to get started:
 - a [CUDA Compute Capability](https://developer.nvidia.com/cuda-gpus) 3.7+ GPU (required only if using GPU)
-- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 10.0+ (required only if using GPU)
+- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.0+ (required only if using GPU)
 - [PyTorch](https://pytorch.org) 1.3+ for PyTorch integration (GPU optional)
-- [BLAS](https://netlib.org/blas/) or any BLAS-like library for CPU computation.
-- [Eigen 3](http://eigen.tuxfamily.org/) to build the C++ examples (optional)
+- [OpenBLAS](https://www.openblas.net/) or any BLAS-like library for CPU computation.
 
 Once you have the prerequisites, you can install with pip or by building the source code.
 
 <!-- ### Using pip
 ```
 pip install evnn_pytorch
 ``` -->
 
 ### Building from source
 > **Note**
 > 
 > Currenty supported only on Linux, use Docker for building on Windows.
 
+Build and install it with `pip`:
 ```bash
-make evnn_pytorch # Build PyTorch API
+pip install .
 ```
+### Building in Docker
 
-If you built the PyTorch API, install it with `pip`:
+Build docker image:
 ```bash
-pip install evnn_pytorch-*.whl
+docker build -t evnn -f docker/Dockerfile .
 ```
 
-If the CUDA Toolkit that you're building against is not in `/usr/local/cuda`, you must specify the
-`$CUDA_HOME` environment variable before running make:
+Example usage:
 ```bash
-CUDA_HOME=/usr/local/cuda-10.2 make
+docker run --rm --gpus=all evnn python -m unittest discover -p "*_test.py" -s /evnn_src/validation -v
 ```
 
+> **Note**
+> 
+> The build script tries to automatically detect GPU compute capability. In case the GPU is not available during compilation, for example when building with docker or when using compute cluster login nodes for compiling, Use enviroment variable `EVNN_CUDA_COMPUTE` to set the required compute capability.
+
 ## Performance
 
 Code for the experiments and benchmarks presented in the paper are published in ``benchmarks`` directory.
 Note that these benchmarks have additional dependencies as documented in `benchmarks/requirements.txt`
 
 ## Documentation
```

### Comparing `evnn_pytorch-0.1.0/evnn_pytorch.egg-info/SOURCES.txt` & `evnn_pytorch-0.2.0/evnn_pytorch.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 LICENSE
 MANIFEST.in
-Makefile
 README.md
 setup.py
 evnn_pytorch.egg-info/PKG-INFO
 evnn_pytorch.egg-info/SOURCES.txt
 evnn_pytorch.egg-info/dependency_links.txt
+evnn_pytorch.egg-info/requires.txt
 evnn_pytorch.egg-info/top_level.txt
 frameworks/pytorch/__init__.py
 frameworks/pytorch/_version.py
 frameworks/pytorch/base_rnn.py
 frameworks/pytorch/egru.cc
 frameworks/pytorch/egru.py
 frameworks/pytorch/support.cc
 frameworks/pytorch/support.h
 lib/blas.h
 lib/device_assert.h
 lib/egru_backward_cpu.cc
-lib/egru_backward_gpu.cu.cc
+lib/egru_backward_gpu.cu
 lib/egru_forward_cpu.cc
-lib/egru_forward_gpu.cu.cc
+lib/egru_forward_gpu.cu
 lib/evnn.h
 lib/inline_ops.h
 lib/evnn/egru.h
 lib/evnn/egru_cpu.h
```

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/__init__.py` & `evnn_pytorch-0.2.0/frameworks/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/base_rnn.py` & `evnn_pytorch-0.2.0/frameworks/pytorch/base_rnn.py`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/egru.cc` & `evnn_pytorch-0.2.0/frameworks/pytorch/egru.cc`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/egru.py` & `evnn_pytorch-0.2.0/frameworks/pytorch/egru.py`

 * *Files 6% similar despite different names*

```diff
@@ -243,15 +243,16 @@
                  input_size,
                  hidden_size,
                  batch_first=False,
                  dropout=0.0,
                  zoneout=0.0,
                  dampening_factor=0.7,
                  pseudo_derivative_support=1.0,
-                 thr_mean=0.0,
+                 thr_mean=0.3,
+                 weight_initialization_gain=1.0,
                  return_state_sequence=False,
                  grad_clip=None,
                  use_custom_cuda=True):
         """
         Initialize the parameters of the GRU layer.
 
         Arguments:
@@ -284,28 +285,34 @@
             raise ValueError('GRU: dropout must be in [0.0, 1.0]')
         if zoneout < 0 or zoneout > 1:
             raise ValueError('GRU: zoneout must be in [0.0, 1.0]')
 
         self.dropout = dropout
         self.alpha = torch.tensor(0.9)
 
+        self.weight_initialization_gain = weight_initialization_gain
+
         self.kernel = nn.Parameter(torch.empty(input_size, hidden_size * 3))
         self.recurrent_kernel = nn.Parameter(
             torch.empty(hidden_size, hidden_size * 3))
         self.bias = nn.Parameter(torch.empty(hidden_size * 3))
         self.recurrent_bias = nn.Parameter(torch.empty(hidden_size * 3))
         self.reset_parameters()
 
         self.dampening_factor = nn.Parameter(
             torch.Tensor([dampening_factor]), requires_grad=False)
         self.pseudo_derivative_support = nn.Parameter(
             torch.Tensor([pseudo_derivative_support]), requires_grad=False)
-        self.thr_reparam = nn.Parameter(torch.normal(torch.zeros(self.hidden_size) + thr_mean,
-                                                     math.sqrt(2) * torch.ones(self.hidden_size)))
-        self.thr = torch.sigmoid(self.thr_reparam)
+
+        # initialize thresholds according to the beta distribution with mean 'thr_mean'
+        assert 0 < thr_mean < 1, f"thr_mean must be between 0 and 1, but {thr_mean} was given"
+        beta = 3
+        alpha = beta * thr_mean / (1 - thr_mean)
+        distribution = torch.distributions.beta.Beta(alpha, beta)
+        self.thr = nn.Parameter(distribution.sample(torch.Size([self.hidden_size])))
 
     def to_native_weights(self):
         """
         Converts EvNN GRU weights to native PyTorch GRU weights.
 
         Returns:
           weight_ih_l0: Parameter, the input-hidden weights of the GRU layer.
@@ -323,15 +330,15 @@
         bias1 = reorder_weights(self.bias).contiguous()
         bias2 = reorder_weights(self.recurrent_bias).contiguous()
 
         kernel = torch.nn.Parameter(kernel)
         recurrent_kernel = torch.nn.Parameter(recurrent_kernel)
         bias1 = torch.nn.Parameter(bias1)
         bias2 = torch.nn.Parameter(bias2)
-        thr = torch.nn.Parameter(self.thr_reparam)
+        thr = torch.nn.Parameter(self.thr)
         return kernel, recurrent_kernel, bias1, bias2, thr
 
     def from_native_weights(self, weight_ih_l0, weight_hh_l0, bias_ih_l0, bias_hh_l0, thr):
         """
         Copies and converts the provided PyTorch GRU weights into this layer.
 
         Arguments:
@@ -350,22 +357,22 @@
         bias = reorder_weights(bias_ih_l0).contiguous()
         recurrent_bias = reorder_weights(bias_hh_l0).contiguous()
 
         self.kernel = nn.Parameter(kernel)
         self.recurrent_kernel = nn.Parameter(recurrent_kernel)
         self.bias = nn.Parameter(bias)
         self.recurrent_bias = nn.Parameter(recurrent_bias)
-        self.thr_reparam = nn.Parameter(thr)
+        self.thr = nn.Parameter(thr)
 
     def reset_parameters(self):
         """Resets this layer's parameters to their initial values."""
         for k, v in self.named_parameters():
             if k in ['kernel', 'recurrent_kernel', 'bias', 'recurrent_bias']:
                 if v.data.ndimension() >= 2:
-                    nn.init.xavier_normal_(v)
+                    nn.init.xavier_normal_(v, gain=self.weight_initialization_gain)
                 else:
                     nn.init.zeros_(v)
 
     def grad_clip_norm(self, enable=True, norm=2.0):
         self._enable_grad_clip = enable
         self._max_norm = nn.Parameter(torch.Tensor(
             [norm if enable else -1.0]), requires_grad=False)
@@ -393,18 +400,23 @@
             (seq_len, batch_size, hidden_size).
           o: the output gate for all sequences (values: 0 or 1).
           trace: smoothed output values, can be beneficial for training.
         """
         input = self._permute(input)
         state_shape = [1, input.shape[1], self.hidden_size]
         h0 = self._get_state(input, state, state_shape)
-        thr = torch.sigmoid(self.thr_reparam)
+
+        # restrict thresholds to be between 0 and 1
+        self.thr.data.clamp_(min=0.0, max=1.0)
+
+        # run forward pass
         y, h, o, trace = self._impl(
-            input, h0[0], thr, self._get_zoneout_mask(input))
-        state = self._get_final_state(y, lengths)
+            input, h0[0], self.thr, self._get_zoneout_mask(input))
+
+        # prepare outputs
         output = self._permute(y[1:])
         h = self._permute(h[1:])
         o = self._permute(o[1:])
         trace = self._permute(trace[1:])
         return output, (h, o, trace)
 
     def _impl(self, input, state, thr, zoneout_mask):
```

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/support.cc` & `evnn_pytorch-0.2.0/frameworks/pytorch/support.cc`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/frameworks/pytorch/support.h` & `evnn_pytorch-0.2.0/frameworks/pytorch/support.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/blas.h` & `evnn_pytorch-0.2.0/lib/blas.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/device_assert.h` & `evnn_pytorch-0.2.0/lib/device_assert.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/egru_backward_cpu.cc` & `evnn_pytorch-0.2.0/lib/egru_backward_cpu.cc`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/egru_backward_gpu.cu.cc` & `evnn_pytorch-0.2.0/lib/egru_backward_gpu.cu`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/egru_forward_cpu.cc` & `evnn_pytorch-0.2.0/lib/egru_forward_cpu.cc`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/egru_forward_gpu.cu.cc` & `evnn_pytorch-0.2.0/lib/egru_forward_gpu.cu`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/evnn/egru.h` & `evnn_pytorch-0.2.0/lib/evnn/egru.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/evnn/egru_cpu.h` & `evnn_pytorch-0.2.0/lib/evnn/egru_cpu.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/evnn.h` & `evnn_pytorch-0.2.0/lib/evnn.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/lib/inline_ops.h` & `evnn_pytorch-0.2.0/lib/inline_ops.h`

 * *Files identical despite different names*

### Comparing `evnn_pytorch-0.1.0/setup.py` & `evnn_pytorch-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) 2023  Khaleelulla Khan Nazeer
+# This file incorporates work covered by the following copyright:
 # Copyright 2020 LMNT, Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -9,110 +11,122 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import os
+
+from glob import glob
+import warnings
+import subprocess
+import torch
+from setuptools import setup
+from torch.utils.cpp_extension import BuildExtension, CUDAExtension, CppExtension, CUDA_HOME
+
+
+def get_gpu_arch_flags():
+    try:
+        major, minor = torch.cuda.get_device_capability()
+        return [f"-gencode=arch=compute_{major}{minor},code=sm_{major}{minor}"]
+    except Exception as e:
+        warnings.warn(f"Error while detecting GPU architecture: {e}\n \
+                        Use env var EVNN_CUDA_COMPUTE to set cuda compute capability")
+        compute_capability = os.getenv("EVNN_CUDA_COMPUTE", None)
+        if compute_capability is None:
+            warnings.warn("EVNN_CUDA_COMPUTE not defined, using default: 80")
+            compute_capability = 80
+
+        return [f"-gencode=arch=compute_{compute_capability},code=sm_{compute_capability}"]
+
+def check_nvcc_available():
+    try:
+        subprocess.run(["nvcc", "--version"], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        return True
+    except FileNotFoundError:
+        warnings.warn(
+            f"nvcc was not found. Skip compiling GPU kernels"
+        )
+        return False
+    except subprocess.CalledProcessError:
+        warnings.warn(
+            f"nvcc was not found. Skip compiling GPU kernels"
+        )
+        return False
+    
+
+arch_flags = get_gpu_arch_flags()
 
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'EVNN: a torch extension for custom event based RNN models.'
 AUTHOR = 'TUD and RUB'
 AUTHOR_EMAIL = 'khaleelulla.khan_nazeer@tu-dresden.de'
 URL = 'https://tu-dresden.de/ing/elektrotechnik/iee/hpsn'
 LICENSE = 'Apache 2.0'
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering :: Mathematics',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries',
 ]
-# Copyright 2020 LMNT, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-
-import os
-import sys
-
-from glob import glob
-from platform import platform
-from torch.utils import cpp_extension
-import torch
-from setuptools import setup
-from setuptools.dist import Distribution
 
 
 with open(f'frameworks/pytorch/_version.py', 'wt') as f:
     f.write(f'__version__ = "{VERSION}"')
 
 base_path = os.path.dirname(os.path.realpath(__file__))
 
-if torch.cuda.is_available():
-    make_cmd = 'make evnn'
+if check_nvcc_available():
 
-    if 'Windows' in platform():
-        CUDA_HOME = os.environ.get('CUDA_HOME', os.environ.get('CUDA_PATH'))
-        extra_args = []
-    else:
-        CUDA_HOME = os.environ.get('CUDA_HOME', '/usr/local/cuda')
-        extra_args = ['-Wno-sign-compare']
-
-    extension = cpp_extension.CUDAExtension(
+    extension = [CUDAExtension(
         'evnn_pytorch_lib',
-        sources=glob('frameworks/pytorch/*.cc'),
-        extra_compile_args=extra_args + ['-DWITH_CUDA'],
+        sources=glob('frameworks/pytorch/*.cc') + glob('lib/*.cu') + glob('lib/*.cc'),
+        extra_compile_args={
+                "cxx": ["-O2", "-std=c++17", "-D_GLIBCXX_USE_CXX11_ABI=0", "-DWITH_CUDA", "-Wno-sign-compare"],
+                "nvcc": ["-O2", "-std=c++17", 
+                         "-U__CUDA_NO_HALF_OPERATORS__",
+                         "-U__CUDA_NO_HALF_CONVERSIONS__",
+                         "-D_GLIBCXX_USE_CXX11_ABI=0", "-DWITH_CUDA",
+                         "-Xcompiler", "-fPIC", "-lineinfo"]
+                + arch_flags,
+        },
         include_dirs=[os.path.join(base_path, 'lib'),
-                      os.path.join(CUDA_HOME, 'include')],
-        libraries=['evnn', 'cblas', 'c10'],
-        library_dirs=['.'])
+                      os.path.join(CUDA_HOME, 'include'),
+                      os.path.join(CUDA_HOME, 'lib64')],
+        libraries=['openblas', 'c10', 'cudart', 'cublas'],
+        library_dirs=['.']),
+    ]
 else:
-    make_cmd = 'make evnn_cpu'
-    extra_args = []
-    extension = cpp_extension.CppExtension(
+    extension = [CppExtension(
         'evnn_pytorch_lib',
-        sources=glob('frameworks/pytorch/*.cc'),
-        extra_compile_args=extra_args,
+        sources=glob('frameworks/pytorch/*.cc') + glob('lib/*.cc'),
+        extra_compile_args={
+                "cxx": ["-O2", "-std=c++17", "-D_GLIBCXX_USE_CXX11_ABI=0", "-Wno-sign-compare"],
+        },
         include_dirs=[os.path.join(base_path, 'lib'),],
-        libraries=['evnn', 'cblas'],
-        library_dirs=['.', os.path.join('/usr/lib/x86_64-linux-gnu')])
-
-
-class BuildEVNN(cpp_extension.BuildExtension):
-    def run(self):
-        os.system(make_cmd)
-        super().run()
+        libraries=['openblas'],
+        library_dirs=['.', os.path.join('/usr/lib/x86_64-linux-gnu')])]
 
 
 setup(name='evnn_pytorch',
       version=VERSION,
       description=DESCRIPTION,
       long_description=open('README.md', 'r', encoding='utf-8').read(),
       long_description_content_type='text/markdown',
       author=AUTHOR,
       author_email=AUTHOR_EMAIL,
       url=URL,
       license=LICENSE,
       keywords='pytorch machine learning rnn lstm gru custom op',
       packages=['evnn_pytorch'],
       package_dir={'evnn_pytorch': 'frameworks/pytorch'},
-      install_requires=[],
-      ext_modules=[extension],
-      cmdclass={'build_ext': BuildEVNN},
+      install_requires=['torch'],
+      ext_modules=extension,
+      cmdclass={'build_ext': BuildExtension.with_options(use_ninja=False),},
       classifiers=CLASSIFIERS)
```

