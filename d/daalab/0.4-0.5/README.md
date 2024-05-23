# Comparing `tmp/daalab-0.4.tar.gz` & `tmp/daalab-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-0.4.tar", last modified: Thu May 23 12:48:48 2024, max compression
+gzip compressed data, was "daalab-0.5.tar", last modified: Thu May 23 14:27:46 2024, max compression
```

## Comparing `daalab-0.4.tar` & `daalab-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.041705 daalab-0.4/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:48:48.041432 daalab-0.4/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.4/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.039838 daalab-0.4/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     2030 2024-05-23 12:44:31.000000 daalab-0.4/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    21976 2024-05-23 12:30:57.000000 daalab-0.4/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1330 2024-05-23 12:39:22.000000 daalab-0.4/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 12:48:48.041125 daalab-0.4/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 12:48:48.000000 daalab-0.4/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 12:48:48.041760 daalab-0.4/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 12:47:43.000000 daalab-0.4/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.772430 daalab-0.5/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 14:27:46.772297 daalab-0.5/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.5/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.771474 daalab-0.5/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     2035 2024-05-23 13:00:14.000000 daalab-0.5/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    22385 2024-05-23 14:21:29.000000 daalab-0.5/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       28 2024-05-23 14:16:37.000000 daalab-0.5/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.772112 daalab-0.5/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 14:27:46.772477 daalab-0.5/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 12:55:10.000000 daalab-0.5/setup.py
```

### Comparing `daalab-0.4/README.md` & `daalab-0.5/README.md`

 * *Files identical despite different names*

### Comparing `daalab-0.4/daalab/__init__.py` & `daalab-0.5/daalab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 prims = print_prims
 bellman = print_bellman
 
 
 def list():
     functions = {
     "zerone": "space complexity: O(nW) and time complexity: O(nW)",
-    "fracknap": "space complexity: O(1) and time complexity: O(n log n)",
+    "fracknap": "space complexity: O(n) and time complexity: O(n log n)",
     "huffman": "space complexity: O(n) and time complexity: O(n log n)",
     "queen1": "space complexity: O(n) and time complexity: O(n!)",
-    "queen2": "space complexity: O(n) and time complexity: O(n!)",
+    "queen2": "space complexity: O(n^2) and time complexity: O(n!)",
     "graphcol": "space complexity: O(V) and time complexity: O(V+E)",
     "matrixchain": "space complexity: O(n^2) and time complexity: O(n^3)",
     "tspbb": "space complexity: O(n^2) and time complexity: O(n^2 * 2^n)",
     "lcs": "space complexity: O(mn) and time complexity: O(mn)",
     "zeronebb": "space complexity: O(n) and time complexity: O(2^n)",
     "floyed": "space complexity: O(n^2) and time complexity: O(n^3)",
     "tspdp": "space complexity: O(n * 2^n) and time complexity: O(n^2 * 2^n)",
     "jobseq": "space complexity: O(n) and time complexity: O(n log n)",
     "dijkstra": "space complexity: O(V^2) and time complexity: O(V^2)",
     "kruskal": "space complexity: O(E) and time complexity: O(E log V)",
-    "prims": "space complexity: O(V^2) and time complexity: O(V^2)",
+    "prims": "space complexity: O(V+E) and time complexity: O(E logV)",
     "bellman": "space complexity: O(V) and time complexity: O(VE)"
 }
 
 
     print("Available functions in the daalab library:")
     for name, description in functions.items():
         print(f"{name}: {description}")
