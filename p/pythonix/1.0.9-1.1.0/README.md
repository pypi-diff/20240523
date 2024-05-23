# Comparing `tmp/pythonix-1.0.9.tar.gz` & `tmp/pythonix-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.9.tar", max compression
+gzip compressed data, was "pythonix-1.1.0.tar", max compression
```

## Comparing `pythonix-1.0.9.tar` & `pythonix-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.9/README.md
--rw-r--r--   0        0        0      409 2024-05-21 15:50:26.570000 pythonix-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       24 2024-05-16 16:50:54.529631 pythonix-1.0.9/pythonix/__init__.py
--rw-r--r--   0        0        0      610 2024-05-21 03:33:06.740000 pythonix-1.0.9/pythonix/curry.py
--rw-r--r--   0        0        0      596 2024-05-21 15:33:42.330000 pythonix-1.0.9/pythonix/deq.py
--rw-r--r--   0        0        0      709 2024-05-21 03:10:17.490000 pythonix-1.0.9/pythonix/dict_utils.py
--rw-r--r--   0        0        0      759 2024-05-19 18:08:28.990000 pythonix-1.0.9/pythonix/fn.py
--rw-r--r--   0        0        0     1528 2024-05-21 02:08:58.640000 pythonix-1.0.9/pythonix/grammar.py
--rw-r--r--   0        0        0       28 2024-05-16 16:50:54.529631 pythonix-1.0.9/pythonix/internals/__init__.py
--rw-r--r--   0        0        0    10528 2024-05-21 03:32:59.410000 pythonix-1.0.9/pythonix/internals/curry.py
--rw-r--r--   0        0        0     6837 2024-05-21 15:33:22.620000 pythonix-1.0.9/pythonix/internals/deq.py
--rw-r--r--   0        0        0     4445 2024-05-21 15:46:17.730000 pythonix-1.0.9/pythonix/internals/dict_utils.py
--rw-r--r--   0        0        0     5075 2024-05-21 14:24:24.050000 pythonix-1.0.9/pythonix/internals/fn.py
--rw-r--r--   0        0        0    11058 2024-05-19 18:33:10.620000 pythonix-1.0.9/pythonix/internals/grammar.py
--rw-r--r--   0        0        0    10393 2024-05-17 17:21:29.129631 pythonix-1.0.9/pythonix/internals/op.py
--rw-r--r--   0        0        0     4844 2024-05-17 17:24:14.659631 pythonix-1.0.9/pythonix/internals/pair.py
--rw-r--r--   0        0        0     6534 2024-05-21 14:22:43.100000 pythonix-1.0.9/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     1968 2024-05-18 19:03:33.219631 pythonix-1.0.9/pythonix/internals/prove.py
--rw-r--r--   0        0        0     7203 2024-05-16 16:50:54.819631 pythonix-1.0.9/pythonix/internals/req.py
--rw-r--r--   0        0        0    25292 2024-05-21 02:06:29.580000 pythonix-1.0.9/pythonix/internals/res.py
--rw-r--r--   0        0        0     5041 2024-05-16 19:09:41.649631 pythonix-1.0.9/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2726 2024-05-16 21:05:40.149631 pythonix-1.0.9/pythonix/internals/tup.py
--rw-r--r--   0        0        0     1356 2024-05-17 04:15:47.249631 pythonix-1.0.9/pythonix/op.py
--rw-r--r--   0        0        0      698 2024-05-17 17:26:00.459631 pythonix-1.0.9/pythonix/pair.py
--rw-r--r--   0        0        0      876 2024-05-17 18:24:21.269631 pythonix-1.0.9/pythonix/pipe.py
--rw-r--r--   0        0        0      755 2024-05-21 15:50:13.600000 pythonix-1.0.9/pythonix/prelude.py
--rw-r--r--   0        0        0      210 2024-05-16 16:50:54.639631 pythonix-1.0.9/pythonix/prove.py
--rw-r--r--   0        0        0      645 2024-05-16 16:24:04.869631 pythonix-1.0.9/pythonix/req.py
--rw-r--r--   0        0        0     1370 2024-05-21 02:08:25.030000 pythonix-1.0.9/pythonix/res.py
--rw-r--r--   0        0        0      290 2024-05-16 16:50:54.669631 pythonix-1.0.9/pythonix/trail.py
--rw-r--r--   0        0        0      358 2024-05-16 16:50:54.679631 pythonix-1.0.9/pythonix/tup.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    10372 2024-05-23 15:34:25.310000 pythonix-1.1.0/README.md
+-rw-r--r--   0        0        0      389 2024-05-23 15:40:20.500000 pythonix-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1544 2024-05-22 19:57:42.800000 pythonix-1.1.0/pythonix/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-23 15:27:03.550000 pythonix-1.1.0/pythonix/curry.py
+-rw-r--r--   0        0        0      655 2024-05-23 15:27:03.550000 pythonix-1.1.0/pythonix/deq.py
+-rw-r--r--   0        0        0      709 2024-05-21 20:22:32.650000 pythonix-1.1.0/pythonix/dict_utils.py
+-rw-r--r--   0        0        0      759 2024-05-19 18:08:28.990000 pythonix-1.1.0/pythonix/fn.py
+-rw-r--r--   0        0        0     1547 2024-05-21 20:14:22.540000 pythonix-1.1.0/pythonix/grammar.py
+-rw-r--r--   0        0        0      131 2024-05-21 20:58:42.120000 pythonix-1.1.0/pythonix/internals/__init__.py
+-rw-r--r--   0        0        0    10532 2024-05-23 15:27:04.050000 pythonix-1.1.0/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     7122 2024-05-23 15:27:03.770000 pythonix-1.1.0/pythonix/internals/deq.py
+-rw-r--r--   0        0        0     4544 2024-05-23 15:27:03.760000 pythonix-1.1.0/pythonix/internals/dict_utils.py
+-rw-r--r--   0        0        0     5075 2024-05-21 14:24:24.050000 pythonix-1.1.0/pythonix/internals/fn.py
+-rw-r--r--   0        0        0    11068 2024-05-22 19:33:07.080000 pythonix-1.1.0/pythonix/internals/grammar.py
+-rw-r--r--   0        0        0     6021 2024-05-23 15:27:03.770000 pythonix-1.1.0/pythonix/internals/op.py
+-rw-r--r--   0        0        0     3949 2024-05-21 20:56:16.430000 pythonix-1.1.0/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     2242 2024-05-23 15:27:03.620000 pythonix-1.1.0/pythonix/internals/prove.py
+-rw-r--r--   0        0        0     7726 2024-05-21 20:44:23.210000 pythonix-1.1.0/pythonix/internals/req.py
+-rw-r--r--   0        0        0    26705 2024-05-23 15:27:04.130000 pythonix-1.1.0/pythonix/internals/res.py
+-rw-r--r--   0        0        0     6578 2024-05-23 15:28:09.360000 pythonix-1.1.0/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     4145 2024-05-23 15:27:03.840000 pythonix-1.1.0/pythonix/internals/tup.py
+-rw-r--r--   0        0        0      876 2024-05-22 19:59:59.230000 pythonix-1.1.0/pythonix/op.py
+-rw-r--r--   0        0        0      598 2024-05-21 20:56:38.560000 pythonix-1.1.0/pythonix/pair.py
+-rw-r--r--   0        0        0     1564 2024-05-23 15:27:03.650000 pythonix-1.1.0/pythonix/prelude.py
+-rw-r--r--   0        0        0      477 2024-05-22 20:00:27.470000 pythonix-1.1.0/pythonix/prove.py
+-rw-r--r--   0        0        0     1402 2024-05-22 20:01:30.780000 pythonix-1.1.0/pythonix/res.py
+-rw-r--r--   0        0        0     1082 2024-05-23 15:27:03.670000 pythonix-1.1.0/pythonix/trail.py
+-rw-r--r--   0        0        0      649 2024-05-22 20:02:18.790000 pythonix-1.1.0/pythonix/tup.py
+-rw-r--r--   0        0        0    10903 1970-01-01 00:00:00.000000 pythonix-1.1.0/PKG-INFO
```

### Comparing `pythonix-1.0.9/pythonix/curry.py` & `pythonix-1.1.0/pythonix/curry.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,8 +18,18 @@
     ...     return delimiter.join(iterable)
     ...
     >>> join_curry = two(join)
     >>> join_curry(', ')(['hello', 'world'])
     'hello, world'
 
 """
-from pythonix.internals.curry import two, three, four, five, six, seven, eight, nine, to_end_two
+from pythonix.internals.curry import (
+    two,
+    three,
+    four,
+    five,
+    six,
+    seven,
+    eight,
+    nine,
+    to_end_two,
+)
```

### Comparing `pythonix-1.0.9/pythonix/deq.py` & `pythonix-1.1.0/pythonix/deq.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 Does not return copies of the ``deque``, but instead mutable references
 to the ``deq`` it recieves. A useful data structure with thread safe
 appends and pops.
 
 Examples: ::
 
+    >>> from pythonix.internals.res import unpack
     >>> deq = new(1, 2, 3)
-    >>> val, nil = get(0)(deq)
+    >>> val, nil = unpack(get(0)(deq))
     >>> val
     1
 
 """
 from pythonix.internals.deq import (
     new,
     get,
@@ -27,9 +28,9 @@
     append,
     appendleft,
     remove,
     reverse,
     rotate,
     maxlen,
     clear,
-    count
+    count,
 )
