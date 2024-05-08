# Comparing `tmp/cengal-4.3.1-py3-none-any.whl.zip` & `tmp/cengal-4.4.0-pp39-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 18709 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1206 b- defN 24-Mar-31 22:36 cengal_shell/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    39399 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      614 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      552 b- defN 24-Mar-31 22:38 cengal-4.3.1.dist-info/RECORD
-7 files, 53234 bytes uncompressed, 17735 bytes compressed:  66.7%
+Zip file size: 18812 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    45157 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      614 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      471 b- defN 24-May-08 04:03 cengal-4.4.0.dist-info/RECORD
+6 files, 57705 bytes uncompressed, 17962 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
-Filename: cengal_shell/__init__.py
+Filename: cengal-4.4.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: cengal-4.3.1.dist-info/LICENSE.md
+Filename: cengal-4.4.0.dist-info/METADATA
 Comment: 
 
-Filename: cengal-4.3.1.dist-info/METADATA
+Filename: cengal-4.4.0.dist-info/NOTICE
 Comment: 
 
-Filename: cengal-4.3.1.dist-info/NOTICE
+Filename: cengal-4.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: cengal-4.3.1.dist-info/WHEEL
+Filename: cengal-4.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cengal-4.3.1.dist-info/top_level.txt
-Comment: 
-
-Filename: cengal-4.3.1.dist-info/RECORD
+Filename: cengal-4.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cengal-4.3.1.dist-info/LICENSE.md` & `cengal-4.4.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cengal-4.3.1.dist-info/METADATA` & `cengal-4.4.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 4.3.1
+Version: 4.4.0
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async wxPython,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
@@ -121,87 +121,225 @@
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: NOTICE
-Requires-Dist: cengal-light[full] ==4.3.1
+Requires-Dist: charset-normalizer
+Requires-Dist: http-parser
+Requires-Dist: cchardet
+Requires-Dist: Cython >=0.29.34
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: greenlet
+Requires-Dist: colorama
+Requires-Dist: py-cpuinfo
+Requires-Dist: lmdb
+Requires-Dist: async-generator
+Requires-Dist: simplejson
+Requires-Dist: cbor
+Requires-Dist: cbor2
+Requires-Dist: ujson
+Requires-Dist: cloudpickle
+Requires-Dist: python3-dtls
+Requires-Dist: psutil
+Requires-Dist: ttkbootstrap
+Requires-Dist: pprintpp
+Requires-Dist: msgpack-pypy
+Requires-Dist: cengal-light[full] ==4.4.0
 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/cengal-light)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cengal-light?color=darkgreen)
 