```

### Comparing `daalab-0.4/daalab/codes.py` & `daalab-0.5/daalab/codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,59 +62,72 @@
 max_value = fractional_knapsack(weights, values, capacity)
 print("Maximum value that can be obtained:", max_value)'''
     print(code)
 
 
 
 def print_huffman():
-    code = '''import heapq
-
-class Node:
-    def __init__(self, freq, symbol):
-        self.freq = freq
-        self.symbol = symbol
-        self.left = None
-        self.right = None
-
-    def __lt__(self, other):
-        return self.freq < other.freq
-
-def huffman_codes(chars, freq):
-    pq = []
-    for i in range(len(chars)):
-        heapq.heappush(pq, Node(freq[i], chars[i]))
-
-    while len(pq) > 1:
-        node1 = heapq.heappop(pq)
-        node2 = heapq.heappop(pq)
-        merged_freq = node1.freq + node2.freq
-        merged_node = Node(merged_freq, None)
-        merged_node.left = node1
-        merged_node.right = node2
-        heapq.heappush(pq, merged_node)
-
-    root = pq[0]
-    codes = {}
-    build_codes(root, "", codes)
-    return codes
-
-def build_codes(node, code, codes):
-    if node.symbol:
-        codes[node.symbol] = code
+    code = '''option = input("Enter 'string' if you want to enter a string or 'freq' if you want to enter frequencies - ")
+if option=='string':
+    string = input('Enter string')
+elif option == 'freq':
+    n = int(input('Enter number of letters - '))
+    string=''
+    for i in range(n):
+        letter, freq = input('Enter letter and frequency space-separated - ').split()
+        string+= letter*int(freq)
+    
+class NodeTree(object):
+    def __init__(self, left=None, right=None):
+        self.left = left
+        self.right = right
+
+    def children(self):
+        return (self.left, self.right)
+
+    def __str__(self):
+        return "%s_%s" % (self.left, self.right)
+
+
+# Main function implementing huffman coding
+def huffman_code_tree(node, left=True, binString=""):
+    if isinstance(node, str):
+        return {node: binString}
+    left, right = node.children()
+    d = dict()
+    d.update(huffman_code_tree(left, True, binString + "0"))
+    d.update(huffman_code_tree(right, False, binString + "1"))
+    return d
+
+
+freq = {}
+for c in string:
+    if c in freq:
+        freq[c] += 1
     else:
-        build_codes(node.left, code + "0", codes)
-        build_codes(node.right, code + "1", codes)
+        freq[c] = 1
 
-chars = input("Enter characters separated by spaces: ").split()
-freq = list(map(int, input("Enter corresponding frequencies separated by spaces: ").split()))
+freq = sorted(freq.items(), key=lambda x: x[1], reverse=True)
 
-codes = huffman_codes(chars, freq)
-print("Huffman Codes:")
-for char, code in codes.items():
-    print(f"{char}: {code}")'''
+nodes = freq
+
+while len(nodes) > 1:
+    (key1, c1) = nodes[-1]
+    (key2, c2) = nodes[-2]
+    nodes = nodes[:-2]
+    node = NodeTree(key1, key2)
+    nodes.append((node, c1 + c2))
+    nodes = sorted(nodes, key=lambda x: x[1], reverse=True)
+
+huffmanCode = huffman_code_tree(nodes[0][0])
+
+print(" Char | Huffman code ")
+print("----------------------")
+for char, frequency in freq:
+    print(" %-4r |%12s" % (char, huffmanCode[char]))'''
     print(code)
 
 
 def print_queen1():
     code = '''def solve_n_queens(n):
     def solve(board, row):
         if row == n:
@@ -424,64 +437,67 @@
 lcs_str, lcs_len = lcs(X, Y)
 print(f"The length of the longest common subsequence is: {lcs_len}")
 print(f"The longest common subsequence is: {lcs_str}")'''
     print(code)
 
 
 def print_01bb():
-    code = '''from collections import namedtuple
-
-Item = namedtuple('Item', ['weight', 'value'])
+    code = '''class Item:
+    def __init__(self, weight, value):
+        self.weight = weight
+        self.value = value
 
 def knapsack_bb(items, capacity):
     def bound(node, weight, value):
         if weight >= capacity:
             return value
-        
+
         bound_value = value
         for item in items[node:]:
             if weight + item.weight <= capacity:
                 bound_value = max(bound_value, value + item.value)
-        
+
         return bound_value
 
     def branch_and_bound(node, weight, value, max_value):
         nonlocal best_value, best_items
-        
+
         if weight <= capacity:
             if value > max_value:
                 max_value = value
-            
+
             if node == len(items):
                 if value > best_value:
                     best_value = value
                     best_items = items_taken[:]
                 return max_value
-            
+
             bound_value = bound(node, weight, value)
             if bound_value > best_value:
                 items_taken.append(items[node])
                 max_value = branch_and_bound(node + 1, weight + items[node].weight, value + items[node].value, max_value)
                 items_taken.pop()
-                
+
                 max_value = branch_and_bound(node + 1, weight, value, max_value)
-        
+
         return max_value
 
     best_value = 0
     best_items = []
     items_taken = []
     max_value = branch_and_bound(0, 0, 0, 0)
-    
+
     return best_value, best_items
 
 # Example usage
 items = []
 for i in range(int(input("Enter number of items: "))):
-    items.append(Item(int(input("Enter Weight: ")),int(input("Enter Value: "))))
+    weight = int(input("Enter Weight: "))
+    value = int(input("Enter Value: "))
+    items.append(Item(weight, value))
 
 capacity = int(input("Enter the max capacity of the knapsack: "))
 
 value, items_taken = knapsack_bb(items, capacity)
 print(f'Maximum value: {value}')
 print(f'Items taken: {[item.value for item in items_taken]}')'''
     print(code)
@@ -820,16 +836,18 @@
         break
     temp = edge.split()
     if len(temp) == 3:
         u, v, w = temp
     elif len(temp) == 1:
         graph[temp[0]] = {}
     w = int(w)
-    if u not in graph:
+   if u not in graph:
         graph[u] = {}
+    if v not in graph:
+        graph[v] = {}
     graph[u][v] = w
 print(graph)
 source = input("enter source - ")
 
 shortest_distances = bellman_ford(graph, source)
 print(shortest_distances)'''
     print(code)
```