```

### Comparing `pythonix-1.0.9/pythonix/dict_utils.py` & `pythonix-1.1.0/pythonix/dict_utils.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.9/pythonix/fn.py` & `pythonix-1.1.0/pythonix/fn.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.9/pythonix/grammar.py` & `pythonix-1.1.0/pythonix/grammar.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,8 +62,10 @@
     PipeInfix,
     PipePrefix,
     PipeApplyInfix,
     PipeApplyPrefix,
     PipeApplySuffix,
     Piper,
     P,
+    do,
+    inner,
 )
```

### Comparing `pythonix-1.0.9/pythonix/internals/curry.py` & `pythonix-1.1.0/pythonix/internals/curry.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,30 @@
 assignments.remove("__annotations__")
 updated_assignments = WRAPPER_ASSIGNMENTS
 # updated_assignments = tuple(assignments)
 
 
 def to_end_two(func: Callable[[T1, T2], U]) -> Callable[[T2, T1], U]:
     """Moves the first arg of a two function argument to be the last instead
-    
+
     Examples: ::
 
         >>> @to_end_two
         ... def join(iterable: list[str], delimiter: str) -> str:
         ...     return delimiter.join(iterable)
         ...
         >>> join(', ', ['hello', 'world'])
         'hello, world'
-    
+
     """
+
     @wraps(func)
     def wrapped(t2: T2, t1: T1) -> U:
         return func(t1, t2)
-    
+
     return wrapped
 
 
 def two(func: Callable[[T1, T2], U]) -> Callable[[T1], Callable[[T2], U]]:
     """Turns a function of two args to a curried one with the same return type
 
     Example: ::
@@ -74,28 +75,30 @@
         >>> add(10)(10)
         20
         >>> add_10 = add(10)
         >>> add_10(20)
         30
 
     """
