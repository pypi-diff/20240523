# Comparing `tmp/modifiable-items-dictionary-2.0.3.tar.gz` & `tmp/modifiable_items_dictionary-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modifiable-items-dictionary-2.0.3.tar", last modified: Mon Oct 16 14:55:50 2023, max compression
+gzip compressed data, was "modifiable_items_dictionary-3.0.0.tar", last modified: Thu May 23 19:09:28 2024, max compression
```

## Comparing `modifiable-items-dictionary-2.0.3.tar` & `modifiable_items_dictionary-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary/modifiable_items_dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-10-16 14:55:50.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-10-16 14:55:50.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 14:55:50.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-16 14:55:50.000000 modifiable-items-dictionary-2.0.3/modifiable_items_dictionary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:55:50.195350 modifiable-items-dictionary-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2023-10-16 14:55:38.000000 modifiable-items-dictionary-2.0.3/tests/test_modifiable_items_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.947297 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_attribute_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18550 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_dict.py
```

### Comparing `modifiable-items-dictionary-2.0.3/LICENSE` & `modifiable_items_dictionary-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modifiable-items-dictionary-2.0.3/modifiable_items_dictionary/modifiable_items_dictionary.py` & `modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,27 @@
 )
 
 # Sentinel
 NO_DEFAULT = object()
 
 # Typing
 # For python 3.6 compatibility
-Self = TypeVar("Self", bound="ModifiableItemsDict")
+Self = TypeVar('Self', bound='ModifiableItemsDict')
 
 Key = Hashable
 Value = Any
 MappingCallable = Union[
-    map, multiprocessing.pool.ThreadPool.map,
+    map,
+    multiprocessing.pool.ThreadPool.map,
     multiprocessing.pool.ThreadPool.imap,
-    multiprocessing.pool.ThreadPool.imap_unordered
+    multiprocessing.pool.ThreadPool.imap_unordered,
 ]
 KeyCallable = Callable[[Any], Key]
 ValueCallable = Callable[[Any], Value]
-KeyModifiers = Optional[
-    Union[Self, KeyCallable, Iterable[KeyCallable], None]
-]
+KeyModifiers = Optional[Union[Self, KeyCallable, Iterable[KeyCallable], None]]
 ValueModifiers = Optional[
     Union[Self, ValueCallable, Iterable[ValueCallable], None]
 ]
 
 
 class ModifiableItemsDict(dict):
     """Dictionary class that can modify __key and v at runtime.
@@ -79,22 +78,22 @@
     # TODO: Add validators
     _key_modifiers: KeyModifiers = None
     _value_modifiers: ValueModifiers = None
     _map_function: MappingCallable = map
 
     @staticmethod
     def _modify_item(
-            item: Any,
-            modifiers: Union[
-                Iterable[Callable[[Any], Hashable]],
-                Iterable[Callable[[Any], Any]],
-                Callable[[Any], Hashable],
-                Callable[[Any], Any],
-                None,
-            ],
+        item: Any,
+        modifiers: Union[
+            Iterable[Callable[[Any], Hashable]],
+            Iterable[Callable[[Any], Any]],
+            Callable[[Any], Hashable],
+            Callable[[Any], Any],
+            None,
+        ],
     ) -> Any:
         """Modifies an *__item* with the *modifiers*
 
         Args:
             item: The __item that will be modified by the *modifiers*.
             modifiers: Modifiers that will modify the *__item*.
 
@@ -104,33 +103,33 @@
         """
         if not modifiers:
             return item
 
         # Defensive Programming
         if isinstance(modifiers, str):
             _error: TypeError = TypeError(
-                "Invalid Modifiers:",
+                'Invalid Modifiers:',
                 modifiers,
-                "Can not be of types",
+                'Can not be of types',
                 (str,),
             )
             raise _error
 
         if isinstance(modifiers, Iterable):
             for modifier in modifiers:
                 item = modifier(item)
             return item
         if callable(modifiers):
             item = modifiers(item)
             return item
 
         _error = TypeError(
-            "Invalid Modifiers:",
+            'Invalid Modifiers:',
             modifiers,
-            "must be of types:",
+            'must be of types:',
             (Iterable, Callable),
         )
         raise _error
 
     def _modify_key(self, key: Key) -> Key:
         """Modify the *__key* with the __key modifiers.
 
