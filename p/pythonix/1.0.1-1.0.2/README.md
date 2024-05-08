# Comparing `tmp/pythonix-1.0.1.tar.gz` & `tmp/pythonix-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.1.tar", max compression
+gzip compressed data, was "pythonix-1.0.2.tar", max compression
```

## Comparing `pythonix-1.0.1.tar` & `pythonix-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     2775 2024-04-25 19:04:51.854118 pythonix-1.0.1/README.md
--rw-r--r--   0        0        0      284 2024-04-25 19:05:05.674118 pythonix-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.1/pythonix/__init__.py
--rw-r--r--   0        0        0     5348 2024-04-25 15:52:31.904118 pythonix-1.0.1/pythonix/internals/__pycache__/op.cpython-312.pyc
--rw-r--r--   0        0        0     2421 2024-04-18 01:37:05.054118 pythonix-1.0.1/pythonix/internals/__pycache__/ops.cpython-312.pyc
--rw-r--r--   0        0        0     4967 2024-04-25 15:54:40.194118 pythonix-1.0.1/pythonix/internals/__pycache__/pair.cpython-312.pyc
--rw-r--r--   0        0        0     7799 2024-04-22 17:28:53.444118 pythonix-1.0.1/pythonix/internals/__pycache__/pipe.cpython-312.pyc
--rw-r--r--   0        0        0     7141 2024-04-18 01:37:05.044118 pythonix-1.0.1/pythonix/internals/__pycache__/pipes.cpython-312.pyc
--rw-r--r--   0        0        0    13646 2024-04-25 15:46:38.174118 pythonix-1.0.1/pythonix/internals/__pycache__/req.cpython-312.pyc
--rw-r--r--   0        0        0    10297 2024-04-23 19:30:10.434118 pythonix-1.0.1/pythonix/internals/__pycache__/request.cpython-312.pyc
--rw-r--r--   0        0        0    22954 2024-04-25 16:07:26.584118 pythonix-1.0.1/pythonix/internals/__pycache__/res.cpython-312.pyc
--rw-r--r--   0        0        0     7175 2024-04-25 16:23:02.564118 pythonix-1.0.1/pythonix/internals/__pycache__/trail.cpython-312.pyc
--rw-r--r--   0        0        0      817 2024-04-25 17:35:02.224118 pythonix-1.0.1/pythonix/internals/__pycache__/types.cpython-312.pyc
--rw-r--r--   0        0        0     4377 2024-04-25 15:52:22.614118 pythonix-1.0.1/pythonix/internals/mdeq.py
--rw-r--r--   0        0        0     2447 2024-04-25 15:52:31.424118 pythonix-1.0.1/pythonix/internals/op.py
--rw-r--r--   0        0        0     1368 2024-04-25 15:54:39.704118 pythonix-1.0.1/pythonix/internals/pair.py
--rw-r--r--   0        0        0     4045 2024-04-22 17:28:24.824118 pythonix-1.0.1/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     7316 2024-04-25 15:46:37.674118 pythonix-1.0.1/pythonix/internals/req.py
--rw-r--r--   0        0        0    11105 2024-04-25 18:28:01.164118 pythonix-1.0.1/pythonix/internals/res.py
--rw-r--r--   0        0        0     2183 2024-04-25 16:23:02.094118 pythonix-1.0.1/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2780 2024-04-25 18:04:02.194118 pythonix-1.0.1/pythonix/internals/tuple.py
--rw-r--r--   0        0        0       95 2024-04-25 17:35:01.674118 pythonix-1.0.1/pythonix/internals/types.py
--rw-r--r--   0        0        0      206 2024-04-23 18:09:04.734118 pythonix-1.0.1/pythonix/mdeq.py
--rw-r--r--   0        0        0       69 2024-04-22 17:26:16.504118 pythonix-1.0.1/pythonix/op.py
--rw-r--r--   0        0        0      133 2024-04-23 19:02:18.274118 pythonix-1.0.1/pythonix/pair.py
--rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.1/pythonix/pipe.py
--rw-r--r--   0        0        0      216 2024-04-25 15:14:51.934118 pythonix-1.0.1/pythonix/prelude.py
--rw-r--r--   0        0        0      644 2024-04-25 15:40:16.334118 pythonix-1.0.1/pythonix/req.py
--rw-r--r--   0        0        0      425 2024-04-22 18:27:24.324118 pythonix-1.0.1/pythonix/res.py
--rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.1/pythonix/trail.py
--rw-r--r--   0        0        0      181 2024-04-22 17:55:20.064118 pythonix-1.0.1/pythonix/tuple.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 pythonix-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3027 2024-05-08 15:06:58.839631 pythonix-1.0.2/README.md
+-rw-r--r--   0        0        0      284 2024-05-08 15:07:57.059631 pythonix-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.2/pythonix/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-08 15:00:35.669631 pythonix-1.0.2/pythonix/curry.py
+-rw-r--r--   0        0        0     5348 2024-04-25 15:52:31.904118 pythonix-1.0.2/pythonix/internals/__pycache__/op.cpython-312.pyc
+-rw-r--r--   0        0        0     2421 2024-04-18 01:37:05.054118 pythonix-1.0.2/pythonix/internals/__pycache__/ops.cpython-312.pyc
+-rw-r--r--   0        0        0     4967 2024-04-25 15:54:40.194118 pythonix-1.0.2/pythonix/internals/__pycache__/pair.cpython-312.pyc
+-rw-r--r--   0        0        0     7799 2024-04-22 17:28:53.444118 pythonix-1.0.2/pythonix/internals/__pycache__/pipe.cpython-312.pyc
+-rw-r--r--   0        0        0     7141 2024-04-18 01:37:05.044118 pythonix-1.0.2/pythonix/internals/__pycache__/pipes.cpython-312.pyc
+-rw-r--r--   0        0        0    13646 2024-04-25 15:46:38.174118 pythonix-1.0.2/pythonix/internals/__pycache__/req.cpython-312.pyc
+-rw-r--r--   0        0        0    10297 2024-04-23 19:30:10.434118 pythonix-1.0.2/pythonix/internals/__pycache__/request.cpython-312.pyc
+-rw-r--r--   0        0        0    22954 2024-04-25 16:07:26.584118 pythonix-1.0.2/pythonix/internals/__pycache__/res.cpython-312.pyc
+-rw-r--r--   0        0        0     7175 2024-04-25 16:23:02.564118 pythonix-1.0.2/pythonix/internals/__pycache__/trail.cpython-312.pyc
+-rw-r--r--   0        0        0      817 2024-04-25 17:35:02.224118 pythonix-1.0.2/pythonix/internals/__pycache__/types.cpython-312.pyc
+-rw-r--r--   0        0        0     8183 2024-05-08 15:01:24.259631 pythonix-1.0.2/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     3915 2024-05-08 14:33:57.509631 pythonix-1.0.2/pythonix/internals/mdeq.py
+-rw-r--r--   0        0        0     2596 2024-05-08 03:48:32.109631 pythonix-1.0.2/pythonix/internals/op.py
+-rw-r--r--   0        0        0     1376 2024-05-08 15:04:34.579631 pythonix-1.0.2/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     4169 2024-05-08 14:18:48.939631 pythonix-1.0.2/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     7385 2024-05-08 14:37:25.509631 pythonix-1.0.2/pythonix/internals/req.py
+-rw-r--r--   0        0        0    12034 2024-05-08 14:07:35.969631 pythonix-1.0.2/pythonix/internals/res.py
+-rw-r--r--   0        0        0     2251 2024-05-08 14:22:48.329631 pythonix-1.0.2/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2697 2024-05-08 14:35:33.779631 pythonix-1.0.2/pythonix/internals/tuple.py
+-rw-r--r--   0        0        0      178 2024-05-08 15:06:04.479631 pythonix-1.0.2/pythonix/internals/types.py
+-rw-r--r--   0        0        0      206 2024-04-23 18:09:04.734118 pythonix-1.0.2/pythonix/mdeq.py
+-rw-r--r--   0        0        0       69 2024-04-22 17:26:16.504118 pythonix-1.0.2/pythonix/op.py
+-rw-r--r--   0        0        0      133 2024-04-23 19:02:18.274118 pythonix-1.0.2/pythonix/pair.py
+-rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.2/pythonix/pipe.py
+-rw-r--r--   0        0        0      246 2024-05-08 15:06:15.069631 pythonix-1.0.2/pythonix/prelude.py
+-rw-r--r--   0        0        0      644 2024-04-25 15:40:16.334118 pythonix-1.0.2/pythonix/req.py
+-rw-r--r--   0        0        0      425 2024-04-22 18:27:24.324118 pythonix-1.0.2/pythonix/res.py
+-rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.2/pythonix/trail.py
+-rw-r--r--   0        0        0      181 2024-04-22 17:55:20.064118 pythonix-1.0.2/pythonix/tuple.py
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 pythonix-1.0.2/PKG-INFO
```

### Comparing `pythonix-1.0.1/README.md` & `pythonix-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 If you have like functional programming, but have to program in Python, then check this out.
 
 ## Features
 
 1. Exceptions as values support similar to Rust
 2. Emphasis on immutable types
 3. Great support for immutable data structures