+
     @wraps(func, assigned=updated_assignments)
     def in1(t1: T1) -> Callable[[T2], U]:
         def in2(t2: T2) -> U:
             return func(t1, t2)
 
         return in2
 
     return in1
 
 
 def three(
     func: Callable[[T1, T2, T3], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], U]]]:
     """Same as ``two``, but handles three arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], U]]:
         def in2(t2: T2) -> Callable[[T3], U]:
             def in3(t3: T3) -> U:
                 return func(t1, t2, t3)
 
             return in3
@@ -105,34 +108,36 @@
     return in1
 
 
 def four(
     func: Callable[[T1, T2, T3, T4], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], U]]]]:
     """Same as ``two``, but handles four arguments"""
+
     @wraps(four)
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], U]]]:
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], U]]:
             def in3(t3: T3) -> Callable[[T4], U]:
                 def in4(t4: T4) -> U:
-                    func(t1, t2, t3, t4)
+                    return func(t1, t2, t3, t4)
 
                 return in4
 
             return in3
 
         return in2
 
     return in1
 
 
 def five(
     func: Callable[[T1, T2, T3, T4, T5], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]]:
     """Same as ``two``, but handles five arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]:
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], U]]]:
             def in3(t3: T3) -> Callable[[T4], Callable[[T5], U]]:
                 def in4(t4: T4) -> Callable[[T5], U]:
@@ -153,14 +158,15 @@
 def six(
     func: Callable[[T1, T2, T3, T4, T5, T6], U]
 ) -> Callable[
     [T1],
     Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]],
 ]:
     """Same as ``two``, but handles six arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]
     ]:
         def in2(
@@ -193,14 +199,15 @@
         [T2],
         Callable[
             [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
         ],
     ],
 ]:
     """Same as ``two``, but handles seven arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
@@ -246,14 +253,15 @@
             Callable[
                 [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
             ],
         ],
     ],
 ]:
     """Same as ``two``, but handles eight arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3],
@@ -318,14 +326,15 @@
                     Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
                 ],
             ],
         ],
     ],
 ]:
     """Same as ``two``, but handles nine arguments"""
+
     @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3],
```

### Comparing `pythonix-1.0.9/pythonix/internals/deq.py` & `pythonix-1.1.0/pythonix/internals/deq.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 Does not return copies of the ``deque``, but instead mutable references
 to the ``deq`` it recieves. A useful data structure with thread safe
 appends and pops.
 
 Examples: ::
 
     >>> deq = new(1, 2, 3)
-    >>> val, nil = get(0)(deq)
+    >>> val, nil = unpack(get(0)(deq))
     >>> val
     1
 
 """
 from collections import deque as deque
-from typing import Iterable, TypeVar
+from typing import Iterable, TypeVar, cast, SupportsIndex
 from pythonix.internals.res import null_and_error_safe, safe, null_safe, Opt
 from pythonix.internals.curry import two, three
+from pythonix.internals.res import unpack
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 def new(*vals: T, **kwargs: int) -> deque[T]:
     """Create a new typed ``deque`` object. Use the maxlen kwarg to specify maxlen
@@ -27,307 +28,311 @@
     Example: ::
 
         >>> deq: deque[T] = new(1, 2, 3)
         >>> deq
         deque([1, 2, 3])
 
     """
-    return deque(vals, maxlen=kwargs.get('maxlen'))
+    return deque(vals, maxlen=kwargs.get("maxlen"))
 
 
 @two
 def append(element: U, deq: deque[T]) -> deque[T | U]:
     """Appends an element to the end of a ``deque``
-    
+
     Example: ::
 
         >>> deq: deque[int] = append(4)(deque((1, 2, 3)))
-        >>> val, nil = pop(deq)
+        >>> val, nil = unpack(pop(deq))
         >>> val
         4
-    
+
     """
-    deq.append(element)
-    return deq
+    deq.append(cast(T, element))
+    return cast(deque[T | U], deq)
 
 
 @two
 def appendleft(element: U, deq: deque[T]) -> deque[T | U]:
     """Appends an element to the beginning of a ``deque``
-    
+
     Example: ::
 
         >>> deq: deque[int] = appendleft(4)(new(1, 2, 3))
-        >>> val, nil = popleft(deq)
+        >>> val, nil = unpack(popleft(deq))
         >>> val
         4
 
     """
-    deq.appendleft(element)
-    return deq
+    deq.appendleft(cast(T, element))
+    return cast(deque[T | U], deq)
 
 
-def clear(deq: deque[T]) -> deque[None]:
+def clear(deq: deque[T]) -> deque[T]:
     """Clears the deque of all elements
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
         >>> cleared = clear(deq)
-        >>> val, nil = pop(cleared)
+        >>> val, nil = unpack(pop(cleared))
         >>> nil
         Nil('pop from an empty deque')
-    
+
     """
     deq.clear()
     return deq
 
 
 def copy(deq: deque[T]) -> deque[T]:
     """Returns a shallow copy of the deque
-    
+
     Example: ::
 
         >>> deq1: deque[int] = new(1, 2, 3)
         >>> deq2: deque[int] = copy(deq1)
         >>> deq1 = appendleft(4)(deq1)
         >>> deq2
         deque([1, 2, 3])
-    
+
     """
     return deq.copy()
 
 
 @two
 def count(element: T, deq: deque[T]) -> int:
     """Returns a count of how many elements match the provided one
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 2, 3)
         >>> count(2)(deq)
         2
-    
+
     """
     return deq.count(element)
 
 
 @two
 def extend(iterable: Iterable[U], deq: deque[T]) -> deque[T | U]:
     """Combines an iterable to the right side of the deque
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
         >>> combined = extend([4, 5, 6])(deq)
         >>> deq
         deque([1, 2, 3, 4, 5, 6])
-    
+
     """
-    deq.extend(iterable)
-    return deq
+    deq.extend(cast(Iterable[T], iterable))
+    return cast(deque[T | U], deq)
+
 
 @two
 def extendleft(iterable: Iterable[U], deq: deque[T]) -> deque[T | U]:
     """Combines an iterable to the left side of the deque
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(4, 5, 6)
         >>> combined = extendleft([3, 2, 1])(deq)
         >>> deq
         deque([1, 2, 3, 4, 5, 6])
-    
+
     """
