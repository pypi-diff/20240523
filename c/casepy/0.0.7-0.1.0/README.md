# Comparing `tmp/casepy-0.0.7.tar.gz` & `tmp/casepy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.7.tar", last modified: Mon May 20 03:02:00 2024, max compression
+gzip compressed data, was "casepy-0.1.0.tar", last modified: Thu May 23 04:37:21 2024, max compression
```

## Comparing `casepy-0.0.7.tar` & `casepy-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 03:01:53.000000 casepy-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-20 03:02:00.324767 casepy-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-20 03:01:53.000000 casepy-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:02:00.324767 casepy-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-20 03:01:53.000000 casepy-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.320767 casepy-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/src/casepy/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/combination_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/permutation_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/simple_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:37:21.312900 casepy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 04:37:14.000000 casepy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-23 04:37:21.312900 casepy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 04:37:14.000000 casepy-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 04:37:14.000000 casepy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 04:37:21.312900 casepy-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 04:37:14.000000 casepy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:37:21.308900 casepy-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:37:21.312900 casepy-0.1.0/src/casepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/combination_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/instant_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/permutation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/simple_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-23 04:37:14.000000 casepy-0.1.0/src/casepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:37:21.312900 casepy-0.1.0/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-23 04:37:21.000000 casepy-0.1.0/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 04:37:21.000000 casepy-0.1.0/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 04:37:21.000000 casepy-0.1.0/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 04:37:21.000000 casepy-0.1.0/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.7/LICENSE` & `casepy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.7/src/casepy/permutation_generator.py` & `casepy-0.1.0/src/casepy/combination_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,179 +1,146 @@
-from .simple_methods import *
-from .utils import *
+from .simple_methods import combination_total
 import random
 
 
-class PermutationGenerator:
+class CombinationGenerator:
 
     def __init__(self):
         self.element_list_initialized = False
         self.number_of_selection_initialized = False
         self.must_have_elements = False
 
     def set_parameters(self, in_number_of_selection: int, element_list: list):
         self.in_number_of_selection = in_number_of_selection
         self.element_list = element_list
 
         self.element_list_initialized = True
         self.number_of_selection_initialized = True
-        self.max_possible = self.__duplicated_case_recursive(
-            in_list_to_bin(self.element_list)[0], self.in_number_of_selection
-        )
-
-    # def set_must_have_elements(self, in_elements_list: list):
-    #     if len(in_elements_list) == len(self.element_list):
-    #         # TODO: [A, "", E, D, ""] -> replace elements in ""
-    #         pass
-    #     else:
-    #         self.must_have_elements = True
-    #         self.must_have_list = in_elements_list
-    #         for element in in_elements_list:
-    #             self.element_list.remove(element)
-
-    #         self.in_number_of_selection -= len(in_elements_list)
-    #         self.max_possible = permutation(
-    #             len(self.element_list), self.in_number_of_selection
-    #         ) * (self.in_number_of_selection + 1)
-
-    def __duplicated_case_recursive(self, in_list: list, in_number_of_select: int):
-        if sum(in_list) == 1:
-            return 1
-
-        result_sum = 0
-        if in_number_of_select == 1:
-            for i in in_list:
-                if i != 0:
-                    result_sum += 1
-            return result_sum
-        for i in range(len(in_list)):
-            if in_list[i] != 0:
-                result_sum += self.__duplicated_case_recursive(
-                    in_list[:i] + [in_list[i] - 1] + in_list[i + 1 :],
-                    in_number_of_select - 1,
-                )
-        return result_sum
+        self.max_possible = combination_total(len(element_list), in_number_of_selection)
 
