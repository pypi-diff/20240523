# Comparing `tmp/fast_viterbi-0.1.0.tar.gz` & `tmp/fast_viterbi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_viterbi-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "fast_viterbi-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fast_viterbi-0.1.0.tar` & `fast_viterbi-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/.clang-format
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2156 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/.gitignore
--rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/LICENSE
--rw-r--r--   0        0        0     3612 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/Makefile
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/README.md
--rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/noxfile.py
--rw-r--r--   0        0        0     2408 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/src/fast_viterbi/__init__.py
--rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/src/fast_viterbi/__main__.py
--rw-r--r--   0        0        0    13136 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/src/main.cpp
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/tests/test_basic.py
--rw-r--r--   0        0        0      757 2022-11-09 12:37:21.000000 fast_viterbi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.clang-format
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2156 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3612 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/Makefile
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/README.md
+-rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/noxfile.py
+-rw-r--r--   0        0        0     2408 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/src/fast_viterbi/__init__.py
+-rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/src/fast_viterbi/__main__.py
+-rw-r--r--   0        0        0    14859 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/src/main.cpp
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/tests/test_basic.py
+-rw-r--r--   0        0        0      757 2022-11-09 12:37:21.000000 fast_viterbi-0.1.1/PKG-INFO
```

### Comparing `fast_viterbi-0.1.0/.github/workflows/pip.yml` & `fast_viterbi-0.1.1/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/.github/workflows/wheels.yml` & `fast_viterbi-0.1.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/.gitignore` & `fast_viterbi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/.pre-commit-config.yaml` & `fast_viterbi-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/CMakeLists.txt` & `fast_viterbi-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/LICENSE` & `fast_viterbi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/Makefile` & `fast_viterbi-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/noxfile.py` & `fast_viterbi-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `fast_viterbi-0.1.0/pyproject.toml` & `fast_viterbi-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core>=0.3.3", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "fast_viterbi"
-version = "0.1.0"
+version = "0.1.1"
 description="a viterbi algo collection"
 readme = "README.md"
 authors = [
   { name = "district10", email = "dvorak4tzx@gmail.com" },
 ]
 dependencies = [
   "fire",
```

### Comparing `fast_viterbi-0.1.0/src/main.cpp` & `fast_viterbi-0.1.1/src/main.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         auto roads = road_path;
         roads.reserve(roads.size() + more_roads.size());
         roads.insert(roads.end(), more_roads.begin(), more_roads.end());
         return Seq(std::move(nodes), std::move(roads));
     }
 };
 
+using Roads = std::unordered_set<std::vector<int64_t>, hash_vector<std::vector<int64_t>>>;
+
 namespace std {
 template <>
 struct hash<Seq> {
     size_t operator()(const Seq &s) const noexcept { return hash_vector<decltype(s.node_path)>()(s.node_path); }
 };
 }  // namespace std
 
@@ -205,14 +207,58 @@
                 sp_paths_.clear();
                 return false;
             }
         }
         return true;
     }
 
+    std::vector<std::vector<int64_t>> all_road_paths() const {
+        if (roads_.empty() || sp_paths_.empty()) {
+            return {};
+        }
+        std::vector<Roads> prev_paths(K_);
+        for (auto &pair : heads_) {
+            auto cidx = pair.first;
+            auto nidx = roads_[0][cidx];
+            prev_paths[cidx].insert({nidx});
+        }
+        for (int n = 0; n < N_ - 1; ++n) {
+            std::vector<Roads> curr_paths(K_);
+            auto &paths = sp_paths_.at(n);
+            auto &layer = links_[n];
+            for (int i = 0; i < K_; ++i) {
+                const auto &heads = prev_paths[i];
+                if (heads.empty() || layer[i].empty()) {
+                    continue;
+                }
+                auto &p = paths.at(i);
+                for (auto &pair : layer[i]) {
+                    int j = pair.first;
+                    const auto &sig = p.at(j);
+                    if (sig.size() == 1) {
+                        curr_paths[j].insert(heads.begin(), heads.end());
+                        continue;
+                    }
+                    for (auto copy : heads) {
+                        copy.insert(copy.end(), sig.begin() + 1, sig.end());
+                        curr_paths[j].insert(std::move(copy));
+                    }
+                }
+            }
+            prev_paths = std::move(curr_paths);
+        }
+        Roads ret;
+        for (auto seqs : prev_paths) {
+            for (auto &seq : seqs) {
+                ret.insert(seq);
+            }
+        }
+        return {ret.begin(), ret.end()};
+    }
+
     std::tuple<double, std::vector<int>, std::vector<int64_t>> inference(const std::vector<int64_t> &road_path) const {
         if (roads_.empty() || sp_paths_.empty()) {
             return std::make_tuple(pos_inf, std::vector<int>{}, std::vector<int64_t>{});
         }
         if (road_path.empty()) {
             return std::make_tuple(pos_inf, std::vector<int>{}, std::vector<int64_t>{});
         }
@@ -357,14 +403,15 @@
         .def("scores", &FastViterbi::scores, "node_path")
         //
         .def("inference", py::overload_cast<>(&FastViterbi::inference, py::const_))
         //
         .def("setup_roads", &FastViterbi::setup_roads, "roads"_a)
         .def("setup_shortest_road_paths", &FastViterbi::setup_shortest_road_paths, "sp_paths"_a)
         //
+        .def("all_road_paths", &FastViterbi::all_road_paths)
         .def("inference", py::overload_cast<const std::vector<int64_t> &>(&FastViterbi::inference, py::const_),
              "road_path"_a, py::call_guard<py::gil_scoped_release>())
 
         //
         ;
 
 #ifdef VERSION_INFO
```

### Comparing `fast_viterbi-0.1.0/PKG-INFO` & `fast_viterbi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_viterbi
-Version: 0.1.0
+Version: 0.1.1
 Summary: a viterbi algo collection
 Author-Email: district10 <dvorak4tzx@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