-4. Wrapper types to enable consecutive function calls via pipes
+4. Wrapper types to enable consecutive function calls via pipelike types
 5. Strongly typed hints with generic support
 6. Emphasis on composability with partially applied functions
 7. Emphasis on removing nullability
 
 ## Examples
 
 ### Piping with Bind and Do
@@ -41,21 +41,27 @@
 ```
 
 ### Error as Value
 ```python
 from pythonix.prelude import *
 from pythonix.res import Res
 
-# Capture errors as types
+# Capture errors as types with the res decorators
 @res.safe(TypeError)
 def foo(bar: int) -> int:
     if not isinstance(bar, int):
         raise TypeError("Invalid type")
     return bar
 
+# Make functions that return `Ok` or `Err` to show the possibility of failure
+def far(boo: int) -> Res[int, TypeError]:
+    if not isinstance(boo, int):
+        return Err(TypeError("Invalid type"))
+    return Ok(boo)
+
 # The result is captured to show errors and success
 bar: Res[int, TypeError] = foo(5)
 
 # Pipe through consecutive functions to handle errors
 bar: int = (
     pipe.Bind(bar)
     (res.map(lambda x: x + 5))
```

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/op.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/op.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/ops.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/ops.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/pair.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/pair.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/pipe.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/pipe.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/pipes.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/pipes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/req.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/req.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/request.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/request.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/res.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/res.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/trail.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/trail.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/__pycache__/types.cpython-312.pyc` & `pythonix-1.0.2/pythonix/internals/__pycache__/types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/internals/mdeq.py` & `pythonix-1.0.2/pythonix/internals/mdeq.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 ### MDeq
 
 Functions used to create and perform operations safely on a singly typed mutable linked list.
 
 """
 from collections import deque
 from __future__ import annotations
-from typing import Callable, Iterable
+from typing import Iterable, Generic, TypeVar
 from pythonix.res import null_and_error_safe, safe, Ok
+from pythonix.curry import two, three
 
-class MDeq[T](object):
+Val = TypeVar('Val')
+NewVal = TypeVar('NewVal')
+
+class MDeq(Generic[Val], object):
     """
     `MDeq` is a singly-typed mutable linked list. `push` and `pop` operations are thread safe and run in
     `O(1)` time. Insert and get operations run in `O(n)` time. As a mutable data structure there are some
     rules to keep in mind.
 
     #### Rules
     - Only share one reference to a `MDeq` at a time
@@ -28,174 +32,139 @@
         (md.push(7))
         (md.push(8))
         (md.push(9))
     )
     ```
     """
 
-    inner: deque[T] = deque()
+    inner: deque[Val] = deque()
 
-    def __init__(self, *args: T):
+    def __init__(self, *args: Val):
         self.inner = deque(args)
 
 
-def new[T](*vals: T) -> MDeq[T]:
+def new(*vals: Val) -> MDeq[Val]:
     """
     Creates a new instance of `MDeq` with the `vals` passed in.
     Make sure all the types are the same or you'll have weird type hints.
     """
     return MDeq(*vals)
 
 
-def push[T](element: T) -> Callable[[MDeq[T]], Ok[None]]:
+@two
+def push(element: Val, deq: MDeq[Val]) -> Ok[None]:
     """
     Pushes a new element `T` to the end of an `MDeq`.
     """
-
-    def inner(deq: MDeq[T]) -> Ok[None]:
-        """
-        Specify the `MDeq` that will receive the new element.
-        """
-        deq.inner.append(element)
-        return Ok(None)
-
-    return inner
+    deq.inner.append(element)
+    return Ok(None)
 
 
-def pushleft[T](element: T) -> Callable[[MDeq[T]], Ok[None]]:
+@two
+def pushleft(element: Val, deq: MDeq[Val]) -> Ok[None]:
     """
     Pushes a new element `T` to be the new first element in an `MDeq`
     """
-
-    def inner(deq: MDeq[T]) -> Ok[None]:
-        deq.inner.appendleft(element)
-        return Ok(None)
-
-    return inner
+    deq.inner.appendleft(element)
+    return Ok(None)
 
 
-def insert[T](element: T):
+@three
+def insert(element: Val, index: int, deq: MDeq[Val]) -> Ok[None]:
     """
     Inserts a new element at the provided index. Runs on `O(n)` time.
 
     Provide the new element `T`
     """
+    deq.inner.insert(index, element)
+    return Ok(None)
 
-    def get_at(index: int):
-        """
-        Now provide the index.
-        """
 
-        def inner(deq: MDeq[T]) -> Ok[None]:
-            """
-            Now provide the `MDeq`
-            """
-            deq.inner.insert(index, element)
-            return Ok(None)
-
-        return inner
-
-    return get_at
-
-
-def copy[T](deq: MDeq[T]) -> MDeq[T]:
+def copy(deq: MDeq[Val]) -> MDeq[Val]:
     """
     Returns a shallow copy of the `MDeq` as a new object.
     """
     return new(*deq.inner.copy())
 
 
 @null_and_error_safe(IndexError)
-def pop[T](deq: MDeq[T]) -> T:
+def pop(deq: MDeq[Val]) -> Val:
     """
     Removes and returns the last element in an `MDeq` if it exists.
     """
     return deq.inner.pop()
 
 
 @null_and_error_safe(IndexError)
-def popleft[T](deq: MDeq[T]) -> T:
+def popleft(deq: MDeq[Val]) -> Val:
     """
     Removes and returns the first element in an `MDeq` if it exists.
     """
     return deq.inner.popleft()
 
 
 @null_and_error_safe(IndexError)
-def first[T](deq: MDeq[T]) -> T:
+def first(deq: MDeq[Val]) -> Val:
     """
     Returns the first element in an `MDeq` if it exists.
     """
     return deq.inner[0]
 
 
 @null_and_error_safe(IndexError)
-def last[T](deq: MDeq[T]) -> T:
+def last(deq: MDeq[Val]) -> Val:
     """
     Returns the last element in an `MDeq` if it exists.
     """
     return deq.inner[-1]
 
 
-def at(index: int):
+
+@two
+@null_and_error_safe(IndexError)
+def at(index: int, deq: MDeq[Val]) -> Val:
     """
     Returns the element at the provided index in an `MDeq` if it exists.
     """
+    return deq.inner[index]
 
-    @null_and_error_safe(IndexError)
-    def inner[T](deq: MDeq[T]) -> T:
-
-        return deq.inner[index]
 
-    return inner
-
-
-def remove(index: int):
+@two
+@safe(IndexError)
+def remove(index: int, deq: MDeq[Val]) -> None:
     """
     Removes the element from the `MDeq` if it exists at the given index.
     """
-
-    @safe(IndexError)
-    def inner[T](deq: MDeq[T]) -> None:
-
-        del deq.inner[index]
-
-    return inner
+    del deq.inner[index]
 
 
-def extend[T](src: Iterable[T]):
+@two
+def extend(src: Iterable[Val], tgt: MDeq[Val]) -> Ok[None]:
     """
     Combines an iterable with a provided `MDeq` with all new elements being appended.
     """
 
-    def inner(tgt: MDeq[T]) -> Ok[None]:
+    tgt.inner.extend(src)
+    return Ok(None)
 
-        tgt.inner.extend(src)
-        return Ok(None)
 
-    return inner
-
-
-def extendleft[T](src: Iterable[T]):
+@two
+def extendleft(src: Iterable[Val], tgt: MDeq[Val]) -> Ok[None]:
     """
     Combines an iterable with a provided `MDeq` with all new elements going first.
     """
 
-    def inner(tgt: MDeq[T]) -> Ok[None]:
-
-        tgt.inner.extendleft(src)
-        return Ok(None)
-
-    return inner
+    tgt.inner.extendleft(src)
+    return Ok(None)
 
 
-def index[T](find: T, start: int = 1):
+def index(find: Val, start: int = 1):
     """
     Retrieves the index of the provide dvalue, if it exists.
     """
 
     @null_and_error_safe(ValueError)
-    def inner(deq: MDeq[T]) -> int:
+    def inner(deq: MDeq[Val]) -> int:
 
         return deq.inner.index(find, start)
 
     return inner
```

### Comparing `pythonix-1.0.1/pythonix/internals/op.py` & `pythonix-1.0.2/pythonix/internals/op.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """
 Functions used to operate over data structures
 """
-from typing import Callable, Iterable, Iterator, Any, SupportsIndex
+from typing import Callable, Iterable, Iterator, Any, SupportsIndex, TypeVar
 from functools import reduce
 from pythonix.internals.res import null_and_error_safe
 
+Val = TypeVar('Val')
+SecondVal = TypeVar('SecondVal')
+NewVal = TypeVar('NewVal')
 
-def filterx[T](using: Callable[[T], bool]) -> Callable[[Iterable[T]], Iterator[T]]:
+def filterx(using: Callable[[Val], bool]) -> Callable[[Iterable[Val]], Iterator[Val]]:
     """
     Filter over an `Iterable` with a function that takes each of its elements and returns a True or False.
     True evaluations are kept while False are not kept in the result.
     """
-    def get_data(iterable: Iterable[T]) -> filter[T]:
+    def get_data(iterable: Iterable[Val]) -> filter[Val]:
 
         return filter(using, iterable)
 
     return get_data
 
 
-def mapx[T, U](using: Callable[[T], U]) -> Callable[[Iterable[T]], Iterator[U]]:
+def mapx(using: Callable[[Val], NewVal]) -> Callable[[Iterable[Val]], Iterator[NewVal]]:
     """
     Run the `using` function over an `Iterable` and return an `Iterator` containing the result 
     """
-    def get_data(iterable: Iterable[T]) -> map[U]:
+    def get_data(iterable: Iterable[Val]) -> map[NewVal]:
 
         return map(using, iterable)
 
     return get_data
 
 
-def reducex[
-    S, T, U
-](using: Callable[[S, T], U]) -> Callable[[Iterable[S | T]], Iterator[U]]:
+def reducex(using: Callable[[Val, SecondVal], NewVal]) -> Callable[[Iterable[Val | SecondVal]], Iterator[NewVal]]:
     """
     Run a function that takes two arguments over an `Iterable` to produce a single result. 
     """
-    def get_data(iterable: Iterable[S | T]) -> reduce[U]:
+    def get_data(iterable: Iterable[Val | SecondVal]) -> reduce[NewVal]:
 
         return reduce(using, iterable)
 
     return get_data
 
 
-def attr[U](name: str, type_hint: type[U] = Any):
+def attr(name: str, type_hint: type[NewVal] = Any):
     """
     Used to safely retrieve attributes from classes in a functional way.
     Can be used with a `type_hint` parameter to provide better type hint support.
     #### Example
     ```python
     from pythonix import Res
     from collections import namedtuple
@@ -58,15 +59,15 @@
 
     assert x.inner = 5
     assert z.inner is Nil
     ```
     """
 
     @null_and_error_safe(AttributeError)
-    def inner[T](obj: T) -> U:
+    def inner(obj: Val) -> NewVal:
         return getattr(obj, name)
 
     return inner
 
 
 def item(index: SupportsIndex):
     """
@@ -82,11 +83,11 @@
 
     assert x.inner = 5
     assert z.inner is Nil
     ```
     """
 
     @null_and_error_safe(IndexError, KeyError)
-    def inner[T](iterable: Iterable[T]) -> T:
+    def inner(iterable: Iterable[Val]) -> Val:
         return iterable[index]
 
     return inner
```

### Comparing `pythonix-1.0.1/pythonix/internals/pair.py` & `pythonix-1.0.2/pythonix/internals/pair.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 """
 Module for handling key value pairs.
 """
 
-from typing import NamedTuple, Tuple, TypeVar
+from typing import NamedTuple, Tuple, TypeVar, Generic, TypeAlias
 from pythonix.internals.types import Fn
+from pythonix.internals.curry import two
 
-type Pairs[V] = Tuple[Pair[V], ...]
 
-T = TypeVar("T")
+Val = TypeVar('Val')
+NewVal = TypeVar('NewVal')
+KeyStr: TypeAlias = str
 
-class Pair[V](NamedTuple):
+class Pair(Generic[Val], NamedTuple):
     """
     A typed key value pair whose key is a `str`
     """
     key: str
-    value: V
+    value: Val
 
+Pairs: TypeAlias = Tuple[Pair[Val], ...]
 
-def new[V](key: str) -> Fn[V, Pair[V]]:
+@two
+def new(key: KeyStr, value: Val) -> Pair[Val]:
     """
-    Create a new `Pair` safely 
+    Create a new key value `Pair` safely 
     """
-    def get_value(value: V):
+    return Pair(key, value)
 
-        return Pair(key, value)
-
-    return get_value
-
-
-def set_key(key: str):
+@two
+def set_key(key: KeyStr, pair: Pair[Val]) -> Pair[Val]:
     """
     Creates a new `Pair` from a provided one with the provided key.
     """
-    def get_pair[V](pair: Pair[V]) -> Pair[V]:
+    return new(key)(pair.value)
 
-        return new(key)(pair.value)
 
-    return get_pair
-
-
-def set_value[W](value: W):
+@two
+def set_value(value: NewVal, pair: Pair[Val]) -> Pair[NewVal]:
     """
     Creates a new `Pair` with a new value, preserving its key.
     """
-    def get_pair[V](pair: Pair[V]) -> Pair[W]:
-
-        return new(pair.key)(value)
+    return new(pair.key)(value)
 
-    return get_pair
 
-def get_value[V](pair: Pair[V]) -> V:
+def get_value(pair: Pair[Val]) -> Val:
     """
     Retrieves the `value` of a provided `Pair`
     """
     return pair.value
 
-def get_key[V](pair: Pair[V]) -> str:
+def get_key(pair: Pair[Val]) -> KeyStr:
     """
     Retrieves the `key` of a provided `Pair`
     """
     return pair.key
 
 
-def map[V, W](using: Fn[V, W]):
+@two
+def map(using: Fn[Val, NewVal], pair: Pair[Val]) -> Pair[NewVal]:
     """
     Change the inner value of a `Pair` with a function
     """
-    def inner(pair: Pair[V]) -> Pair[W]:
-        return set_value(using(pair.value))(pair)
-    
-    return inner
+    return set_value(using(pair.value))(pair)
```

### Comparing `pythonix-1.0.1/pythonix/internals/pipe.py` & `pythonix-1.0.2/pythonix/internals/pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
-from typing import Callable, Protocol, Tuple, overload
+from typing import Callable, Protocol, Tuple, overload, TypeVar, Generic
 from pythonix.internals import trail
 from pythonix.internals.trail import Trail, Log
-from functools import singledispatch
 
+Val = TypeVar('Val')
+NewVal = TypeVar('NewVal')
 
-class HasInner[T](Protocol):
 
-    inner: T
+class HasInner(Generic[Val], Protocol):
 
+    inner: Val
 
-class Bind[T]:
+
+class Bind(Generic[Val]):
     """
     Container that allows sequential functions calls to change its inner value and type.
     Transformations can be done with with either the `run` or `__call__` methods.
     #### Example
     ```python
     y: bool = (
         Bind(5)
@@ -25,37 +27,37 @@
     ```
     #### Methods
     - `run(Fn(T) -> U) -> Bind<U>`: Runs the provided function and returns a new `Bind` object containing
     its result
     - `__call__(Fn(T) -> U) -> Bind<U>`: Identical to the `run` function.
     """
 
-    inner: T
+    inner: Val
 
-    def __init__(self, inner: T) -> None:
+    def __init__(self, inner: Val) -> None:
         self.inner = inner
 
-    def run[U](self, using: Callable[[T], U]) -> Bind[U]:
+    def run(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
         """
         Performs a transformation on the contained value using the function provided.
         Returns a new `Bind` object containing the new value. Works only with single arity
         functions.
         """
         return Bind(using(self.inner))
 
-    def __call__[U](self, using: Callable[[T], U]) -> Bind[U]:
+    def __call__(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
         """
         Performs a transformation on the contained value using the function provided.
         Returns a new `Bind` object containing the new value. Works only with single arity
         functions.
         """
         return Bind(using(self.inner))
 
 
-class Do[T]:
+class Do(Generic[Val]):
     """
     Container used to run arbitrary functions on an `inner` value without changing its
     state. Useful for logging, printing, or other inconsequential side effects.
     #### Example
     ```python
     do: Do[int] = Do(5)
     (
@@ -67,64 +69,60 @@
     assert do.inner == 5
     ```
     #### Methods
     - `run(Fn(T) -> U) -> Do[T]`: Runs the provided function on the contained value and returns itself.
     - `__call__(Fn(T) -> U) -> Do[T]`: Identical to the `run` function.
     """
 
-    inner: T
+    inner: Val
 
-    def __init__(self, inner: T) -> None:
+    def __init__(self, inner: Val) -> None:
         self.inner = inner
 
-    def run[U](self, using: Callable[[T], U]) -> Do[T]:
+    def run(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
         """
         using(self.inner)
         return self
 
-    def __call__[U](self, using: Callable[[T], U]) -> Do[T]:
+    def __call__(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
         """
         return self.run(using)
 
 
-class Blaze[T]:
+class Blaze(Generic[Val]):
     """
     `Bind` container used to accumulate log messages during runtime without
     side effects to the functions being ran. Runs functions with an optional
     log message attached. If the function being called returns a `Trail` log container,
     then it will attach its logs to the currently accumulated logs.
     """
 
     logs: Tuple[Log, ...] = tuple()
-    inner: trail.Trail[T]
+    inner: trail.Trail[Val]
 
-    def __init__(self, inner: T | Trail[T], *logs: Log):
+    def __init__(self, inner: Val | Trail[Val], *logs: Log):
         match inner:
             case Trail():
                 self.inner = inner
                 self.logs = logs + inner.logs
             case _:
                 self.inner = trail.new()(inner)
                 self.logs = logs
 
     @overload
-    def __call__[
-        U
-    ](self, using: Callable[[T], trail.Trail[U]], *logs: Log) -> Blaze[U]: ...
+    def __call__(self, using: Callable[[Val], trail.Trail[NewVal]], *logs: Log) -> Blaze[NewVal]: ...
 
     @overload
-    def __call__[U](self, using: Callable[[T], U], *logs: Log) -> Blaze[U]: ...
+    def __call__(self, using: Callable[[Val], NewVal], *logs: Log) -> Blaze[NewVal]: ...
 
-    def __call__[
-        U
-    ](self, using: Callable[[T], trail.Trail[U] | U], *logs: Log) -> Blaze[U]:
+    def __call__(self, using: Callable[[Val], trail.Trail[NewVal] | NewVal], *logs: Log) -> Blaze[NewVal]:
         """
         Call the function and attach the logs from the function `Trail` and the optional logs
         to the new instance of `Blaze` containing the result.
         """
         return Blaze(using(self.inner.inner), *(self.logs + logs))
```

### Comparing `pythonix-1.0.1/pythonix/internals/req.py` & `pythonix-1.0.2/pythonix/internals/req.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import NamedTuple, ParamSpec, Callable, Tuple
+from typing import NamedTuple, ParamSpec, Callable, Tuple, TypeVar
 from pythonix.op import mapx
 from pythonix.pipe import Bind
 from pythonix.res import Res
 import pythonix.pair as pair
 from functools import singledispatch
 from requests import (
-    get as _get,
-    post as _post,
-    put as _put,
-    delete as _delete,
+    get      as _get,
+    post     as _post,
+    put      as _put,
+    delete   as _delete,
     Response as OGResponse,
     HTTPError
 )
 from pythonix.internals.pair import Pair, Pairs
 from pythonix.internals.pipe import Bind
 from pythonix import res
 
@@ -48,14 +48,16 @@
     Request type to be sent via an HTTP method
     """
     url: str
     headers: Pairs[bytes]
     params: Pairs[bytes]
     data: Pairs[bytes]
 
+RequestType = TypeVar('RequestType', bound='Request')
+
 class Get(Request):
     """
     An HTTP request set as a `GET`
     """
     method: Callable[P, Response] = _get
 
 class Post(Request):
@@ -82,15 +84,15 @@
     return bytes(value)
 
 @to_bytes.register(str)
 def _(value: str) -> bytes:
     return bytes(value, 'utf-8')
 
 
-def set_value_to_bytes[V](keyvalue: Pair[str | int]) -> Pair[bytes]:
+def set_value_to_bytes(keyvalue: Pair[str | int]) -> Pair[bytes]:
     Bind(keyvalue)(pair.map(to_bytes)).inner
 
 
 def get(url: str):
     """
     Set the URL for the request type
     """
@@ -258,21 +260,21 @@
     def get_content[R: (Request)](content: R) -> R:
 
         return content.__class__(content.url, content.headers, content.params, data)
 
     return get_content
 
 
-def body[R: (Request)](content: R) -> Tuple[Pair[bytes], ...]:
+def body(content: RequestType) -> Tuple[Pair[bytes], ...]:
     """
     Combines the headers, params, and content of `Request`
     """
     return content.headers + content.params + content.data
 
-def send[R: (Request)](request: R) -> Res[Response, HTTPError]:
+def send(request: RequestType) -> Res[Response, HTTPError]:
     """
     Sends the provided `Request` and then parses its response, capturing any errors that occur.
     """
     return (
         Bind(request)
         (body)
         (lambda body: {'url': request.url} | {k: v for k, v in body})
```

### Comparing `pythonix-1.0.1/pythonix/internals/trail.py` & `pythonix-1.0.2/pythonix/internals/trail.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import NamedTuple, Tuple, Callable, ParamSpec
+from typing import NamedTuple, Tuple, Callable, ParamSpec, TypeVar, Generic
 from datetime import datetime, timezone
-from abc import ABCMeta
-from enum import Enum
 
 P = ParamSpec("P")
-
+LogType = TypeVar('LogType', bound='Log')
+Val = TypeVar('Val')
+NewVal = TypeVar('NewVal')
 
 class Log(NamedTuple):
     datetime: datetime
     message: str
 
     def __str__(self) -> str:
         return f'{self.__class__.__name__}("{self.datetime.strftime('%Y-%m-%dT%H:%M:%SZ')}", "{self.message}")'
@@ -25,19 +25,19 @@
 class Error(Log):
     ...
 
 class Critical(Log):
     ...
 
 
-def log[L: (Log)](log_type: type[L]):
+def log(log_type: type[LogType]):
     """
     Creates a new `Log` instance with the specified message attached
     """
-    def inner(message: str) -> L:
+    def inner(message: str) -> LogType:
         """
         Attach a message to the log 
         """
         return log_type(datetime.now(timezone.utc), message)
 
     return inner
 
@@ -45,62 +45,62 @@
 debug = log(Debug)
 info = log(Info)
 warning = log(Warning)
 error = log(Error)
 critical = log(Critical)
 
 
-class Trail[T](NamedTuple):
+class Trail(Generic[Val], NamedTuple):
     """
     Container type used to wrap a value with a series of `Log` type records
     """
     logs: Tuple[Log, ...]
-    inner: T
+    inner: Val
 
 
-def new[L: (Log)](*logs: L):
+def new(*logs: LogType):
     """
     Create a new `Trail` object with the desired logs attached.
     """
-    def get_inner[T](inner: T) -> Trail[T]:
+    def get_inner(inner: Val) -> Trail[Val]:
         """
         Attach the wrapped value to the `Trail`
         """
         return Trail(logs, inner)
 
     return get_inner
 
 
-def append[L: (Log)](*logs: L):
+def append(*logs: LogType):
     """
     Append a new series of logs to a `Trail`
     """
-    def inner[T](trail: Trail[T]) -> Trail[T]:
+    def inner(trail: Trail[Val]) -> Trail[Val]:
 
         return new(*(trail.logs + logs))(trail.inner)
 
     return inner
 
 
-def logs[T, L: (Log)](trail: Trail[T]) -> Tuple[L, ...]:
+def logs(trail: Trail[Val]) -> Tuple[LogType, ...]:
     """
     Convenience function to return the logs of a `Trail`
     """
     return trail.logs
 
 
-def trail[L: (Log)](*logs: L):
+def trail(*logs: LogType):
     """
     Decorator function used to wrap the output of a function with a default set of logs.
     This also changes the output of the function to return a `Trail` of the type returned
     by the function.
     """
-    def inner[U](func: Callable[P, U]):
+    def inner(func: Callable[P, NewVal]):
 
-        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Trail[U]:
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Trail[NewVal]:
 
             return new(*logs)(func(*args, **kwargs))
 
         return wrapper
 
     return inner
```

### Comparing `pythonix-1.0.1/pythonix/internals/tuple.py` & `pythonix-1.0.2/pythonix/internals/tuple.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,113 @@
 """
 Module for handling tuples without risk of panics
 """
-from typing import Tuple
+from typing import Tuple, TypeVar
 from pythonix.op import item
 from pythonix.res import safe, null_and_error_safe
+from pythonix.curry import two, three
 from enum import Enum
 
+Val = TypeVar('Val')
+NewVal = TypeVar('NewVal')
+type IndexInt = int
 
 class Side(Enum):
     LEFT: str = "LEFT"
     RIGHT: str = "RIGHT"
 
 
-def new[T](*elements: T) -> Tuple[T, ...]:
+def new(*elements: Val) -> Tuple[Val, ...]:
     """
     Convenience function to create a new series of data of a given type
     """
     return elements
 
 
 def push(side: Side = Side.RIGHT):
     """
     Push an element to either side of a `Tuple`
     """
-    def get_element[U](element: U):
+    def get_element(element: NewVal):
         
-        def inner[T](tuples: Tuple[T, ...]) -> Tuple[T | U, ...]:
+        def inner(tuples: Tuple[Val, ...]) -> Tuple[Val | NewVal, ...]:
 
             match side:
                 case Side.LEFT:
                     return (element,) + tuples
                 case Side.RIGHT:
                     return tuples + (element,)
 
         return inner
 
     return get_element
 
 
-def get(index: int):
+@two
+def get(index: IndexInt, tuples: Tuple[Val, ...]):
     """
     Retrieve an element from a `Tuple` at the provided index
     """
-    def inner[T](tuples: Tuple[T, ...]):
-
-        return item(index)(tuples)
-
-    return inner
+    return item(index)(tuples)
 
 
 def extend(side: Side = Side.RIGHT):
     """
     Combine two tuple series together
     """
-    def get_left[T](new: Tuple[T, ...]):
+    def get_left(new: Tuple[Val, ...]):
 
-        def get_right[U](old: Tuple[U, ...]) -> Tuple[T | U, ...]:
+        def get_right(old: Tuple[NewVal, ...]) -> Tuple[Val | NewVal, ...]:
 
             match side:
                 case Side.LEFT:
                     return new + old
                 case Side.RIGHT:
                     return old + new
 
         return get_right
 
     return get_left
 
 
-def index[T](element: T):
+@two
+@null_and_error_safe(ValueError)
+def index(element: Val, tuples: Tuple[Val, ...]) -> int:
     """
     Find the index of an element in `Tuple` if it exists
     """
-    @null_and_error_safe(ValueError)
-    def inner(tuples: Tuple[T, ...]) -> int:
-
-        return tuples.index(element)
-
-    return inner
+    return tuples.index(element)
 
 
-def count_occurrences[T](value: T):
+@two
+def count_occurrences(value: Val, tuples: Tuple[Val, ...]) -> int:
     """
     Count the occurrences of the provided value in a `Tuple`
     """
-    def inner(tuples: Tuple[T, ...]) -> int:
+    return tuples.count(value)
 
-        return tuples.count(value)
 
-    return inner
-
-
-def insert(index: int):
+@three
+def insert(index: IndexInt, insert: NewVal, tuples: Tuple[Val, ...]) -> Tuple[Val | NewVal, ...]:
     """
     Recreate the `Tuple` with the provided element at the index
     """
-    def new_item[U](insert: U):
-
-        def inner[T](tuples: Tuple[T, ...]) -> Tuple[T | U, ...]:
-            return tuples[:index] + (insert,) + tuples[index:]
-        
-        return inner
-    
-    return new_item
+    return tuples[:index] + (insert,) + tuples[index:]
 
 
-def remove(index: int):
+@two
+@safe(IndexError)
+def remove(index: IndexInt, tuples: Tuple[Val, ...]) -> Tuple[Val, ...]:
     """
     Recreate the `Tuple` without the element at the provided index
     """
-    @safe(IndexError)
-    def inner[T](tuples: Tuple[T, ...]) -> Tuple[T, ...]:
-        if index > (length := len(tuples)):
-            raise IndexError(f'Incompatible index {index} is greater than length {length}')
-        return tuples[:index] + tuples[index+1:] 
-    return inner
+    if index > (length := len(tuples)):
+        raise IndexError(f'Incompatible index {index} is greater than length {length}')
+    return tuples[:index] + tuples[index+1:] 
 
 
 push_left = push(Side.LEFT)
 push_right = push(Side.RIGHT)
-last = get(-1)
-first = get(0)
 extend_left = extend(Side.LEFT)
 extend_right = extend(Side.RIGHT)
+last = get(-1)
+first = get(0)
```

### Comparing `pythonix-1.0.1/pythonix/pipe.py` & `pythonix-1.0.2/pythonix/pipe.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/pythonix/req.py` & `pythonix-1.0.2/pythonix/req.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.1/PKG-INFO` & `pythonix-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pythonix
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: jhok2013
 Author-email: jhok2013@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PYTHONIX
 
 A collection of functional modules in Python 12 inspired by Gleam and Rust.
 If you have like functional programming, but have to program in Python, then check this out.
 
 ## Features
 
 1. Exceptions as values support similar to Rust
 2. Emphasis on immutable types
 3. Great support for immutable data structures
-4. Wrapper types to enable consecutive function calls via pipes
+4. Wrapper types to enable consecutive function calls via pipelike types
 5. Strongly typed hints with generic support
 6. Emphasis on composability with partially applied functions
 7. Emphasis on removing nullability
 
 ## Examples
 
 ### Piping with Bind and Do
@@ -53,21 +54,27 @@
 ```
 
 ### Error as Value
 ```python
 from pythonix.prelude import *
 from pythonix.res import Res
 
-# Capture errors as types
+# Capture errors as types with the res decorators
 @res.safe(TypeError)
 def foo(bar: int) -> int:
     if not isinstance(bar, int):
         raise TypeError("Invalid type")
     return bar
 
+# Make functions that return `Ok` or `Err` to show the possibility of failure
+def far(boo: int) -> Res[int, TypeError]:
+    if not isinstance(boo, int):
+        return Err(TypeError("Invalid type"))
+    return Ok(boo)
+
 # The result is captured to show errors and success
 bar: Res[int, TypeError] = foo(5)
 
 # Pipe through consecutive functions to handle errors
 bar: int = (
     pipe.Bind(bar)
     (res.map(lambda x: x + 5))
```

