# Comparing `tmp/daalab-0.5.tar.gz` & `tmp/daalab-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-0.5.tar", last modified: Thu May 23 14:27:46 2024, max compression
+gzip compressed data, was "daalab-0.6.tar", last modified: Thu May 23 17:10:48 2024, max compression
```

## Comparing `daalab-0.5.tar` & `daalab-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.772430 daalab-0.5/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 14:27:46.772297 daalab-0.5/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.5/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.771474 daalab-0.5/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     2035 2024-05-23 13:00:14.000000 daalab-0.5/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    22385 2024-05-23 14:21:29.000000 daalab-0.5/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       28 2024-05-23 14:16:37.000000 daalab-0.5/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 14:27:46.772112 daalab-0.5/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 14:27:46.000000 daalab-0.5/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 14:27:46.772477 daalab-0.5/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 12:55:10.000000 daalab-0.5/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:10:48.906783 daalab-0.6/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 17:10:48.906525 daalab-0.6/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.6/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:10:48.905373 daalab-0.6/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    32334 2024-05-23 17:09:30.000000 daalab-0.6/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    23663 2024-05-23 14:30:55.000000 daalab-0.6/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       28 2024-05-23 17:01:04.000000 daalab-0.6/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:10:48.906277 daalab-0.6/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 17:10:48.000000 daalab-0.6/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 17:10:48.000000 daalab-0.6/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 17:10:48.000000 daalab-0.6/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 17:10:48.000000 daalab-0.6/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 17:10:48.906847 daalab-0.6/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 17:09:58.000000 daalab-0.6/setup.py
```

### Comparing `daalab-0.5/README.md` & `daalab-0.6/README.md`

 * *Files identical despite different names*

### Comparing `daalab-0.5/daalab/codes.py` & `daalab-0.6/daalab/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,72 +62,59 @@
 max_value = fractional_knapsack(weights, values, capacity)
 print("Maximum value that can be obtained:", max_value)'''
     print(code)
 
 
 
 def print_huffman():
-    code = '''option = input("Enter 'string' if you want to enter a string or 'freq' if you want to enter frequencies - ")
-if option=='string':
-    string = input('Enter string')
-elif option == 'freq':
-    n = int(input('Enter number of letters - '))
-    string=''
-    for i in range(n):
-        letter, freq = input('Enter letter and frequency space-separated - ').split()
-        string+= letter*int(freq)
-    
-class NodeTree(object):
-    def __init__(self, left=None, right=None):
-        self.left = left
-        self.right = right
-
-    def children(self):
-        return (self.left, self.right)
-
-    def __str__(self):
-        return "%s_%s" % (self.left, self.right)
-
-
-# Main function implementing huffman coding
-def huffman_code_tree(node, left=True, binString=""):
-    if isinstance(node, str):
-        return {node: binString}
-    left, right = node.children()
-    d = dict()
-    d.update(huffman_code_tree(left, True, binString + "0"))
-    d.update(huffman_code_tree(right, False, binString + "1"))
-    return d
-
+    code = '''import heapq
 
-freq = {}
-for c in string:
-    if c in freq:
-        freq[c] += 1
+class Node:
+    def __init__(self, freq, symbol):
+        self.freq = freq
+        self.symbol = symbol
+        self.left = None
+        self.right = None
+
+    def __lt__(self, other):
+        return self.freq < other.freq
+
+def huffman_codes(chars, freq):
+    pq = []
+    for i in range(len(chars)):
+        heapq.heappush(pq, Node(freq[i], chars[i]))
+
+    while len(pq) > 1:
+        node1 = heapq.heappop(pq)
+        node2 = heapq.heappop(pq)
+        merged_freq = node1.freq + node2.freq
+        merged_node = Node(merged_freq, None)
+        merged_node.left = node1
+        merged_node.right = node2
+        heapq.heappush(pq, merged_node)
+
+    root = pq[0]
+    codes = {}
+    build_codes(root, "", codes)
+    return codes
+
+def build_codes(node, code, codes):
+    if node.symbol:
+        codes[node.symbol] = code
     else:
-        freq[c] = 1
-
-freq = sorted(freq.items(), key=lambda x: x[1], reverse=True)
-
-nodes = freq
-
-while len(nodes) > 1:
-    (key1, c1) = nodes[-1]
-    (key2, c2) = nodes[-2]
-    nodes = nodes[:-2]
-    node = NodeTree(key1, key2)
-    nodes.append((node, c1 + c2))
-    nodes = sorted(nodes, key=lambda x: x[1], reverse=True)
+        build_codes(node.left, code + "0", codes)
+        build_codes(node.right, code + "1", codes)
 
-huffmanCode = huffman_code_tree(nodes[0][0])
+chars = input("Enter characters separated by spaces: ").split()
+freq = list(map(int, input("Enter corresponding frequencies separated by spaces: ").split()))
 
-print(" Char | Huffman code ")
-print("----------------------")
-for char, frequency in freq:
-    print(" %-4r |%12s" % (char, huffmanCode[char]))'''
+codes = huffman_codes(chars, freq)
+print("Huffman Codes:")
+for char, code in codes.items():
+    print(f"{char}: {code}")'''
     print(code)
 
 
 def print_queen1():
     code = '''def solve_n_queens(n):
     def solve(board, row):
         if row == n:
@@ -848,7 +835,68 @@
 print(graph)
 source = input("enter source - ")
 
 shortest_distances = bellman_ford(graph, source)
 print(shortest_distances)'''
     print(code)
 
+
+def print_huffman2():
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
+    else:
+        freq[c] = 1
+
+freq = sorted(freq.items(), key=lambda x: x[1], reverse=True)
+
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
+    print(code)
```