-    deq.extendleft(iterable)
-    return deq
+    deq.extendleft(cast(Iterable[T], iterable))
+    return cast(deque[T | U], deq)
 
 
 @three
 def insert(element: U, index: int, deq: deque[T]) -> deque[T | U]:
     """Insert a new element at the specified index
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
         >>> insert(0)(0)(deq)
         deque([0, 1, 2, 3])
-    
+
     """
-    deq.insert(index, element)
-    return deq
+    deq.insert(index, cast(T, element))
+    return cast(deque[T | U], deq)
 
 
 def index(element: T, **kwargs: int):
     """Retrieves the index of the first occurence of a given element
-    
+
     Use the ``start`` and ``stop`` *kwargs* to specify where to start and stop.
 
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 2, 3, 4)
         >>> index(2)(deq)
         1
         >>> index(2, start=2)(deq)
         2
-    
+
     """
 
     def inner(deq: deque[T]) -> int:
-        if 'start' in kwargs.keys() and 'stop' in kwargs.keys():
-            start = kwargs.get('start')
-            stop = kwargs.get('stop')
-            return deq.index(element, start, stop)
-        if 'start' in kwargs.keys():
-            start = kwargs.get('start')
-            return deq.index(element, start) 
+        if "start" in kwargs.keys() and "stop" in kwargs.keys():
+            start = kwargs.get("start")
+            stop = kwargs.get("stop")
+            if start is not None and stop is not None:
+                return deq.index(element, start, stop)
+        if "start" in kwargs.keys():
+            start = kwargs.get("start")
+            if start is not None:
+                return deq.index(element, start)
         return deq.index(element)
-    
+
     return inner
 
 
 @two
 @null_and_error_safe(IndexError)
-def get(index: int | slice, deq: deque[T]) -> T:
+def get(index: SupportsIndex, deq: deque[T]) -> T:
     """Retrieve the element at a given index
-    
+
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> val, nil = get(0)(deq)
+        >>> val, nil = unpack(get(0)(deq))
         >>> val
         1
-        >>> val, nil = get(4)(deq)
+        >>> val, nil = unpack(get(4)(deq))
         >>> nil
         Nil('deque index out of range')
-    
+
     """
     return deq[index]
 
 
 @null_and_error_safe(IndexError)
 def pop(deq: deque[T]) -> T:
     """Retrieve and remove the last element
-    
+
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> val, nil = pop(deq)
+        >>> val, nil = unpack(pop(deq))
         >>> val
         3
         >>> deq
         deque([1, 2])
-    
+
     """
     return deq.pop()
 
+
 @null_and_error_safe(IndexError)
 def popleft(deq: deque[T]) -> T:
     """Retrieve and remove the first element
-    
+
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> val, nil = popleft(deq)
+        >>> val, nil = unpack(popleft(deq))
         >>> val
         1
         >>> deq
         deque([2, 3])
-    
+
     """
     return deq.popleft()
 
 
 @two
 @safe(IndexError)
 def remove(element: T, deq: deque[T]) -> deque[T]:
     """Remove an element if it's present
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> deq, nil = remove(2)(deq)
+        >>> deq, nil = unpack(remove(2)(deq))
         >>> deq
         deque([1, 3])
-    
+
     """
     deq.remove(element)
     return deq
 
 
 def reverse(deq: deque[T]) -> deque[T]:
     """Reverse the order of elements
-    
+
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
         >>> reverse(deq)
         deque([3, 2, 1])
-    
+
     """
     deq.reverse()
     return deq
 
 
 def rotate(n: int = 1):
     """Brings the last element to be first *n* times
-    
+
     Examples: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
         >>> rotate()(deq)
         deque([3, 1, 2])
         >>> rotate()(deq)
         deque([2, 3, 1])
         >>> rotate()(deq)
         deque([1, 2, 3])
-    
+
     """
-    def inner(deq: deque[T]) -> deque[T]:
 
+    def inner(deq: deque[T]) -> deque[T]:
         deq.rotate(n)
         return deq
-    
+
     return inner
 
 
 def first(deq: deque[T]) -> Opt[T]:
     """Gets the first element
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> val, nil = first(deq)
+        >>> val, nil = unpack(first(deq))
         >>> val
         1
-    
+
     """
     return get(0)(deq)
 
 
 def last(deq: deque[T]) -> Opt[T]:
     """Gets the last element
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3)
-        >>> val, nil = last(deq)
+        >>> val, nil = unpack(last(deq))
         >>> val
         3
-    
+
     """
     return get(-1)(deq)
 
 
 @null_safe
-def maxlen(deq: deque[T]) -> int:
+def maxlen(deq: deque[T]) -> int | None:
     """Gets the maximum length of the deque
-    
+
     Example: ::
 
         >>> deq: deque[int] = new(1, 2, 3, maxlen=3)
-        >>> m, nil = maxlen(deq)
+        >>> m, nil = unpack(maxlen(deq))
         >>> m
         3
 
     """
-    return deq.maxlen
+    return deq.maxlen
```

### Comparing `pythonix-1.0.9/pythonix/internals/dict_utils.py` & `pythonix-1.1.0/pythonix/internals/dict_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,22 @@
     True
     >>> data: dict[str, int] = {'First': 1, 'Second': 2}
     >>> str_values_dict: dict[str, str] = map_values(str)(data)
     >>> tuple(str_values_dict.values())
     ('1', '2')
 
 """
-from typing import TypeVar, Dict, Callable, Mapping, Tuple
+from typing import TypeVar, Dict, Callable, Mapping, Tuple, cast
 from pythonix.internals.op import item
+from pythonix.internals.res import Opt, unpack
 
 V = TypeVar("V")
 W = TypeVar("W")
-K = TypeVar("K", str, int, float, tuple)
-L = TypeVar("L", str, int, float, tuple)
+K = TypeVar("K")
+L = TypeVar("L")
 
 
 def map_items(using: Callable[[K, V], Tuple[L, W]]):
     """Applies *using* with dict items to return a new dict with the results
 
     Example: ::
 