@@ -154,32 +153,32 @@
         """
         _modified_value: Value = self._modify_item(
             value, self._value_modifiers
         )
         return _modified_value
 
     def _modify_key_and_item(
-            self, key_and_value: Tuple[Key, Value]
+        self, key_and_value: Tuple[Key, Value]
     ) -> Tuple[Key, Value]:
         _key, _value = key_and_value
         if self._key_modifiers:
             _key = self._modify_key(_key)
         if self._value_modifiers:
             _value = self._modify_value(_value)
         return _key, _value
 
     @overload
     def _create_modified_mapping(
-            self, items_view: ItemsView[Key, Value]
+        self, items_view: ItemsView[Key, Value]
     ) -> Mapping[Key, Value]:
         ...
 
     @overload
     def _create_modified_mapping(
-            self, iterable: Iterable[Tuple[Key, Value]]
+        self, iterable: Iterable[Tuple[Key, Value]]
     ) -> Mapping[Key, Value]:
         ...
 
     def _create_modified_mapping(self, iterable):
         """Create the modified mapping from the *Iterable*.
 
         Args:
@@ -196,15 +195,15 @@
                 self._modify_key_and_item, iterable
             )
         }
 
         return new_mapping
 
     def _iterable_to_modified_dict(
-            self, iterable: Iterable
+        self, iterable: Iterable
     ) -> Mapping[Key, Value]:
         """Convert an *iterable* to a *Mapping* that has had it's keys and
         values modified.
 
         Args:
             iterable: *Iterable* that will be converted to a *Mapping* which
             has had it's items modified.
@@ -217,40 +216,38 @@
         elif isinstance(iterable, Iterable):
             iterable = self._create_modified_mapping(iterable)
 
         return iterable
 
     @classmethod
     def fromkeys(
-            cls,
-            __iterable: Iterable[Key],
-            __value: Optional[Union[Value, None]] = None,
+        cls,
+        __iterable: Iterable[Key],
+        __value: Optional[Union[Value, None]] = None,
     ) -> Self:
         return cls(dict.fromkeys(__iterable, __value))
 
     @overload
     def __init__(self, **kwargs: Value) -> None:
         ...
 
     @overload
-    def __init__(
-            self, mapping: Mapping[Key, Value], **kwargs: Value
-    ) -> None:
+    def __init__(self, mapping: Mapping[Key, Value], **kwargs: Value) -> None:
         ...
 
     @overload
     def __init__(
-            self, iterable: Iterable[Tuple[str, Any]], **kwargs: Value
+        self, iterable: Iterable[Tuple[str, Any]], **kwargs: Value
     ) -> None:
         ...
 
     def __init__(
-            self,
-            iterable=None,
-            **kwargs,
+        self,
+        iterable=None,
+        **kwargs,
     ):
         # If there is a ValueError have the inherited class deal with it.
         with contextlib.suppress(ValueError):
             if iterable:
                 iterable = self._iterable_to_modified_dict(iterable)
             if kwargs:
                 kwargs = self._iterable_to_modified_dict(kwargs)
@@ -312,27 +309,25 @@
         return value
 
     @overload
     def update(self, __m: Mapping[Key, Value], **kwargs: Value) -> None:
         ...
 
     @overload
-    def update(
-            self, __m: Iterable[Tuple[str, Any]], **kwargs: Value
-    ) -> None:
+    def update(self, __m: Iterable[Tuple[str, Any]], **kwargs: Value) -> None:
         ...
 
     @overload
     def update(self, **kwargs: Value) -> None:
         ...
 
     def update(
-            self,
-            __m=None,
-            **kwargs,
+        self,
+        __m=None,
+        **kwargs,
     ):
         # If there is a ValueError have the inherited class deal with it.
         with contextlib.suppress(ValueError):
             if __m:
                 __m = self._iterable_to_modified_dict(__m)
             if kwargs:
                 kwargs = self._iterable_to_modified_dict(kwargs)
```

### Comparing `modifiable-items-dictionary-2.0.3/tests/test_modifiable_items_dict.py` & `modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,55 +37,58 @@
             return _ip_address
 
     return _value
 
 
 @pytest.fixture(
     params=(
-            {
-                "CamelCase": 1,
-                "lower": 2,
-                "UPPER": 3,
-                "snake_case": 4,
-                5: "Five",
-                True: "True",
-            },
-            {1: 2, ("hello", "Goodbye"): 2},
+        {
+            'CamelCase': 1,
+            'lower': 2,
+            'UPPER': 3,
+            'snake_case': 4,
+            5: 'Five',
+            True: 'True',
+        },
+        {1: 2, ('hello', 'Goodbye'): 2},
     )
 )
 def valid_mapping(request) -> typing.Mapping:
     inputs: typing.Mapping = request.param
     return inputs
 
 
 class HostDict(modifiable_items_dictionary.ModifiableItemsDict):
     _key_modifiers = [_strip, _case_fold]
     _value_modifiers = staticmethod(_to_ipaddress)
 
 
 class _TestingClass(typing.NamedTuple):
     cls: typing.Type[modifiable_items_dictionary.ModifiableItemsDict]
-    modify_key: (modifiable_items_dictionary.modifiable_items_dictionary
-                 .KeyCallable)
-    modify_value: (modifiable_items_dictionary.modifiable_items_dictionary
-                   .ValueCallable)
+    modify_key: (
+        modifiable_items_dictionary.modifiable_items_dictionary.KeyCallable
+    )
+    modify_value: (
+        modifiable_items_dictionary.modifiable_items_dictionary.ValueCallable
+    )
 
 
 def host_dict_with_list_and_static_method_modifiers() -> typing.Type[
     modifiable_items_dictionary.ModifiableItemsDict
 ]:
     class HostDict(modifiable_items_dictionary.ModifiableItemsDict):
         _key_modifiers = [_strip, _case_fold]
         _value_modifiers = staticmethod(_to_ipaddress)
 
     return HostDict
 
 
 def host_dict_with_list_and_method_modifiers() -> typing.Type[
-    modifiable_items_dictionary.ModifiableItemsDict]:
+    modifiable_items_dictionary.ModifiableItemsDict
+]:
     class HostDict(modifiable_items_dictionary.ModifiableItemsDict):
         _key_modifiers = [_strip, _case_fold]
 
         def _value_modifiers(self, _value: typing.Any) -> typing.Any:
             if isinstance(_value, str):
                 with contextlib.suppress(ValueError):
                     _ip_address: typing.Union[
@@ -96,55 +99,55 @@
             return _value
 
     return HostDict
 
 
 @pytest.fixture(
     params=(
-            _TestingClass(
-                host_dict_with_list_and_static_method_modifiers(),
-                _strip_and_case_fold,
-                _to_ipaddress,
-            ),
-            _TestingClass(
-                host_dict_with_list_and_method_modifiers(),
-                _strip_and_case_fold,
-                _to_ipaddress,
-            ),
-            _TestingClass(
-                modifiable_items_dictionary.ModifiableItemsDict,
-                lambda x: x,
-                lambda x: x
-                )
+        _TestingClass(
+            host_dict_with_list_and_static_method_modifiers(),
+            _strip_and_case_fold,
+            _to_ipaddress,
+        ),
+        _TestingClass(
+            host_dict_with_list_and_method_modifiers(),
+            _strip_and_case_fold,
+            _to_ipaddress,
+        ),
+        _TestingClass(
+            modifiable_items_dictionary.ModifiableItemsDict,
+            lambda x: x,
+            lambda x: x,
+        ),
     )
 )
 def class_under_test(request) -> _TestingClass:
     _modifiable_class: _TestingClass = request.param
     return _modifiable_class
 
 
 @pytest.fixture(
     params=[
-        {" GooGle.com ": "142.250.69.206", "CisCO": "72.163.4.185"},
-        [(" GooGle.com ", "142.250.69.206"), ("CisCO", "72.163.4.185")],
+        {' GooGle.com ': '142.250.69.206', 'CisCO': '72.163.4.185'},
+        [(' GooGle.com ', '142.250.69.206'), ('CisCO', '72.163.4.185')],
     ]
 )
 def hosts(request) -> typing.Mapping:
     _hosts: typing.Mapping = request.param
     return _hosts
 
 
 @pytest.fixture(params=(set(), list(), dict()))
 def unhashable_type(request):
     unhashable_type = request.param
     return unhashable_type
 
 
 class TestModifiableItemsDict:
-    @pytest.mark.parametrize("bad_modifiers", [1, 7.62, "string"])
+    @pytest.mark.parametrize('bad_modifiers', [1, 7.62, 'string'])
     def test_bad_modifiers(self, bad_modifiers):
         class BadModifierTest(modifiable_items_dictionary.ModifiableItemsDict):
             _key_modifiers = bad_modifiers
 
         with pytest.raises(TypeError):
             BadModifierTest(a=1)
 
@@ -154,161 +157,147 @@
             _value_modifiers = None
 
         expected = valid_mapping
         actual = NoModifiersDict(valid_mapping)
         assert actual == expected
 
     def test__init__mapping(
-            self,
-            valid_mapping: typing.Mapping,
-            class_under_test
+        self, valid_mapping: typing.Mapping, class_under_test
     ):
         _class, _key_operation, _value_operation = class_under_test
 
         modifiable_dict = _class(valid_mapping)
         expected = {
             _key_operation(key): _value_operation(value)
             for key, value in valid_mapping.items()
         }
         assert modifiable_dict == expected
 
     @pytest.mark.parametrize(
-        "valid_kwargs",
-        ({"a": 1, "B": 2}, {"lower": 3, "UPPER": 4, "MiXeD": 5}),
+        'valid_kwargs',
+        ({'a': 1, 'B': 2}, {'lower': 3, 'UPPER': 4, 'MiXeD': 5}),
     )
     def test__init__kwargs(
-            self,
-            valid_kwargs: typing.Mapping,
-            class_under_test
+        self, valid_kwargs: typing.Mapping, class_under_test
     ):
         _class, _key_operation, _value_operation = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            **valid_kwargs
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(**valid_kwargs)
         expected = {
             _key_operation(key): _value_operation(value)
             for key, value in valid_kwargs.items()
         }
         assert modifiable_items_dict == expected
 
     @pytest.mark.parametrize(
-        "mapping_and_kwargs",
+        'mapping_and_kwargs',
         [
-            ({"a": 1, "B": 2}, {"lower": 3, "UPPER": 4, "MiXeD": 5}),
+            ({'a': 1, 'B': 2}, {'lower': 3, 'UPPER': 4, 'MiXeD': 5}),
         ],
     )
     def test__init__iterable_and_kwargs(
-            self,
-            mapping_and_kwargs: typing.Tuple[typing.Mapping, typing.Mapping],
-            class_under_test
+        self,
+        mapping_and_kwargs: typing.Tuple[typing.Mapping, typing.Mapping],
+        class_under_test,
     ):
         _class, _key_operation, _value_operation = class_under_test
         args, kwargs = mapping_and_kwargs
         expected = {
             _key_operation(key): _value_operation(value)
             for key, value in dict(**args, **kwargs).items()
         }
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            args,
-            **kwargs
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(args, **kwargs)
         assert modifiable_items_dict == expected
 
     @pytest.mark.parametrize(
-        "iterables",
+        'iterables',
         [
-            zip(["one", "TwO", "ThrEE"], [1, 2, 3]),
-            [("TwO", 2), ("one", 1), ("ThrEE", 3), (4, "FouR")],
+            zip(['one', 'TwO', 'ThrEE'], [1, 2, 3]),
+            [('TwO', 2), ('one', 1), ('ThrEE', 3), (4, 'FouR')],
         ],
     )
     def test__init__iterable(
-            self,
-            iterables: typing.Iterable[
-                typing.Tuple[typing.Hashable, typing.Any]],
-            class_under_test
+        self,
+        iterables: typing.Iterable[typing.Tuple[typing.Hashable, typing.Any]],
+        class_under_test,
     ):
         _class, _key_operation, _value_operation = class_under_test
         iterables_copy = copy.deepcopy(iterables)
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            iterables
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(iterables)
         expected: typing.Mapping = {
             _key_operation(key): _value_operation(value)
             for key, value in iterables_copy
         }
         assert modifiable_items_dict == expected
         assert repr(modifiable_items_dict) == repr(expected)
 
-    @pytest.mark.parametrize("invalid_type", ([1], {2}, True, 1))
+    @pytest.mark.parametrize('invalid_type', ([1], {2}, True, 1))
     def test__init__invalid_type(self, invalid_type, class_under_test):
         _class, _, _ = class_under_test
 
         with pytest.raises(TypeError):
             _class(invalid_type)
 
-    @pytest.mark.parametrize("iterable", [[("1", 1), ("two", 2, 2)]])
+    @pytest.mark.parametrize('iterable', [[('1', 1), ('two', 2, 2)]])
     def test__init__bad_iterable_elements(self, iterable, class_under_test):
         _class, _, _ = class_under_test
 
         with pytest.raises(ValueError):
             _class(iterable)
 
     @pytest.mark.parametrize(
-        "keys",
-        (["lower", "Title", "UPPER", "CamelCase", "snake_case", object()],),
+        'keys',
+        (['lower', 'Title', 'UPPER', 'CamelCase', 'snake_case', object()],),
     )
     def test_fromkeys(self, keys: typing.Iterable, class_under_test):
         _class, _key_operation, _value_operation = class_under_test
 
-        value = "Some Value"
+        value = 'Some Value'
         expected: typing.Mapping = {
             _key_operation(key): _value_operation(value) for key in keys
         }
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class.fromkeys(
-            keys,
-            value
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class.fromkeys(keys, value)
         assert modifiable_items_dict == expected
         assert isinstance(modifiable_items_dict, _class)
 
         for key in keys:
             assert key in modifiable_items_dict
 
     @pytest.mark.parametrize(
-        "keys",
-        (["lower", "Title", "UPPER", "CamelCase", "snake_case", object()],),
+        'keys',
+        (['lower', 'Title', 'UPPER', 'CamelCase', 'snake_case', object()],),
     )
     def test_fromkeys_none_value(
-            self,
-            keys: typing.Iterable,
-            class_under_test
+        self, keys: typing.Iterable, class_under_test
     ):
         _class, _key_operation, _value_operation = class_under_test
 
         expected: typing.Mapping = {
             _key_operation(key): _value_operation(None) for key in keys
         }
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class.fromkeys(
-            keys
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class.fromkeys(keys)
         assert modifiable_items_dict == expected
         assert isinstance(modifiable_items_dict, _class)
 
         for key in keys:
             assert key in modifiable_items_dict
 
-    @pytest.mark.parametrize("invalid_type", (True, 1))
+    @pytest.mark.parametrize('invalid_type', (True, 1))
     def test_fromkeys_with_invalid_type(self, invalid_type, class_under_test):
         _class, _, _ = class_under_test
 
         with pytest.raises(TypeError):
             _class.fromkeys(invalid_type)
 
     def test__setitem__(self, valid_mapping, class_under_test):
@@ -322,183 +311,181 @@
         assert modifiable_dict == expected
         assert repr(modifiable_dict) == repr(expected)
 
     def test___setitem__bad_key_type(self, unhashable_type, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
         with pytest.raises(TypeError):
             modifiable_items_dict[unhashable_type] = 0
 
     def test__getitem__(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         for key, value in valid_mapping.items():
             assert modifiable_items_dict[key] == value
 
     def test__getitem__missing_key(self, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
         assert modifiable_items_dict == dict()
 
         # make unique __key which will not be in dict
         _missing_key = object()
 
         with pytest.raises(KeyError):
             _ = modifiable_items_dict[_missing_key]
 
     def test__delitem__(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         for key, value in valid_mapping.items():
             del modifiable_items_dict[key]
             assert key not in modifiable_items_dict
 
     def test__delitem__missing_key(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         with contextlib.suppress(KeyError):
-            del modifiable_items_dict["missing_key"]
+            del modifiable_items_dict['missing_key']
 
     def test_get(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         for key, value in valid_mapping.items():
             assert modifiable_items_dict.get(key) == value
             assert modifiable_items_dict.get(key, None) == value
 
     def test_get_missing_key(self, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         # make unique __key which will not be in dict
         _missing_key = object()
-        _default = "__default v"
+        _default = '__default v'
 
         assert modifiable_items_dict.get(_missing_key) is None
-        assert (
-                modifiable_items_dict.get(_missing_key, _default)
-                == _default
-        )
+        assert modifiable_items_dict.get(_missing_key, _default) == _default
 
     def test_get_unhashable_key(self, unhashable_type, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
-        _default = "__default v"
+        _default = '__default v'
 
         with pytest.raises(TypeError):
             modifiable_items_dict.get(unhashable_type)
             modifiable_items_dict.get(unhashable_type, _default)
 
     def test_pop(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         for key, value in valid_mapping.items():
             assert modifiable_items_dict.pop(key) == value
             assert key not in modifiable_items_dict
 
     def test_pop_default(self, valid_mapping, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            valid_mapping
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(valid_mapping)
         _missing_key = object()
-        _default = "default value"
+        _default = 'default value'
 
         assert modifiable_items_dict.pop(_missing_key, _default) == _default
 
     def test_pop_missing_key(self, class_under_test):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         # make unique __key which will not be in dict
         _missing_key = object()
 
         with pytest.raises(KeyError):
             modifiable_items_dict.pop(_missing_key)
 
     def test_pop_unhashable_type(self, class_under_test, unhashable_type):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         with pytest.raises(KeyError):
             modifiable_items_dict.pop(unhashable_type)
 
     def test_setdefault(self, valid_mapping, class_under_test):
         _class, _key_operation, _value_operation = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
         expected: dict = dict()
         for key, item in valid_mapping.items():
             expected.setdefault(_key_operation(key), _value_operation(item))
             modifiable_items_dict.setdefault(key, item)
         assert modifiable_items_dict == expected
         assert repr(modifiable_items_dict) == repr(expected)
 
     def test_setdefault_unhashable_type(
-            self, class_under_test, unhashable_type
+        self, class_under_test, unhashable_type
     ):
         _class, _, _ = class_under_test
 
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         with pytest.raises(TypeError):
             modifiable_items_dict.setdefault(unhashable_type)
 
     @pytest.mark.parametrize(
-        "starting_data", ({"start_lower": 1, "START_UPPER": 2, "__key": 1},)
+        'starting_data', ({'start_lower': 1, 'START_UPPER': 2, '__key': 1},)
     )
     @pytest.mark.parametrize(
-        "args", ({"UPPER": 1, "lower": 2, "CamelCase": 3, "Key": 2},)
+        'args', ({'UPPER': 1, 'lower': 2, 'CamelCase': 3, 'Key': 2},)
     )
-    @pytest.mark.parametrize("kwargs", ({"UP": 1, "down": 2, "__key": 3},))
+    @pytest.mark.parametrize('kwargs', ({'UP': 1, 'down': 2, '__key': 3},))
     def test_update_using_mapping(
-            self, class_under_test, starting_data, args, kwargs
+        self, class_under_test, starting_data, args, kwargs
     ):
         _class, _key_operation, _value_operation = class_under_test
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            starting_data
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(starting_data)
 
         expected = dict(
             {
                 _key_operation(key): _value_operation(value)
                 for key, value in starting_data.items()
             }
         )
@@ -517,29 +504,28 @@
         )
 
         modifiable_items_dict.update(args, **kwargs)
 
         assert modifiable_items_dict == expected
 
     @pytest.mark.parametrize(
-        "starting_data", ({"start_lower": 1, "START_UPPER": 2, "__key": 1},)
+        'starting_data', ({'start_lower': 1, 'START_UPPER': 2, '__key': 1},)
     )
     @pytest.mark.parametrize(
-        "args",
-        ([("UPPER", 1), ("lower", 2), ("CamelCase", 3), ("__key", 2)],),
+        'args',
+        ([('UPPER', 1), ('lower', 2), ('CamelCase', 3), ('__key', 2)],),
     )
-    @pytest.mark.parametrize("kwargs", ({"UP": 1, "down": 2, "__key": 3},))
+    @pytest.mark.parametrize('kwargs', ({'UP': 1, 'down': 2, '__key': 3},))
     def test_update_using_sequence(
-            self, class_under_test, starting_data, args, kwargs
+        self, class_under_test, starting_data, args, kwargs
     ):
         _class, _key_operation, _value_operation = class_under_test
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class(
-            starting_data
-            )
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class(starting_data)
 
         expected = dict(
             {
                 _key_operation(key): _value_operation(value)
                 for key, value in starting_data.items()
             }
         )
@@ -560,22 +546,24 @@
         modifiable_items_dict.update(args, **kwargs)
 
         assert modifiable_items_dict == expected
 
     def test_update_unhashable_key(self, class_under_test, unhashable_type):
         _class, _, _ = class_under_test
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         iterable = [(unhashable_type, 1)]
 
         with pytest.raises(TypeError):
             modifiable_items_dict.update(iterable)
 
-    @pytest.mark.parametrize("iterable", [[("1", 1), ("two", 2, 2)]])
+    @pytest.mark.parametrize('iterable', [[('1', 1), ('two', 2, 2)]])
     def test_update_bad_iterable_value(self, class_under_test, iterable):
         _class, _, _ = class_under_test
         modifiable_items_dict: (
-            modifiable_items_dictionary.ModifiableItemsDict) = _class()
+            modifiable_items_dictionary.ModifiableItemsDict
+        ) = _class()
 
         with pytest.raises(ValueError):
             modifiable_items_dict.update(iterable)
```