-    def possible_cases(self):
-        return self.max_possible
+    def set_must_have_elements(self, in_elements_list: list):
+        self.must_have_elements = True
+        self.must_have_list = in_elements_list
+        for element in in_elements_list:
+            self.element_list.remove(element)
+
+        self.in_number_of_selection -= len(in_elements_list)
+        self.max_possible = combination_total(
+            len(self.element_list), self.in_number_of_selection
+        )
 
     def all_case(self) -> list:
         if not self.element_list_initialized:
             raise Exception("element_list is not initialized")
         if not self.number_of_selection_initialized:
             raise Exception("number_of_selection is not initialized")
 
         result_list = []
         for i in range(self.max_possible):
             result_list.append(
-                self.permutation_core(i, self.in_number_of_selection, self.element_list)
+                self.combination_core(i, self.in_number_of_selection, self.element_list)
             )
         return result_list
 
     def random_case(self, return_i=False) -> list:
         if not self.element_list_initialized:
             raise Exception("element_list is not initialized")
         if not self.number_of_selection_initialized:
             raise Exception("number_of_selection is not initialized")
 
         random_i = (int)(random.random() * self.max_possible)
 
         if return_i:
-            return random_i, self.permutation_core(
+            return random_i, self.combination_core(
                 random_i,
                 self.in_number_of_selection,
                 self.element_list,
             )
-        return self.permutation_core(
+        return self.combination_core(
             random_i,
             self.in_number_of_selection,
             self.element_list,
         )
 
     def i_case(self, in_iterator: int) -> list:
         if not self.element_list_initialized:
             raise Exception("element_list is not initialized")
         if not self.number_of_selection_initialized:
             raise Exception("number_of_selection is not initialized")
 
-        return self.__permutation_core(in_iterator)
+        return self.combination_core(
+            in_iterator, self.in_number_of_selection, self.element_list
+        )
+
+    # def combination_case(self, in_iterator: int, in_number_of_selection: int) -> list:
+    #     if self.element_list_initialized:
+    #         raise Exception("element_list is not initialized")
+    #     return self.combination_case(
+    #         in_iterator, in_number_of_selection, self.element_list
+    #     )
+
+    def case_to_i(self, in_case: list) -> int:
+
+        include_elements_iterator_list = []
+        for element in in_case:
+            include_elements_iterator_list.append(self.element_list.index(element))
+        include_elements_iterator_list.sort()
+
+        start_index = 0
+        result = 0
+        for i in include_elements_iterator_list:
+            if i == start_index:
+                start_index += 1
+            else:
+                result += combination_total(
+                    i, self.in_number_of_selection - start_index
+                )
+                start_index += 1
+            print(result, start_index)
+        print("include_elements_iterator_list", include_elements_iterator_list)
+
+        return result
 
-    def permutation_core_old(
+    def combination_core(
         self, in_iterator: int, in_number_of_selection: int, element_list: list
     ) -> list:
         result_list = []
-        buff_element_list = element_list.copy()
-        number_of_element = len(buff_element_list)
+        number_of_elements = len(element_list)
+        max_possible = combination_total(number_of_elements, in_number_of_selection)
 
-        iterator = in_iterator
+        if in_iterator >= max_possible:
+            return []
 
-        if self.must_have_elements:
-            iterator = in_iterator // (self.in_number_of_selection + 1)
+        target_iterator = 0
+        while True:
+            if in_number_of_selection == 0:
+                break
 
-        for i in range(in_number_of_selection):
-            current_permutation = permutation(
-                number_of_element - i - 1, in_number_of_selection - i - 1
-            )
-            current_permutation_index = iterator // current_permutation
-            iterator = iterator % current_permutation
-            result_list.append(buff_element_list[current_permutation_index])
-            buff_element_list.pop(current_permutation_index)
+            test = combination_total(number_of_elements - 1, in_number_of_selection - 1)
 
-        if self.must_have_elements:
-            insert_index = in_iterator % (self.in_number_of_selection + 1)
-            for i, element in enumerate(self.must_have_list):
-                result_list.insert(insert_index + i, element)
+            if in_iterator >= test:
+                in_iterator -= test
 
-        return result_list
+                number_of_elements -= 1
 
-    def __permutation_recursive(
-        self, in_iterator: int, in_list: list, in_number_of_select: int
-    ):
-        result_list = []
-        if in_number_of_select == 1:
-            filtered_list = []
-            # print("in 0 -> ", in_list, in_iterator)
-            for i, data in enumerate(in_list):
-                if data != 0:
-                    filtered_list.append(i)
-            result_list.append(filtered_list[in_iterator])
-            # print("in 1 -> ", filtered_list, result_list)
-            return result_list
-        if in_number_of_select == 0:
-            return result_list
-        # results = list(filter(lambda x: x.startswith('f'), animals))
-
-        for i in range(len(in_list)):
-            if in_list[i] != 0:
-                test_list = in_list[:i] + [in_list[i] - 1] + in_list[i + 1 :]
-                test_list_possible_cases = self.__duplicated_case_recursive(
-                    test_list, in_number_of_select - 1
-                )
-                if test_list_possible_cases > in_iterator:
-                    result_list.append(i)
-                    result_list += self.__permutation_recursive(
-                        in_iterator,
-                        test_list,
-                        in_number_of_select - 1,
-                    )
-
-                    break
-                else:
-                    in_iterator -= test_list_possible_cases
+                target_iterator += 1
 
-        return result_list
+            else:
+                result_list.append(element_list[target_iterator])
 
-    def __permutation_core(self, in_iterator: int):
-        if not in_iterator < self.max_possible:
-            return []
+                number_of_elements -= 1
+                in_number_of_selection -= 1
 
-        bin_list, element_list = in_list_to_bin(self.element_list)
+                target_iterator += 1
 
-        result_iterator = self.__permutation_recursive(
-            in_iterator, bin_list, self.in_number_of_selection
-        )
+        if self.must_have_elements:
+            for element in self.must_have_list:
+                result_list.append(element)
 
-        result_list = []
-        for i in result_iterator:
-            result_list.append(element_list[i])
+        return sorted(result_list)
 
-        return result_list
+
+if __name__ == "__main__":
+    generator = CombinationGenerator()
+    generator.set_parameters(4, [1, 2, 3, 4, 5])
+
+    print(generator.all_case())
```

### Comparing `casepy-0.0.7/src/casepy/simple_methods.py` & `casepy-0.1.0/src/casepy/simple_methods.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 def factorial(in_target_number: int) -> int:
     result = 1
     for i in range(1, in_target_number + 1):
         result *= i
     return result
 
 
-def combination(in_number_of_elements: int, in_number_of_select: int) -> int:
+def combination_total(in_number_of_elements: int, in_number_of_select: int) -> int:
     if in_number_of_elements == in_number_of_select:
         return 1
     if in_number_of_elements < in_number_of_select:
         return 0
 
     return (int)(
         factorial(in_number_of_elements)
         / (
             factorial(in_number_of_elements - in_number_of_select)
             * factorial(in_number_of_select)
         )
     )
 
 
-def permutation(in_elements_info, in_number_of_select: int) -> int:
-    if type(in_elements_info) == int:
-        return permutation_core(in_elements_info, in_number_of_select)
-    else:
-        setted_elements_list = list(set(in_elements_info))
-        setted_elements_list.sort()
-
-        element_counting = []
-        for element in setted_elements_list:
-            element_counting.append(in_elements_info.count(element))
-
-        result = permutation_core(len(in_elements_info), in_number_of_select)
-        for count in element_counting:
-            result /= factorial(count)
-
-        return int(result)
-
-
-def permutation_core(in_number_of_elements: int, in_number_of_select: int) -> int:
+def permutation_total(in_number_of_elements: int, in_number_of_select: int) -> int:
+    """
+    Return the number of all possible permutation cases (tranditional method).
+
+    Args:
+        in_number_of_elements (int): The number of elements.
+        in_number_of_select (int): The number of selections.
+
+    Returns:
+        int: The number of all possible permutation cases.
+    """
     if in_number_of_elements == in_number_of_select:
         return factorial(in_number_of_elements)
     if in_number_of_elements < in_number_of_select:
         return 0
 
     return (int)(
         factorial(in_number_of_elements)
```