@@ -43,15 +44,15 @@
     return get_dict
 
 
 def map_keys(using: Callable[[K], L]):
     """Applies *using* over dict keys to return a new dict with the results
 
     Example: ::
-        
+
         >>> data: dict[str, int] = {'First': 1, 'Second': 2}
         >>> upper_dict: dict[str, int] = map_keys(str.upper)(data)
         >>> upper_keys: tuple[str, ...] = tuple(upper_dict.keys())
         >>> upper_keys == ('FIRST', 'SECOND')
         True
 
     """
@@ -116,24 +117,27 @@
     return get_dict
 
 
 def merge(new_dict: Dict[L, W]):
     """Merges two dictionaries together, overriding the first with the second
 
     Example: ::
-        
+
         >>> old: dict[str, int] = {'foo': 0}
         >>> new: dict[int, str] = {1: 'bar'}
         >>> merge(new)(old)
         {'foo': 0, 1: 'bar'}
 
     """
 
     def get_old(old_dict: Dict[K, V]) -> Dict[K | L, V | W]:
-        return old_dict | new_dict
+        return {
+            **cast(Dict[K | L, V | W], old_dict),
+            **cast(Dict[K | L, V | W], new_dict),
+        }
 
     return get_old
 
 
 def put(key: L):
     """Puts a new value into a `dict`.
 
@@ -159,17 +163,17 @@
 def get(key: K):
     """Gets value from dict as Ok[T], or Err[Nil] if not found
 
     Example: ::
 
         >>> d = {'foo': 'bar'}
         >>> bar = get('foo')(d)
-        >>> val, err = bar
+        >>> val, err = unpack(bar)
         >>> val
         'bar'
 
     """
 
-    def get_data(mapping: Mapping[K, V]):
+    def get_data(mapping: Mapping[K, V]) -> Opt[V]:
         return item(key)(mapping)
 
     return get_data
```

### Comparing `pythonix-1.0.9/pythonix/internals/fn.py` & `pythonix-1.1.0/pythonix/internals/fn.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.9/pythonix/internals/grammar.py` & `pythonix-1.1.0/pythonix/internals/grammar.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         >>> 10 | add_ten
         20
         >>> add_ten(10)
         20
 
 """
 from __future__ import annotations
-from typing import TypeVar, Callable, Generic, Self
+from typing import TypeVar, Callable, Generic, cast
 from pythonix.internals.curry import two
 
 S = TypeVar("S")
 T = TypeVar("T")
 U = TypeVar("U")
 E = TypeVar("E", bound="Exception")
 
@@ -285,15 +285,15 @@
             >>> actual: str = 10 |P| (lambda x: x + 10) |P| do(print) |P| str
             20
 
         Passing ``print`` to ``P`` would usually have the next value be ``None``.
         However, since we used ``do``, its original value was preserved.
 
     """
-    func(val)
+    func(cast(S, val))
     return val
 
 
 def inner(val: T) -> T:
     """Returns its only argument. Useful for Piper >
 
     Example:
@@ -382,15 +382,15 @@
                 >>> actual: str = Piper(5).bind(lambda x: x + 5).bind(str).inner
                 >>> expected == actual
                 True
 
         """
         return Piper(op(self.inner))
 
-    def do(self, op: Callable[[T], U]) -> Self[T]:
+    def do(self, op: Callable[[T], U]) -> Piper[T]:
         """Run *op* with *inner*, but return original `Piper`. Same as |
 
         Args:
             *op* ((S) -> U): Func that takes inner and returns a new value
 
         Examples:
```

### Comparing `pythonix-1.0.9/pythonix/internals/res.py` & `pythonix-1.1.0/pythonix/internals/res.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,51 +29,59 @@
         ... def get_baz(data: dict[str, str]) -> str:
         ...     return data['baz']
         ...
 
 And much, much more. Everything has its own documentation so check it out.
     
 """
-from __future__ import annotations
 from functools import wraps
+from dataclasses import dataclass
+from abc import ABC
 from typing import (
+    Tuple,
     TypeVar,
     Generic,
-    NamedTuple,
     cast,
     ParamSpec,
     Callable,
     TypeAlias,
-    Iterator,
 )
 
 P = ParamSpec("P")
 
+NotResError = TypeError("Must pass in an Ok or Err")
 UnwrapErr = ValueError("Attempted to retrieve an Err from an Ok")
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 E = TypeVar("E", bound="Exception")
 F = TypeVar("F", bound="Exception")
 G = TypeVar("G", bound="Exception")
 
 
+class BaseRes(Generic[T], ABC):
+    """Base class for use by Ok and Err"""
+
+    inner: T
+
+
 class Nil(Exception):
     """Error class used to represent an unexpected `None` value.
 
     Using ``Ok[T] | Err[Nil]`` replaces using ``T | None`` to represent potential
     null values.
 
     """
 
     def __init__(self, message: str = "Did not expect None"):
         super().__init__(message)
 
 
-class Ok(Generic[T], NamedTuple):
+@dataclass(frozen=True)
+class Ok(BaseRes, Generic[T]):
     """Represents a successful outcome of a function that could have failed.
 
     Useful for pattern matching on a function that returns `Ok[T] | Err[E]`.
     Inner values can be unpacked like a tuple.
 
     Note:
         The preferred constructor is ``ok`` as it will preserve type information
@@ -87,20 +95,19 @@
         ...         raise e
         ...
         5
 
     """
 
     inner: T
-
-    def __iter__(self) -> Iterator[T | None]:
-        return iter((self.inner, None))
+    __match_args__ = ("inner",)
 
 
-class Err(Generic[E], NamedTuple):
+@dataclass(frozen=True)
+class Err(BaseRes, Generic[E]):
     """Represents a successful outcome of a function that could have failed.
 
     Useful for pattern matching on a function that returns `Ok[T] | Err[E]`.
     Contained value must be a subclass of ``Exception``.
 
     Note:
         The preferred constructor is ``err``, as it preserves type information