-![PyPI - Version](https://img.shields.io/pypi/v/cengal-light) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cengal-light) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/cengal-light) ![PyPI - Format](https://img.shields.io/pypi/format/cengal-light) ![Static Badge](https://img.shields.io/badge/Architecture-x86__64_%7C_ARM__64-blue)
+![GitHub tag (with filter)](https://img.shields.io/github/v/tag/FI-Mihej/Cengal) ![Static Badge](https://img.shields.io/badge/OS-Linux_%7C_Windows_%7C_macOS-blue) ![Static Badge](https://img.shields.io/badge/coverage-38%25-blue) ![Static Badge](https://img.shields.io/badge/covered_lines_of_code-15855-blue)
 
-![Static Badge](https://img.shields.io/badge/wheels-Linux_%7C_Windows_%7C_macOS-blue) ![Static Badge](https://img.shields.io/badge/OS-Linux_%7C_Windows_%7C_macOS-blue)
+![PyPI - Version](https://img.shields.io/pypi/v/cengal-light) ![PyPI - Format](https://img.shields.io/pypi/format/cengal-light?color=darkgreen) ![Static Badge](https://img.shields.io/badge/wheels-Linux_%7C_Windows_%7C_macOS-blue) ![Static Badge](https://img.shields.io/badge/Architecture-x86__64_%7C_ARM__64-blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cengal-light) ![Static Badge](https://img.shields.io/badge/PyPy-3.8_%7C_3.9_%7C_3.10-blue) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/cengal-light) 
 
-![GitHub tag (with filter)](https://img.shields.io/github/v/tag/FI-Mihej/Cengal) ![PyPI - Status](https://img.shields.io/pypi/status/cengal) ![GitHub License](https://img.shields.io/github/license/FI-Mihej/Cengal)
+![GitHub License](https://img.shields.io/github/license/FI-Mihej/Cengal?color=darkgreen) ![PyPI - Status](https://img.shields.io/pypi/status/cengal) 
 
 # Cengal
 
-Cengal is a versatile Python library designed for a wide range of applications. To enhance performance, certain modules within Cengal have been implemented using Cython and/or C.
+Cengal is a versatile Python library designed for a wide range of applications. To enhance performance, certain modules within Cengal have been implemented using Cython, C/C++, Nim or Go.
 
-## API Design Approach
+## Architecture & API Design Rationale
+
+<details>
+<summary title="Rationale"><kbd> Rationale </kbd></summary>
 
 The Cengal library adheres to an API design approach used in frameworks such as Qt. For those familiar with the C++ language, I will draw comparisons between the approaches of Qt and the C++ Standard Template Library (STL). The API provided by the STL was designed to significantly reduce the burden on programmers who develop the STL. This decision was logical from the standpoint of marketing the STL among compiler creators. However, this led to the usability of the STL for the user not being great. This is evident in the fact that the STL provides the most minimal possible API, and any conveniences must be programmed anew by each programmer every time - constantly reinventing the wheel. In contrast, Qt uses the opposite approach to API construction: classes have many methods whose purposes are similar, but are aimed at different usage models. This simplifies the use of Qt for users, speeds up the writing of the final code, and avoids many errors that we usually make when we write our own 'bicycles' for the same actions each time (not because the we are not smart, but because we are humans and therefore prone to make mistakes from time to time).
 
+</details>
+
 # Cengal compatibility and requirements
 
-* Target platforms: Win32, Linux, OS X, Android, iOS, Emscripten
+<details>
+<summary title="Compatibility and requirements"><kbd> Compatibility and requirements </kbd></summary>
+
+* Target platforms: Win32, Linux, macOS, Android, iOS, Emscripten
 * Target architectures: x64, x86, ARM
 * Target interpreters: CPython, PyPy
 * Recommended Python versions: 3.8+
 
+</details>
+
 # Installation
 
+<details>
+<summary title="General wheel"><kbd> General wheel </kbd></summary>
+
 To get started with Cengal, you can easily install it along with all the mandatory dependencies by running `pip install cengal`. This command not only installs Cengal and its required dependencies but also takes care of fetching and installing prebuilt wheels tailored for the Cengal library. These wheels are compatible with both Windows and Linux systems and work seamlessly with both CPython and PyPy interpreters.
 
+</details>
+
+<details>
+<summary title="Wheel without dependencies"><kbd> Wheel without dependencies </kbd></summary>
+
 If you prefer to install Cengal without its dependencies, you can opt for the 'cengal-light' package, which serves as the backend for the 'cengal' package. Simply run `pip install cengal-light` to get the lightweight version of Cengal.
 
+</details>
+
 # Documentation
 
 [Cengal Documentation](https://FI-Mihej.github.io/Cengal)
 
 For example [Cengal Coroutines Concepts & Usage](https://FI-Mihej.github.io/Cengal/coroutines_concepts/)
 
 or partially:
 
 [Cengal Wiki](https://github.com/FI-Mihej/Cengal/wiki)
 
 For example [Wiki: Cengal Coroutines Concepts & Usage](https://github.com/FI-Mihej/Cengal/wiki/Cengal-Coroutines)
 
 # Stand-Alone Packages for Specific Cengal Modules
 
+<details>
+<summary title="Rationale"><kbd> Rationale </kbd></summary>
+
 To cater to varying needs and streamline the installation process, I've introduced stand-alone packages for select Cengal modules. These packages are designed to offer users the ability to install specific Cengal functionality without the burden of the library's full set of dependencies.
 
 The core of this approach lies in our 'cengal-light' package, which houses both Python and compiled Cengal modules. The 'cengal' package itself serves as a lightweight shell, devoid of its own modules, but dependent on 'cengal-light[full]' for a complete Cengal library installation with all required dependencies.
 
 For users seeking individual Cengal features or looking to minimize dependencies, our stand-alone packages provide a convenient solution. Each stand-alone package is dedicated to a specific Cengal module and relies on 'cengal-light' as its sole dependency.
 
+</details>
+
 Below, you'll find a list of these stand-alone packages, each corresponding to a distinct Cengal module:
 
+* [CengalPolyBuild](https://github.com/FI-Mihej/CengalPolyBuild): A Comprehensive and Hackable Build System for Multilingual Python Packages: Cython (including automatic conversion from Python to Cython), C/C++, Objective-C, Go, and Nim, with ongoing expansions to include additional languages. (Planned to be released soon) 
+* [InterProcessPyObjects](https://github.com/FI-Mihej/InterProcessPyObjects) (package for `cengal.parallel_execution.asyncio.ashared_memory_manager` module): High-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. 
 * [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) (package for `cengal.hardware.memory.barriers` module): Fast crossplatform memory barriers for Python.
 * [cengal_cpu_info](https://github.com/FI-Mihej/cengal_cpu_info) (package for `cengal.hardware.info.cpu` module): Extended, cached CPU info with consistent output format.
 * [cengal_app_dir_path_finder](https://github.com/FI-Mihej/cengal_app_dir_path_finder) (package for `cengal.file_system.app_fs_structure.app_dir_path` module): Offering a unified API for easy retrieval of OS-specific application directories, enhancing data management across Windows, Linux, and macOS.
 
 Stay tuned for future additions to our collection of stand-alone packages!
 
 # Exclusive Features: No Alternatives Online
 
+
+<details>
+<summary title="Build system (work in progress)"><kbd> Build system (work in progress) </kbd></summary>
+
 ## Build system (work in progress)
 
 Automatic hackable build system for your package which supports Python modules made with different languages: Cython (including Python to Cython automatic compilation), C/C++, ObjectiveC, Go, Nim. Other languages support is in progress.
 
 Compiles your code, gather binary artifacts and puts them into your wheel.
 
 ### Examples
 
 * [Compilable Golang module](https://github.com/FI-Mihej/Cengal/blob/master/cengal/_examples/ex_golang)
 * [Compilable Nim module](https://github.com/FI-Mihej/Cengal/blob/master/cengal/_examples/ex_nim)
 * [Pure Python module auto-compiled with Cython](https://github.com/FI-Mihej/Cengal/blob/master/examples/compiled_python)
 
+</details>
+
+<details>
+<summary title="Fast inter-process communication through shared memory"><kbd> Fast inter-process communication through shared memory </kbd></summary>
+
+## Fast inter-process communication through shared memory
+
+blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. By minimizing the need for frequent serialization-deserialization, it enhances overall speed and responsiveness. The package offers a comprehensive suite of functionalities designed to support a diverse array of Python types and facilitate asynchronous IPC, optimizing performance for demanding applications.
+
+![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+
+```python
+from cengal.hardware.memory.shared_memory import *
+from cengal.parallel_execution.asyncio.ashared_memory_manager import *
+```
+
+### Key Features
+
+* Shared Memory Communication:
+    * Enables sharing of Python objects directly between processes using shared memory.
+    * Utilizes a linked list of global messages to inform connected processes about new shared objects.
+
+* Lock-Free Synchronization:
+    * Uses memory barriers for efficient communication, avoiding slow syscalls.
+    * Ensures each process can access and modify shared memory without contention.
+
+* Supported Python Types:
+    * Handles various Python data structures including:
+        * Basic types: `None`, `bool`, 64-bit `int`, large `int` (arbitrary precision integers), `float`, `complex`, `bytes`, `bytearray`, `str`.
+        * Standard types: `Decimal`, `slice`, `datetime`, `timedelta`, `timezone`, `date`, `time`
+        * Containers: `tuple`, `list`, classes inherited from: `AbstractSet` (`frozenset`), `MutableSet` (`set`), `Mapping` and `MutableMapping` (`dict`).
+        * Pickable classes instancess: custom classes including `dataclass`
+    * Allows mutable containers (lists, sets, mappings) to save basic types (`None`, `bool`, 64 bit `int`, `float`) internally, optimizing memory use and speed.
+
+* NumPy and Torch Support:
+    * Supports numpy arrays by creating shared bytes objects coupled with independent arrays.
+    * Supports torch tensors by coupling them with shared numpy arrays.
+
+* Custom Class Support:
+    * Projects pickable custom classes instancess (including `dataclasses`) onto shared dictionaries in shared memory.
+    * Modifies the class instance to override attribute access methods, managing data fields within the shared dictionary.
+    * supports classes with or without `__dict__` attr
+    * supports classes with or without `__slots__` attr
+
+* Asyncio Compatibility:
+    * Provides a wrapper module for async-await functionality, integrating seamlessly with asyncio.
+    * Ensures asynchronous operations work smoothly with the package's lock-free approach.
+
+### Docs
+
+[Readme.md](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/README.md)
+
+### Examples
+
+* An async examples (with asyncio):
+    * [shared_objects__example__sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__example__sender.py)
+    * [shared_objects__example__receiver.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__example__receiver.py)
+    * [shared_objects__types.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__types.py)
+
+### Performance Benchmark results
+
+| Approach                        | sync/async | Throughput GiB/s |
+|---------------------------------|------------|------------------|
+| InterProcessPyObjects (sync)    | sync       | 3.770            |
+| InterProcessPyObjects + uvloop  | async      | 3.222            |
+| InterProcessPyObjects + asyncio | async      | 3.079            |
+| multiprocessing.shared_memory   | sync       | 2.685            |
+| uvloop.UnixDomainSockets        | async      | 0.966            |
+| asyncio + cengal.Streams        | async      | 0.942            |
+| uvloop.Streams                  | async      | 0.922            |
+| asyncio.Streams                 | async      | 0.784            |
+| asyncio.UnixDomainSockets       | async      | 0.708            |
+| multiprocessing.Queue           | sync       | 0.669            |
+| multiprocessing.Pipe            | sync       | 0.469            |
+
+### Todo
+
+- [ ] Connect more than two processes
+- [ ] Use third-party fast hashing implementations instead of or in addition to built in `hash()` call
+- [ ] Continuous performance improvements
+
+</details>
+
+<details>
+<summary title="Concurrent Execution of blocking CPU-Bound and GUI Tasks on a Single Thread"><kbd> Concurrent Execution of blocking CPU-Bound and GUI Tasks on a Single Thread </kbd></summary>
+
 ## Concurrent Execution of blocking CPU-Bound and GUI Tasks on a Single Thread
 
 Cengal offers a unique and powerful feature that allows you to execute a diverse set of tasks concurrently on a single thread, effectively managing CPU-bound and GUI-related operations without introducing the complexity of multithreading or multiprocessing. Notably, Cengal can convert `blocking CPU-bound` functions into proper asynchronous coroutines, preventing them from blocking the thread for extended periods.
 
 ### Examples
 
 In this example, an application concurrently (at the same time) executes all of the following components within a single thread:
@@ -222,184 +360,140 @@
 * [rich_example.py](https://github.com/FI-Mihej/Cengal/blob/master/examples/rich_example.py)
 * [third_party_cpu_bound.py](https://github.com/FI-Mihej/Cengal/blob/master/examples/third_party_cpu_bound.py)
 
 #### Tutorial
 
 * [Decorator which converts blocking code to concurrent code](https://github.com/FI-Mihej/Cengal/wiki/Decorator-which-converts-blocking-code-to-concurrent-code)
 
+</details>
 
-## True Interprocess Shared Memory (Proof of Concept)
-
-Cengal introduces a novel approach to interprocess shared memory, currently at the proof of concept stage. With this feature, you can seamlessly share data between your Python processes (currently limited to 2 processes) and work with them just as you would in a single process. The underlying mechanism optimizes cross-process communication by employing efficient memory barriers instead of resource-intensive system calls.
-
-Supported data types (current stage):
-
-* shared Numpy arrays
-* `list`: Unlike `multiprocessing.shared_memory.ShareableList`, Cengal's shared lists are both `mutable` and `resizable` between different processes. They support various container types (lists, tuples, dicts) as items and implement all standard `list` methods. Plus, they offer superior performance compared to `multiprocessing.shared_memory.ShareableList`.
-* `dict`: Currently immutable.
-* `tuple`
-* `str`
-* `bytes`
-* `bytearray`
-* `bool`
-* `float`: Cengal's shared float values support Addition Assignment (`shared_list[20] += 999.3`) and all other native methods and operators, unlike values in `multiprocessing.shared_memory.ShareableList`.
-* `int`: Currently limited to int64. Similar to shared float values, Cengal's shared integers support Addition Assignment (`shared_list[15] += 999`) and all other native methods and operators.
-* `None`
-
-### Examples
-
-General example:
-
-* [shared_memory_example.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/shared_memory_example.py)
-
-Messages transmit:
-
-* [shmem_sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/shmem_sender.py)
-* [shmem_receiver.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/shmem_receiver.py)
-
-Shared Numpy Array:
-
-* [numpy_array_shmem_main.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/numpy_array_shmem_main.py)
-* [numpy_array_shmem_worker.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/numpy_array_shmem_worker.py)
-
-and smaller:
-
-```python
-from multiprocessing import Process
-from cengal.hardware.memory.shared_memory import *
-
-
-shared_memory_name = 'test_shared_mem'
-shared_memory_size = 200 * 1024 * 1024
-switches = 1000
-changes_per_switch = 2000
-
-
-def work(manager, shared_data)
-    index = 0
-    while index < switches:
-        with wait_my_turn(manager):
-            # emulatin our working process
-            for i in range(changes_per_switch):
-                shared_data[1] += 1
-
-def second_process():
-    consumer: SharedMemory = SharedMemory('test_shmem', False)
-    consumer.wait_for_messages()
-    with wait_my_turn(consumer):
-        shared_data = consumer.take_message()
-    
-    work(consumer, shared_data)
-
-
-creator: SharedMemory = SharedMemory(shared_memory_name, True, shared_memory_size)
-p = Process(target=second_process)
-p.start()
-creator.wait_consumer_ready()
-with wait_my_turn(creator):
-    data = [
-        'hello',
-        0,
-        (8, 2.0, False),
-        {
-            b'world': -6,
-            5: 4
-        }
-    ]
-    shared_data = creator.put_message(data)
-
-work(creator, shared_data)
-p.join()
-```
-
-### Performance Benchmark results
-
-In the realm of performance, Cengal's shared `list` container, although not yet fully optimized, is already outpacing the performance of `multiprocessing.shared_memory.ShareableList`. What sets it apart is its comprehensive support for native methods and operators, including Addition Assignment (`shared_list[15] += 999`), a feature unavailable in `multiprocessing.shared_memory.ShareableList`.
-
-Cengal's shared `list` container demonstrates remarkable speed, boasting the ability to handle over 30,000,000 reads/writes per second for an int64 value (`shared_list[2] = 1234` / `val = shared_list[7]`), or more than 1,450,000 addition assignments per second (`shared_list[15] += 999`). These performance figures underscore the efficiency and versatility of Cengal's interprocess shared memory solution, even in its current state.
-
-[Benchmark Results](https://github.com/FI-Mihej/Cengal/blob/master/cengal/hardware/memory/shared_memory/versions/v_0/development/benchmark_results.md)
-
-
-### Roadmap
-
-* Continuosly moving more logic to Cython
-* Implement mutable `dict` and `set` using an appropricate C hashmap library or C++ code (depending what will be faster in our case)
-* Increase number of interacting processes from 2 to variable value
-* Implement garbage collector for shared data in addition to manual `free()` call
-* Implement an appropriate Service for `cengal.parallel_execution.coroutines` - for comfortable shared memory usage inside an async code (including `asyncio`) 
-* Improve memory allocation algorithm in an attempt of making it faster
+<details>
+<summary title="Async LMDB database API"><kbd> Async LMDB database API </kbd></summary>
 
 ## Async LMDB database API
 
 An example of usage (unit test of the module):
 * [test__db.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_1/tests/test__db.py)
 
+</details>
+
+<details>
+<summary title="Async logging into LMDB database"><kbd> Async logging into LMDB database </kbd></summary>
+
 ## Async logging into LMDB database
 
 Developer can observe their logs in runtime using `cengal.parallel_execution.coroutines.coro_tools.loop_administration.admin_tk` module (made with Async Tkinter GUI):
 * [admin_tk.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/loop_administration/admin_tk/versions/v_0/admin_tk.py)
 
 An example of usage of the admin_tk:
 * [admin_test.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/loop_administration/admin_tk/versions/v_0/development/admin_test.py)
 
 Alternatively, developer can load logs in off-line mode using Log Viewer application (made with async Tkinter GUI):
 * [log_viewer.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/log_viewer/versions/v_0/log_viewer.py)
 
+</details>
+
+<details>
+<summary title="Async Tkinter and Customtkinter"><kbd> Async Tkinter and Customtkinter </kbd></summary>
+
 ## Async Tkinter and Customtkinter
 
 * [tkinter_0.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/development/tkinter_0.py)
 * [customtkinter_0.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/development/customtkinter_0.py)
 
+</details>
+
+<details>
+<summary title="Async wxPython"><kbd> Async wxPython </kbd></summary>
+
 ## Async wxPython
 
 * [async_wxpython_example.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/integrations/wxpython/versions/v_0/development/async_wxpython_example.py)
 
+</details>
+
+<details>
+<summary title="Async QT (PySide, PySide2, PySide6, PyQt4, PyQt5, PyQt6)"><kbd> Async QT (PySide, PySide2, PySide6, PyQt4, PyQt5, PyQt6) </kbd></summary>
+
 ## Async QT (PySide, PySide2, PySide6, PyQt4, PyQt5, PyQt6)
 
 * [pyside6__coro_slot_example_0.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/integrations/qt/pyside6/versions/v_0/development/pyside6__coro_slot_example_0.py)
 
-## Async PyTermGUI
+</details>
+
+<details>
+<summary title="Async PyTermGUI"><kbd> Async PyTermGUI </kbd></summary>
+
+## Async [PyTermGUI](https://github.com/bczsalba/pytermgui)
 
 * [hello_world_app_autoexit.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/development/hello_world_app_autoexit.py)
 * [hello_world.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/development/hello_world.py)
 
+</details>
+
+<details>
+<summary title="Wrapper for Netti (reliable UDP connection library for games in Nim)"><kbd> Wrapper for Netti (reliable UDP connection library for games in Nim) </kbd></summary>
+
+## Wrapper for [Netti (reliable UDP connection library for games in Nim)](https://github.com/treeform/netty)
+
+* [netty_benchmarks.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/integrations/nim__netty/core/versions/v_0/development/netty_benchmarks.py)
+
+</details>
+
+<details>
+<summary title="Transparent background for your desktop applications (TBA)"><kbd> Transparent background for your desktop applications (TBA) </kbd></summary>
+
 ## Transparent background for your desktop applications (TBA)
 
 * Target OS: Windows 11, Windows 10, Windows 8, Windows 7, Windows Vista.
 * Target frameworks: PySide, PyQt, Kivy, PyWebView 
 
 ![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/Cengal_PyWebView_Transparent_UI_Windows_10.png)
 ,
 ![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/Cengal_Kivy_Transparent_UI_Windows_10.png)
 
+</details>
+
+<details>
+<summary title="Tkinter True Borderless apps for Windows platform (TBA)"><kbd> Tkinter True Borderless apps for Windows platform (TBA) </kbd></summary>
+
 ## Tkinter True Borderless apps for Windows platform (TBA)
 
 * Target OS: Windows 11, Windows 10, Windows 8, Windows 7, Windows Vista.
 * Target frameworks: CustomTkinter, Tkinter, ttkbootstrap, ...
 
 ![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/Cengal_Tkinter_True_Borderless_Draggable_Applications_Windows_10.png)
 
+</details>
+
+<details>
+<summary title="Cengal Coroutines and Asyncio Administration and Monitoring Page"><kbd> Cengal Coroutines and Asyncio Administration and Monitoring Page </kbd></summary>
+
 ## Cengal Coroutines and Asyncio Administration and Monitoring Page
 
 Observe loop performance, services state and coroutines list with details. Use an async interactive console in order to interact with your application from inside.
 
 ### YouTube Showcase
 
 <a href="https://www.youtube.com/watch?feature=player_embedded&v=qiuOH9B6uCY" target="_blank">
  <img src="https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/CoroSchedulerAdminYoutube.png" alt="Watch the video" width="640" height="360" border="5" />
 </a>
 
 ### Examples
 
 [admin_test.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/loop_administration/admin_tk/versions/v_0/development/admin_test.py)
 
+</details>
+
 
 # Modules with unique functionality
 
+<details>
+<summary title="Unique modules List (was not updated for some time)"><kbd> Unique modules List (was not updated for some time) </kbd></summary>
+
 * **"parallel_execution"**
     * **"coroutines"** - asynchronous loop with almost preemptive multitasking within the single thread. Brings an async approach to an unmodified Tkinter, Qt, Kivy, etc. Unlike asyncio/trio/curio, it uses microkernel (services-based) approach which makes it highly- and easily-expandable. Can be executed both independently (asyncio/uvloop loop will be injected within the Cengal-coroutine when needed) and within already executed asyncio/uvloop loop. Can be used from the PyScript for the Web app creation.
         * **"coro_standard_services"** - set of standard services. You can replace standard service by yours for your app or for third-party module without code changes: by registering your own alias.
             * **"loop_yield"** - automatically kinda yield from your loops from time to time (priority based). Can be used to make a proper coroutine (which will not hangs on its endless loops) even from the long-running CPU-hungry third-party function (by function's bytecode modification made in runtime).
             * **"tkinter"** - make your Tkninter app async easily. Run any number of asynchronous Tkinter apps in single thread.
             * **"db"** - async wrapper around LMDB which provides an appropriate async API
             * **"asyncio_loop"** - use asyncio-based code directly from your async Cengal-coroutine neither [Trio](https://github.com/python-trio/trio) nor [Curio](https://github.com/dabeaz/curio) able to to do this
@@ -426,15 +520,21 @@
     * **"memory"** - RAM related
         * **"barriers"** - fast full memory barriers for both x86/x64 and ARM (Windows, Linux, OS X, iOS, Android).
 * **"time_management"** - 
     * **"high_precision_sync_sleep"** - provides an ability to put your thread into legetimate sleep for at least 10x smaller time period than `time.sleep()` from the Python's Standard Library able to do on same Operating System: uses `nanosleep()` on Linux and periodic `SwitchToThread()` on Windows.
     * **"cpu_clock_cycles"** - Returnes value of `RDTSCP` on x86/x86_64 or `CNTVCT_EL0` on ARM. Fast implementation: 6-12 times faster than all other competitors on Github. Note: CPU Time Stamp Counter (TSC) is not depends on actual current CPU frequency in modern CPUs (starting from around year 2007) so can be safely used as a high precision clock (see `time_management.cpu_clock` module). Windows, Linux and other Operating Systems are using it internaly.
     * **"cpu_clock"** - like `perf_counter()` but 25% faster. Supports both x86/x86_64 and ARM. `cpu_clock` is slightly faster than `cpu_clock_cycles` because `double` (`float` in Python terms) transfered from C-code to Python code more efficiently than `64-bit int` (which needs an addition internal logic inside the Python itself for conversion). Highest-precision possible since it is CPU Time Stamp Counter based which is not depends on actual current CPU frequency in modern CPUs (starting from around year 2007) so can be safely used as a high precision clock (and Windows, Linux and other Operating Systems are using it internaly in this way). **Benchmark**: [cpu_clock_test.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/time_management/cpu_clock/versions/v_0/development/cpu_clock_test.py)
 
+</details>
+
 # Some Other modules
+
+<details>
+<summary title="Other modules List (was not updated for some time)"><kbd> Other modules List (was not updated for some time) </kbd></summary>
+
 * **"parallel_execution"**
     * **"coroutines"** - 
         * **"coro_tools"** - tools
             * **"wait_coro"** - decorate your coroutine in order to be able to execute it from the plain sunc code as a sync function
             * **"run_in_loop"** - serves the same purpose as an asyncio.run() call
             * **"prepare_loop"** - creates and returns loop. You may use it later
     * **"asyncio"** - tools for an asyncio
@@ -491,14 +591,16 @@
         * **"nt"** - 
             * **"blur_behind"** - Turn on Aero Glass backgrownd in Winndows 7, 10, 11 using documented or undocumented API (which one is awailable)
             * **"dpi_awareness"** - Turn on DPI awareness
 * **"web_tools"** - 
     * **"detect_browsers_host_device_type"** - 
         * **"by_http_user_agent"** - detects is it mobile or tablet device by analizing its http user_agent string
 
+</details>
+
 ## Size of the Cengal library
 
 At the moment of 19 Mar 2024:
 
 Around 200 modules
 
 ```
@@ -514,40 +616,83 @@
 -------------------------------------------------------------------------------
 SUM:                           770          24509          30650          79612
 -------------------------------------------------------------------------------
 ```
 
 Counted with [cloc](https://github.com/AlDanial/cloc) util.
 
+## Unittest coverage
+
+At the moment of 2 Apr 2024:
+
+Linux:
+
+```
+Stmts   Miss  Cover
+41576  25826    38%
+```
+
 ## Examples
 
+<details>
+<summary title="Examples locations"><kbd> Examples locations </kbd></summary>
+
 * Can be found in [examples](https://github.com/FI-Mihej/Cengal/blob/master/examples/) dir
 * Each module has a `development` folder. Examples are usually placed there
 * Some of old examples can be fined inside the [tests](https://github.com/FI-Mihej/Cengal/blob/master/tests/) dir.
 
 ### Cengal.coroutines examples
 
 * [General idea, greenlet main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/main.py)
 * [General idea, async main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/amain.py)
 * [Transparent interconnection between Cengal.coroutines and asyncio](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/asyncio_interconnection.py)
 
 ### Text processing example
 
 [Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
 
-# Build
+</details>
+
+# Build from sources
+
+<details>
+<summary title="Build instructions"><kbd> Build instructions </kbd></summary>
 
-`pip install git+https://github.com/FI-Mihej/Cengal.git`
+Linux, macOS:
+
+```bash
+git clone https://github.com/FI-Mihej/Cengal.git
+cd ./Cengal
+./prepare__setup.sh
+./install_in_dev_mode.sh
+```
+
+Windows:
+
+```bat
+git clone https://github.com/FI-Mihej/Cengal.git
+cd .\Cengal
+.\prepare__setup.cmd
+.\install_in_dev_mode.cmd
+```
 
 Installation process requires compilation. So ensure that:
 * GCC/Clang is installed in your Linux/WSL (`sudo apt-get --yes install build-essential` for Ubuntu. And `./before_install_on_wsl.sh` for Ubuntu under WSL for UI like Tkinter or Qt if you are using some kind of XServer on your host Windows)
 * At least `Visual Studio Community - Build Tools` are installed on your Windows and you are installing Cengal from within its `Developer Command Prompt` for an appropriate target CPU architecture (`x64 Native Tools Command Prompt for VS 2022` for example). Make sure that you have compatible version of Visual Studio for your target CPython interpreter (see `python -VV` command output. For example `Python 3.9.11 (tags/v3.9.11:2de452f, Mar 16 2022, 14:33:45) [MSC v.1929 64 bit (AMD64)]`: this python interpreter requires Visual Studio 2019 version 16.11.2+ according to `1929` word search in [Wikipedia page](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B))
+* Nim installed (Optional)
+* Go installed (Optional)
+
+</details>
 
 # Projects using Cengal
 
+* [CengalPolyBuild](https://github.com/FI-Mihej/CengalPolyBuild) - A Comprehensive and Hackable Build System for Multilingual Python Packages: Cython (including automatic conversion from Python to Cython), C/C++, Objective-C, Go, and Nim, with ongoing expansions to include additional languages. (Planned to be released soon) 
+* [cengal_app_dir_path_finder](https://github.com/FI-Mihej/cengal_app_dir_path_finder) - A Python module offering a unified API for easy retrieval of OS-specific application directories, enhancing data management across Windows, Linux, and macOS 
+* [cengal_cpu_info](https://github.com/FI-Mihej/cengal_cpu_info) - Extended, cached CPU info with consistent output format.
+* [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) - Fast crossplatform memory barriers for Python.
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
 * [SmartCATaloguer.com](http://www.smartcataloguer.com/index.html) - TagDB based catalog of images (tags), music albums (genre tags) and apps (categories)
 
 # License
```

## Comparing `cengal-4.3.1.dist-info/NOTICE` & `cengal-4.4.0.dist-info/NOTICE`

 * *Files identical despite different names*