@@ -112,31 +119,45 @@
         ...         val
         ...     case Err(e):
         ...         str(e)
         'foo'
 
     """
 
+    __match_args__ = ("inner",)
     inner: E
 
-    def __iter__(self) -> Iterator[E | None]:
-        return iter((None, self.inner))
-
 
 Res: TypeAlias = Ok[T] | Err[E]
-"""Type alias for ``Ok[T]`` or ``Err[E]``. Useful for quickly annotating
+"""Convenient type alias for a value that could be Ok or Err"""
 
-Example: ::
 
-    >>> res: Res[int, ValueError] = ok(ValueError)(10)
-    
-"""
+def unpack(res: Res[T, E]) -> Tuple[T | None, E | None]:
+    """Unpack a reuslt in a Go like way to make error handling simple
 
-Opt: TypeAlias = Ok[T] | Err[Nil]
-"""Type alias for ``Ok[T] | Err[Nil]``. Useful for quick annotations and types.
+    Examples: ::
+
+        >>> val, err = unpack(ok(ValueError)(10))
+        >>> val
+        10
+        >>> err is None
+        True
+
+    """
+    match res:
+        case Ok(t):
+            return t, None
+        case Err(e):
+            return None, e
+        case _:
+            raise NotResError
+
+
+Opt: TypeAlias = Res[T, Nil]
+"""Type alias for ``Res[T, Nil]``. Useful for quick annotations and types.
 
 Example: ::
 
     >>> maybe_int: Opt[int] = some(10)
 
 """
 
@@ -154,16 +175,16 @@
         ...         val
         ...     case Err(e):
         ...         str(e)
         'foo'
 
     """
 
-    def get_err(exception_object: E) -> Res[T, E]:
-        return Err(exception_object)
+    def get_err(err_obj: E) -> Res[T, E]:
+        return cast(Res[T, E], Err(err_obj))
 
     return get_err
 
 
 def ok(err_type: type[E]) -> Callable[[T], Res[T, E]]:
     """Creates an ``Ok[T]`` while also providing type information for ``Err[E]``
 
@@ -206,16 +227,16 @@
         ...     case Err(Nil()):
         ...         ...
         ...
         'world'
 
     """
     if inner is not None:
-        return ok(Nil)(inner)
-    return err(T)(Nil())
+        return Ok(inner)
+    return Err(Nil())
 
 
 def is_ok(res: Res[T, E]) -> bool:
     """Return `True` if the `Res` is `Ok`, else ``False``
 
     Another easy way to see if a result is ``Ok`` or ``Err``
 
@@ -233,14 +254,16 @@
 
     """
     match res:
         case Ok():
             return True
         case Err():
             return False
+        case _:
+            raise NotResError
 
 
 def is_err(res: Res[T, E]) -> bool:
     """Return ``True`` if the ``Res`` is ``Err``, else ``True``
 
     Another easy way to see if a result is ``Err`` or ``Ok``
 
@@ -258,14 +281,16 @@
 
     """
     match res:
         case Ok():
             return False
         case Err():
             return True
+        case _:
+            raise NotResError
 
 
 def is_ok_and(predicate: Callable[[T], bool]) -> Callable[[Res[T, E]], bool]:
     """Return `True` if the `Res` is `Ok` and the `predicate` evaluates to `True`
 
     Args:
         *predicate* ((T) -> bool): Func to be evaluated against inner
@@ -282,16 +307,18 @@
 
     """
 
     def inner(res: Res[T, E]) -> bool:
         match res:
             case Ok(t):
                 return predicate(t)
-            case _:
+            case Err():
                 return False
+            case _:
+                raise NotResError
 
     return inner
 
 
 def is_err_and(predicate: Callable[[E], bool]) -> Callable[[Res[T, E]], bool]:
     """Return `True` if the `Res` is `Err` and the *predicate* evaluates to `True`
 
@@ -308,18 +335,20 @@
         >>> is_err_and(lambda e: str(e) == 'foo')(outcome)
         True
 
     """
 
     def inner(res: Res[T, E]) -> bool:
         match res:
+            case Ok():
+                return False
             case Err(e):
                 return predicate(e)
             case _:
-                return False
+                raise NotResError
 
     return inner
 
 
 def unwrap(res: Res[T, E]) -> T:
     """Returns the wrapped value if ``Ok``, or will raise the exception if ``Err``.
 
@@ -351,14 +380,16 @@
             ValueError
     """
     match res:
         case Ok(value):
             return cast(T, value)
         case Err(e):
             raise e
+        case _:
+            raise NotResError
 
 
 def unwrap_or(default: T) -> Callable[[Res[T, E]], T]:
     """Return the `Ok` value if `Ok`, else return the default
 
     Args:
         *default* (T): The value to be returned if ``Err``
@@ -378,16 +409,18 @@
 
     """
 
     def inner(res: Res[T, E]) -> T:
         match res:
             case Ok(val):
                 return val
-            case _:
+            case Err():
                 return default
+            case _:
+                raise NotResError
 
     return inner
 
 
 def unwrap_or_else(on_err: Callable[[], T]) -> Callable[[Res[T, E]], T]:
     """Return the `Ok` value if `Ok`, else run the `on_err` function
     that returns the same type.
@@ -411,16 +444,18 @@
 
     """
 
     def inner(res: Res[T, E]) -> T:
         match res:
             case Ok(val):
                 return val
-            case _:
+            case Err():
                 return on_err()
+            case _:
+                raise NotResError
 
     return inner
 
 
 def unwrap_err(result: Res[T, E]) -> E:
     """Returns the wrapped Exception if ``Err``, or panice if ``Ok``.
 
@@ -453,14 +488,16 @@
 
     """
     match result:
         case Ok():
             raise UnwrapErr
         case Err(e):
             return e
+        case _:
+            raise NotResError
 
 
 def map(using: Callable[[T], U]) -> Callable[[Res[T, E]], Res[U, E]]:
     """Run the function on the `Ok` if `Ok`, else return the current `Err`
 
     Useful for conditionally transforming ``Res`` values, independent of their
     state.
@@ -490,17 +527,19 @@
         ValueError
 
     """
 
     def inner(res: Res[T, E]) -> Res[U, E]:
         match res:
             case Ok(t):
-                return ok(E)(using(t))
+                return Ok(using(t))
+            case Err(e):
+                return Err(e)
             case _:
-                return cast(Res[U, E], err(U)(res.inner))
+                raise NotResError
 
     return inner
 
 
 def map_or(using: Callable[[T], U]) -> Callable[[U], Callable[[Res[T, E]], Res[U, E]]]:
     """Runs the function on the `Ok` or return the `default` if `Err`
 
@@ -524,17 +563,19 @@
 
     def get_default(
         default: U,
     ) -> Callable[[Res[T, E]], Res[U, E]]:
         def inner(res: Res[T, E]) -> Res[U, E]:
             match res:
                 case Ok(t):
-                    return ok(E)(using(t))
+                    return Ok(using(t))
+                case Err():
+                    return Ok(default)
                 case _:
-                    return ok(E)(default)
+                    raise NotResError
 
         return inner
 
     return get_default
 
 
 def map_err(using: Callable[[E], F]) -> Callable[[Res[T, E]], Res[T, F]]:
@@ -555,20 +596,22 @@
         >>> to_type_error = lambda e: TypeError(str(e))
         >>> mapped_err: Res[int, TypeError] = map_err(to_type_error)(err_outcome)
         >>> unwrap_err(mapped_err)
         TypeError('')
 
     """
 
-    def inner(res: Res[T, E]) -> Res[T, E]:
+    def inner(res: Res[T, E]) -> Res[T, F]:
         match res:
             case Err(e):
-                return err(T)(using(e))
+                return Err(using(e))
+            case Ok(t):
+                return Ok(t)
             case _:
-                return cast(Res[T, F], err(T)(res.inner))
+                raise NotResError
 
     return inner
 
 
 def map_or_else(
     using: Callable[[T], U]
 ) -> Callable[[Callable[[], U]], Callable[[Res[T, E]], Res[U, E]]]:
@@ -596,25 +639,27 @@
 
     """
 
     def get_default(default: Callable[[], U]) -> Callable[[Res[T, E]], Res[U, E]]:
         def inner(res: Res[T, E]) -> Res[U, E]:
             match res:
                 case Ok(t):
-                    return ok(E)(using(t))
+                    return Ok(using(t))
+                case Err():
+                    return Ok(default())
                 case _:
-                    return ok(E)(default())
+                    raise NotResError
 
         return inner
 
     return get_default
 
 
 def and_then(using: Callable[[T], Res[U, E]]) -> Callable[[Res[T, E]], Res[U, E]]:
-    """Replaces *res* with new result from *using*s output
+    """Replaces *res* with new result from *using*s output if Ok
 
     This is useful when you need to run functions that also return a result.
 
     Note:
         Preserve type hints by making sure that the `E` values are the same
 
     Args:
@@ -629,29 +674,27 @@
         >>> succeeds = lambda x: some(str(x))
         >>> ok_outcome: Opt[int] = some(10)
         >>> err_outcome: Opt[int] = err(int)(Nil())
         >>> new_ok: Opt[str] = and_then(succeeds)(ok_outcome)
         >>> unwrap(new_ok)
         '10'
         >>> new_err: Opt[str] = and_then(succeeds)(err_outcome)
-        >>> unwrap(new_err)
-        Traceback (most recent call last):
-          File "<stdin>", line 1, in <module>
-            unwrap(new_err)
-            raise e
-        res.Nil: Did not expect None
+        >>> unwrap_err(new_err)
+        Nil('Did not expect None')
 
     """
 
     def inner(res: Res[T, E]) -> Res[U, E]:
         match res:
             case Ok(t):
-                return cast(Res[U, E], using(t))
+                return using(t)
+            case Err(e):
+                return Err(e)
             case _:
-                return cast(Res[U, E], err(U)(res.inner))
+                raise NotResError
 
     return inner
 
 
 def or_else(using: Callable[[E], Res[T, F]]) -> Callable[[Res[T, E]], Res[T, F]]:
     """Runs *using* to replace current state if ``Err``, else returns current state.
 
@@ -664,26 +707,29 @@
 
     Returns:
         *output* (Res[T, F]): ``Res`` with updated ``Err`` value, or same ``Ok``
 
     Examples: ::
 
         >>> err_outcome: Res[int, ValueError] = err(int)(ValueError())
-        >>> on_fail = lambda _: Nil()
+        >>> on_fail = lambda _: Err(Nil())
         >>> new_err: Res[int, Nil] = or_else(on_fail)(err_outcome)
         >>> unwrap_err(new_err)
+        Nil('Did not expect None')
 
     """
 
     def inner(res: Res[T, E]) -> Res[T, F]:
         match res:
             case Err(e):
-                return cast(Res[T, F], using(e))
+                return using(e)
+            case Ok(t):
+                return Ok(t)
             case _:
-                return cast(Res[T, F], err(U)(res.inner))
+                raise NotResError
 
     return inner
 
 
 def and_res(new_res: Res[U, E]) -> Callable[[Res[T, E]], Res[U, E]]:
     """Returns the provided result if the old one is `Ok`
 
@@ -697,28 +743,35 @@
     Examples: ::
 
         >>> old: Opt[int] = some(10)
         >>> new: Opt[str] = some('hello')
         >>> resolved: Opt[str] = and_res(new)(old)
         >>> unwrap(resolved)
         'hello'
+        >>> new: Opt[str] = err(str)(Nil())
+        >>> resolved: Opt[str] = and_res(new)(old)
+        >>> unwrap_err(resolved)
+        Nil('Did not expect None')
 
     """
 
     def inner(old_res: Res[T, E]) -> Res[U, E]:
         match old_res:
             case Ok():
                 match new_res:
                     case Ok(u):
-                        return ok(E)(u)
+                        return Ok(u)
                     case Err(e):
-                        return err(U)(e)
-                return new_res
+                        return Err(e)
+                    case _:
+                        raise NotResError
             case Err(e):
-                return err(U)(e)
+                return Err(e)
+            case _:
+                raise NotResError
 
     return inner
 
 
 def or_res(new_res: Res[T, F]) -> Callable[[Res[T, E]], Res[T, F]]:
     """Returns the provided result if the current one is an `Err`
 
@@ -732,27 +785,35 @@
     Examples: ::
 
         >>> new: Res[int, ValueError] = err(int)(ValueError())
         >>> old: Res[int, TypeError] = err(int)(TypeError())
         >>> resolved: Res[int, ValueError] = or_res(new)(old)
         >>> unwrap_err(resolved)
         ValueError()
+        >>> new: Res[int, ValueError] = ok(ValueError)(10)
+        >>> resolved: Res[int, TypeError] = or_res(new)(old)
+        >>> unwrap(resolved)
+        10
 
     """
 
     def inner(old_res: Res[T, E]) -> Res[T, F]:
         match old_res:
             case Ok(t):
-                return ok(F)(t)
+                return Ok(t)
             case Err():
                 match new_res:
                     case Ok(t):
-                        return ok(F)(t)
+                        return Ok(t)
                     case Err(f):
-                        return err(T)(f)
+                        return Err(f)
+                    case _:
+                        raise NotResError
+            case _:
+                raise NotResError
 
     return inner
 
 
 def flatten(res: Res[Res[T, E], F]) -> Res[T, E | F]:
     """Flattens a `Res` containing a `Res`. Not recursive.
 
@@ -771,19 +832,23 @@
         10
 
     """
     match res:
         case Ok(inner):
             match inner:
                 case Ok(t):
-                    return cast(Res[T, E | F], ok(E | F)(t))
+                    return Ok(t)
                 case Err(f):
-                    return cast(Res[T, E | F], err(T)(f))
+                    return Err(f)
+                case _:
+                    raise NotResError
         case Err(e):
-            return cast(Res[T, E | F], err(T)(e))
+            return Err(e)
+        case _:
+            raise NotResError
 
 
 def safe(*err_type: type[E]):
     """Decorator function to catch raised ``Exception`` and return ``Res[T, E]``
 
     ``T`` is the original return value and ``E`` is the combination of specified
     ``Exceptions``
@@ -815,17 +880,17 @@
 
     """
 
     def inner(using: Callable[P, U]) -> Callable[P, Res[U, E]]:
         @wraps(using)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[U, E]:
             try:
-                return cast(Res[U, E], ok(E)(using(*args, **kwargs)))
+                return Ok(using(*args, **kwargs))
             except err_type as e:
-                return cast(Res[U, E], err(U)(e))
+                return Err(e)
 
         return wrapper
 
     return inner
 
 
 def null_safe(using: Callable[P, U | None]):
@@ -881,15 +946,15 @@
 
     def inner(using: Callable[P, T | None]):
         @wraps(using)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Opt[T]:
             try:
                 return some(using(*args, **kwargs))
             except err_types as e:
-                return map_err(lambda f: Nil(str(f)))(err(T)(e))
+                return Err(Nil(str(e)))
 
         return wrapper
 
     return inner
 
 
 def combine_errors(to: F, inherit_message: bool = False):
```

### Comparing `pythonix-1.0.9/pythonix/pair.py` & `pythonix-1.1.0/pythonix/pair.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Key value pair utility functions to make using pairs easier.
 
-Includes methods for creating pairs, setting and gettings keys and values, and mapping over a value.
+Includes methods for creating pairs, setting and gettings keys and values,
+and mapping over a value.
 
-Example:
-    ```python
-    from pythonix.prelude import *
+Example: ::
+
+    >>> pair = new('foo')(None)
+    >>> pair = set_key('bar')(pair)
+    >>> pair = set_value(5)(pair)
+    >>> pair = map_value(lambda x: x + 5)(pair)
+    >>> get_value(pair)
+    10
+    >>> get_key(pair)
+    'bar'
+    >>> key, val = pair
+    >>> (key, val)
+    ('bar', 10)
 
-    (
-        B(pair.new('foo')(None))
-        (pair.set_key('bar'))
-        (pair.set_value(5))
-        (pair.map(lambda x: x + 5))
-        .do
-        (pair.get_value |P| prove.equals(10) |P| res.unwrap)
-        (pair.get_key |P| prove.equals('bar') |P| res.unwrap)
-        (prove.equals(('bar', 10)) |P| res.unwrap)
-    )
-    ```
 """
 from pythonix.internals.pair import (
     Pair,
     Pairs,
     new,
     get_key,
     get_value,
     set_key,
     set_value,
-    map,
+    map_value,
 )
```

### Comparing `pythonix-1.0.9/pythonix/res.py` & `pythonix-1.1.0/pythonix/res.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     is_err,
     is_err_and,
     is_ok,
     is_ok_and,
     map,
     map_err,
     map_or,
+    unpack,
     map_or_else,
     null_safe,
     ok,
     or_else,
     safe,
     map_err,
     unwrap,
@@ -61,8 +62,9 @@
     unwrap_or,
     unwrap_or_else,
     Ok,
     Err,
     null_and_error_safe,
     q,
     qe,
+    combine_errors,
 )
```

