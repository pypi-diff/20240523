# Comparing `tmp/cygv-0.0.1.tar.gz` & `tmp/cygv-0.0.2.tar.gz`

## Comparing `cygv-0.0.1.tar` & `cygv-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 cygv-0.0.1/Cargo.toml
--rw-r--r--   0     1001      127      268 2024-05-19 22:27:33.000000 cygv-0.0.1/.github/dependabot.yml
--rw-r--r--   0     1001      127     2582 2024-05-19 22:27:33.000000 cygv-0.0.1/.github/workflows/deploy.yml
--rw-r--r--   0     1001      127      739 2024-05-19 22:27:33.000000 cygv-0.0.1/.github/workflows/python.yml
--rw-r--r--   0     1001      127      575 2024-05-19 22:27:33.000000 cygv-0.0.1/.github/workflows/rust.yml
--rw-r--r--   0     1001      127     1092 2024-05-19 22:27:33.000000 cygv-0.0.1/.gitignore
--rw-r--r--   0     1001      127    10838 2024-05-19 22:27:33.000000 cygv-0.0.1/LICENSE-APACHE
--rw-r--r--   0     1001      127     1062 2024-05-19 22:27:33.000000 cygv-0.0.1/LICENSE-MIT
--rw-r--r--   0     1001      127     1382 2024-05-19 22:27:33.000000 cygv-0.0.1/README.md
--rw-r--r--   0     1001      127     1039 2024-05-19 22:27:33.000000 cygv-0.0.1/docs-header.html
--rw-r--r--   0     1001      127       96 2024-05-19 22:27:33.000000 cygv-0.0.1/python/cygv/__init__.py
--rw-r--r--   0     1001      127     2030 2024-05-19 22:27:33.000000 cygv-0.0.1/python/cygv/hkty.py
--rw-r--r--   0     1001      127     3342 2024-05-19 22:27:33.000000 cygv-0.0.1/python/tests/test_hkty.py
--rw-r--r--   0     1001      127     4694 2024-05-19 22:27:33.000000 cygv-0.0.1/src/factorial.rs
--rw-r--r--   0     1001      127      818 2024-05-19 22:27:33.000000 cygv-0.0.1/src/fundamental_period/error.rs
--rw-r--r--   0     1001      127    21776 2024-05-19 22:27:33.000000 cygv-0.0.1/src/fundamental_period.rs
--rw-r--r--   0     1001      127     7295 2024-05-19 22:27:33.000000 cygv-0.0.1/src/hkty.rs
--rw-r--r--   0     1001      127    15034 2024-05-19 22:27:33.000000 cygv-0.0.1/src/instanton.rs
--rw-r--r--   0     1001      127     2002 2024-05-19 22:27:33.000000 cygv-0.0.1/src/lib.rs
--rw-r--r--   0     1001      127     1051 2024-05-19 22:27:33.000000 cygv-0.0.1/src/misc/error.rs
--rw-r--r--   0     1001      127     2969 2024-05-19 22:27:33.000000 cygv-0.0.1/src/misc.rs
--rw-r--r--   0     1001      127     1854 2024-05-19 22:27:33.000000 cygv-0.0.1/src/polynomial/coefficient.rs
--rw-r--r--   0     1001      127      741 2024-05-19 22:27:33.000000 cygv-0.0.1/src/polynomial/error.rs
--rw-r--r--   0     1001      127     1579 2024-05-19 22:27:33.000000 cygv-0.0.1/src/polynomial/prettyprint.rs
--rw-r--r--   0     1001      127      987 2024-05-19 22:27:33.000000 cygv-0.0.1/src/polynomial/properties.rs
--rw-r--r--   0     1001      127    29751 2024-05-19 22:27:33.000000 cygv-0.0.1/src/polynomial.rs
--rw-r--r--   0     1001      127     1690 2024-05-19 22:27:33.000000 cygv-0.0.1/src/pool.rs
--rw-r--r--   0     1001      127     3908 2024-05-19 22:27:33.000000 cygv-0.0.1/src/python.rs
--rw-r--r--   0     1001      127      707 2024-05-19 22:27:33.000000 cygv-0.0.1/src/semigroup/error.rs
--rw-r--r--   0     1001      127    12158 2024-05-19 22:27:33.000000 cygv-0.0.1/src/semigroup.rs
--rw-r--r--   0     1001      127      555 2024-05-19 22:27:33.000000 cygv-0.0.1/src/series_inversion/error.rs
--rw-r--r--   0     1001      127    12877 2024-05-19 22:27:33.000000 cygv-0.0.1/src/series_inversion.rs
--rw-r--r--   0     1001      127     3911 2024-05-19 22:27:33.000000 cygv-0.0.1/tests/full_hkty.rs
--rw-r--r--   0     1001      127    13389 2024-05-19 22:27:36.000000 cygv-0.0.1/Cargo.lock
--rw-r--r--   0     1001      127     1396 2024-05-19 22:27:33.000000 cygv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 cygv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 cygv-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      127      268 2024-05-22 23:37:17.000000 cygv-0.0.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     2582 2024-05-22 23:37:17.000000 cygv-0.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      127      739 2024-05-22 23:37:17.000000 cygv-0.0.2/.github/workflows/python.yml
+-rw-r--r--   0     1001      127      575 2024-05-22 23:37:17.000000 cygv-0.0.2/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127     1092 2024-05-22 23:37:17.000000 cygv-0.0.2/.gitignore
+-rw-r--r--   0     1001      127     1934 2024-05-22 23:37:17.000000 cygv-0.0.2/CHANGELOG.md
+-rw-r--r--   0     1001      127    10838 2024-05-22 23:37:17.000000 cygv-0.0.2/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1062 2024-05-22 23:37:17.000000 cygv-0.0.2/LICENSE-MIT
+-rw-r--r--   0     1001      127     1804 2024-05-22 23:37:17.000000 cygv-0.0.2/README.md
+-rw-r--r--   0     1001      127     3450 2024-05-22 23:37:17.000000 cygv-0.0.2/cliff.toml
+-rw-r--r--   0     1001      127     1039 2024-05-22 23:37:17.000000 cygv-0.0.2/docs-header.html
+-rw-r--r--   0     1001      127       96 2024-05-22 23:37:17.000000 cygv-0.0.2/python/cygv/__init__.py
+-rw-r--r--   0     1001      127     2030 2024-05-22 23:37:17.000000 cygv-0.0.2/python/cygv/hkty.py
+-rw-r--r--   0     1001      127     4982 2024-05-22 23:37:17.000000 cygv-0.0.2/python/tests/test_hkty.py
+-rw-r--r--   0     1001      127     4686 2024-05-22 23:37:17.000000 cygv-0.0.2/src/factorial.rs
+-rw-r--r--   0     1001      127      818 2024-05-22 23:37:17.000000 cygv-0.0.2/src/fundamental_period/error.rs
+-rw-r--r--   0     1001      127    21864 2024-05-22 23:37:17.000000 cygv-0.0.2/src/fundamental_period.rs
+-rw-r--r--   0     1001      127     7295 2024-05-22 23:37:17.000000 cygv-0.0.2/src/hkty.rs
+-rw-r--r--   0     1001      127    14988 2024-05-22 23:37:17.000000 cygv-0.0.2/src/instanton.rs
+-rw-r--r--   0     1001      127     2003 2024-05-22 23:37:17.000000 cygv-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      127     1051 2024-05-22 23:37:17.000000 cygv-0.0.2/src/misc/error.rs
+-rw-r--r--   0     1001      127     2969 2024-05-22 23:37:17.000000 cygv-0.0.2/src/misc.rs
+-rw-r--r--   0     1001      127     1854 2024-05-22 23:37:17.000000 cygv-0.0.2/src/polynomial/coefficient.rs
+-rw-r--r--   0     1001      127      741 2024-05-22 23:37:17.000000 cygv-0.0.2/src/polynomial/error.rs
+-rw-r--r--   0     1001      127     1579 2024-05-22 23:37:17.000000 cygv-0.0.2/src/polynomial/prettyprint.rs
+-rw-r--r--   0     1001      127      987 2024-05-22 23:37:17.000000 cygv-0.0.2/src/polynomial/properties.rs
+-rw-r--r--   0     1001      127    29754 2024-05-22 23:37:17.000000 cygv-0.0.2/src/polynomial.rs
+-rw-r--r--   0     1001      127     1690 2024-05-22 23:37:17.000000 cygv-0.0.2/src/pool.rs
+-rw-r--r--   0     1001      127     5495 2024-05-22 23:37:17.000000 cygv-0.0.2/src/python.rs
+-rw-r--r--   0     1001      127      707 2024-05-22 23:37:17.000000 cygv-0.0.2/src/semigroup/error.rs
+-rw-r--r--   0     1001      127    12158 2024-05-22 23:37:17.000000 cygv-0.0.2/src/semigroup.rs
+-rw-r--r--   0     1001      127      555 2024-05-22 23:37:17.000000 cygv-0.0.2/src/series_inversion/error.rs
+-rw-r--r--   0     1001      127    13193 2024-05-22 23:37:17.000000 cygv-0.0.2/src/series_inversion.rs
+-rw-r--r--   0     1001      127     3911 2024-05-22 23:37:17.000000 cygv-0.0.2/tests/full_hkty.rs
+-rw-r--r--   0     1001      127    13389 2024-05-22 23:37:20.000000 cygv-0.0.2/Cargo.lock
+-rw-r--r--   0     1001      127     1460 2024-05-22 23:37:17.000000 cygv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3359 1970-01-01 00:00:00.000000 cygv-0.0.2/PKG-INFO
```

### Comparing `cygv-0.0.1/.github/workflows/deploy.yml` & `cygv-0.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/.github/workflows/python.yml` & `cygv-0.0.2/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/.github/workflows/rust.yml` & `cygv-0.0.2/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/.gitignore` & `cygv-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/LICENSE-APACHE` & `cygv-0.0.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/LICENSE-MIT` & `cygv-0.0.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/README.md` & `cygv-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # cygv
 
-[![Rust CI](https://github.com/ariostas/cygv/actions/workflows/rust.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/rust.yml)
+[![Rust CI](https://github.com/ariostas/cygv/actions/workflows/rust.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/rust.yml) [![Python CI](https://github.com/ariostas/cygv/actions/workflows/python.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/python.yml) [![Crates.io Version](https://img.shields.io/crates/v/cygv)](https://crates.io/crates/cygv) [![PyPI - Version](https://img.shields.io/pypi/v/cygv)](https://pypi.org/project/cygv/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/cygv)](https://pypi.org/project/cygv/)
 
 > [!WARNING]
 > This project is still in early stages. The code and documentation are under active development and may change significantly.
 
 This project implements an efficient algorithm to perform the HKTY procedure [[1], [2]] to compute Gopakumar-Vafa (GV) and Gromov-Witten (GW) invariants of Calabi-Yau (CY) manifolds obtained as hypersurfaces or complete intersections in toric varieties. This project is based on the work presented in the paper "[Computational Mirror Symmetry]", but written in the Rust programming language and with some additional improvements.
 
 ## License
```

### Comparing `cygv-0.0.1/docs-header.html` & `cygv-0.0.2/docs-header.html`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/python/cygv/hkty.py` & `cygv-0.0.2/python/cygv/hkty.py`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/python/tests/test_hkty.py` & `cygv-0.0.2/python/tests/test_hkty.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,69 @@
     intnums = [[0, 0, 0, 2], [0, 0, 1, 1], [0, 1, 1, -1], [1, 1, 1, -5]]
     # For now, these are just smoke tests
     compute_gv(generators, grading_vector, q, intnums, min_points=100)
     compute_gv(generators, grading_vector, q, intnums, min_points=100, prec=200)
     compute_gw(generators, grading_vector, q, intnums, min_points=100)
     compute_gw(generators, grading_vector, q, intnums, min_points=100, prec=200)
 
+    generators = [
+        [-1, 0, 0, 0, 0, 1, -1],
+        [0, 0, 0, 0, 0, -2, 1],
+        [0, 0, 0, 0, 0, -1, 1],
+        [0, 0, 0, 0, 0, 0, 1],
+        [0, 0, 0, 1, -1, 0, 0],
+        [0, 0, 1, -1, 1, 0, 0],
+        [0, 0, 1, 0, 0, 1, 0],
+        [1, 0, 0, 0, 1, 0, -1],
+        [1, 1, 0, 0, 0, -2, 0],
+    ]
+    grading_vector = [-2, 3, 2, 5, 4, 0, 1]
+    q = [
+        [-1, 1, 0, 0, -1, 0, 0, 0, -1, 0, 0],
+        [1, 0, 1, 0, 3, 0, -2, 0, -1, 0, 0],
+        [1, 0, 0, 1, -1, 0, 1, 0, 0, 0, 0],
+        [2, 0, 0, 0, 2, 1, -2, 0, 1, 0, 0],
+        [2, 0, 0, 0, 3, 0, -3, 1, 1, 0, 0],
+        [0, 0, 0, 0, 1, 0, -1, 0, -1, 1, 0],
+        [1, 0, 0, 0, 2, 0, -2, 0, 0, 0, 1],
+    ]
+    intnums = [
+        [0, 5, 6, 1],
+        [1, 2, 3, 2],
+        [1, 3, 4, 2],
+        [1, 4, 6, 1],
+        [1, 5, 6, 1],
+        [0, 0, 2, -2],
+        [0, 0, 6, -1],
+        [0, 5, 5, -2],
+        [0, 6, 6, -1],
+        [1, 2, 2, 4],
+        [1, 3, 3, -2],
+        [1, 4, 4, -2],
+        [1, 5, 5, -2],
+        [1, 6, 6, -2],
+        [2, 2, 2, 24],
+        [2, 2, 3, 8],
+        [2, 3, 3, 2],
+        [3, 3, 3, -12],
+        [3, 3, 4, 10],
+        [3, 4, 4, -8],
+        [4, 4, 4, 6],
+        [4, 4, 6, 1],
+        [4, 6, 6, -3],
+        [5, 5, 5, 8],
+        [5, 5, 6, -2],
+        [6, 6, 6, 7],
+    ]
+    # For now, these are just smoke tests
+    compute_gv(generators, grading_vector, q, intnums, min_points=100)
+    compute_gv(generators, grading_vector, q, intnums, min_points=100, prec=200)
+    compute_gw(generators, grading_vector, q, intnums, min_points=100)
+    compute_gw(generators, grading_vector, q, intnums, min_points=100, prec=200)
+
 
 def test_fourfold():
     generators = [
         [0, 0, 0, -2, 3, 0],
         [1, 0, -4, 0, 0, 0],
         [0, 0, 1, 1, 0, 0],
         [0, 1, 0, 0, 1, -2],
```

### Comparing `cygv-0.0.1/src/factorial.rs` & `cygv-0.0.2/src/factorial.rs`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,16 @@
         let mut true_rat = Rational::new();
 
         let prec = 512;
         let mut res_float = Float::new(prec);
         let mut tmp_float = Float::new(prec);
         let mut true_float = Float::new(prec);
 
-        let n_m = vec![(0, 1), (1, 1), (10, 1), (10, 2)];
-        let h_n_m = vec![(0, 1), (1, 1), (7_381, 2_520), (1_968_329, 1_270_080)];
+        let n_m = [(0, 1), (1, 1), (10, 1), (10, 2)];
+        let h_n_m = [(0, 1), (1, 1), (7_381, 2_520), (1_968_329, 1_270_080)];
 
         for (h, (n, m)) in h_n_m.iter().zip(n_m.iter()) {
             harmonic(*n, *m, &mut res_rat, &mut tmp_rat);
             harmonic(*n, *m, &mut res_float, &mut tmp_float);
 
             true_rat.assign(*h);
             true_float.assign(&true_rat);
```

### Comparing `cygv-0.0.1/src/fundamental_period/error.rs` & `cygv-0.0.2/src/fundamental_period/error.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/fundamental_period.rs` & `cygv-0.0.2/src/fundamental_period.rs`

 * *Files 3% similar despite different names*

```diff
@@ -267,26 +267,32 @@
         let (neg_idx2, neg_int2) = neg_ints_iter
             .next()
             .expect("the curve only has one negative intersection");
         assert!(
             neg_ints_iter.next().is_none(),
             "the curve has more than two negative intersections"
         );
+        let sn = if (neg_int1 + neg_int2) % 2 == 0 {
+            1
+        } else {
+            -1
+        };
 
         let mut n: Vec<_> = curves_dot_q0.column(t).iter().map(|c| *c as u32).collect();
         n.push((-neg_int1 - 1) as u32);
         n.push((-neg_int2 - 1) as u32);
         let d: Vec<_> = curves_dot_q
             .column(t)
             .iter()
             .enumerate()
             .filter(|(i, _)| *i != neg_idx1 && *i != neg_idx2)
             .map(|(_, c)| *c as u32)
             .collect();
         factorial_prod(&n, &d, &mut tmp_fact);
+        tmp_fact *= sn;
         for &(aa, bb) in beta_pairs.iter() {
             tmp_final.assign(&tmp_fact);
             tmp_final *=
                 q[(neg_idx1, aa)] * q[(neg_idx2, bb)] + q[(neg_idx1, bb)] * q[(neg_idx2, aa)];
             tx.send((
                 t as u32,
                 Some(aa as u32),
@@ -527,48 +533,48 @@
         let grading_vector = RowDVector::from_row_slice(&[3, -1]);
         let sg = Semigroup::with_min_elements(generators, grading_vector, 15).unwrap();
         let zero_rat = Rational::new();
         let poly_props = PolynomialProperties::new(&sg, &zero_rat);
 
         let q = DMatrix::from_column_slice(6, 2, &[1, 1, 1, 0, 1, 2, 0, 0, -1, 1, 1, -1]);
         let nefpart = Vec::new();
-        let intnum_idxpairs = vec![(0, 0), (0, 1), (1, 1)].iter().cloned().collect();
+        let intnum_idxpairs = [(0, 0), (0, 1), (1, 1)].iter().cloned().collect();
 
         let fp = compute_omega(&poly_props, &sg, &q, &nefpart, &intnum_idxpairs);
         assert!(fp.is_ok());
         let fp = fp.unwrap();
 
         let c0_size = 4;
         let c0_coeffs = vec![1, 360, 1247400];
-        let c0_coeffs: HashSet<_> = c0_coeffs.into_iter().map(|c| Rational::from(c)).collect();
+        let c0_coeffs: HashSet<_> = c0_coeffs.into_iter().map(Rational::from).collect();
         assert_eq!(fp.c0.nonzero.len(), c0_size);
         assert_eq!(
             fp.c0.coeffs.clone().into_values().collect::<HashSet<_>>(),
             c0_coeffs
         );
 
         let c1_0_size = 9;
         let c1_0_coeffs = vec![
             60, -6930, 3312, 166320, 2772, 1361360, -36756720, -334639305, 13142520,
         ];
-        let c1_0_coeffs: HashSet<_> = c1_0_coeffs.into_iter().map(|c| Rational::from(c)).collect();
+        let c1_0_coeffs: HashSet<_> = c1_0_coeffs.into_iter().map(Rational::from).collect();
         assert_eq!(fp.c1[0].nonzero.len(), c1_0_size);
         assert_eq!(
             fp.c1[0]
                 .coeffs
                 .clone()
                 .into_values()
                 .collect::<HashSet<_>>(),
             c1_0_coeffs
         );
         let c1_1_size = 10;
         let c1_1_coeffs = vec![
             -60, 6930, -540, -1361360, -166320, 540, -2598750, 60, 36756720, 334639305,
         ];
-        let c1_1_coeffs: HashSet<_> = c1_1_coeffs.into_iter().map(|c| Rational::from(c)).collect();
+        let c1_1_coeffs: HashSet<_> = c1_1_coeffs.into_iter().map(Rational::from).collect();
         assert_eq!(fp.c1[1].nonzero.len(), c1_1_size);
         assert_eq!(
             fp.c1[1]
                 .coeffs
                 .clone()
                 .into_values()
                 .collect::<HashSet<_>>(),
@@ -585,15 +591,15 @@
             (317945960, 9),
             (-851735880, 1),
             (-18140848109_i64, 2_i64),
             (79322526, 1),
         ];
         let c2_00_coeffs: HashSet<_> = c2_00_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(fp.c2[&(0, 0)].nonzero.len(), c2_00_size);
         assert_eq!(
             fp.c2[&(0, 0)]
                 .coeffs
                 .clone()
                 .into_values()
@@ -615,15 +621,15 @@
             (1, 16),
             (452, 1),
             (-57445875, 2),
             (23478658899_i64, 4_i64),
         ];
         let c2_01_coeffs: HashSet<_> = c2_01_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(fp.c2[&(0, 1)].nonzero.len(), c2_01_size);
         assert_eq!(
             fp.c2[&(0, 1)]
                 .coeffs
                 .clone()
                 .into_values()
@@ -645,15 +651,15 @@
             (1, 8),
             (400, 1),
             (10308375, 1),
             (-2668905395_i64, 1_i64),
         ];
         let c2_11_coeffs: HashSet<_> = c2_11_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(fp.c2[&(1, 1)].nonzero.len(), c2_11_size);
         assert_eq!(
             fp.c2[&(1, 1)]
                 .coeffs
                 .clone()
                 .into_values()
```

### Comparing `cygv-0.0.1/src/hkty.rs` & `cygv-0.0.2/src/hkty.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/instanton.rs` & `cygv-0.0.2/src/instanton.rs`

 * *Files 3% similar despite different names*

```diff
@@ -328,15 +328,15 @@
         let grading_vector = RowDVector::from_row_slice(&[3, -1]);
         let sg = Semigroup::with_min_elements(generators, grading_vector, 15).unwrap();
         let zero_rat = Rational::new();
         let poly_props = PolynomialProperties::new(&sg, &zero_rat);
 
         let q = DMatrix::from_column_slice(6, 2, &[1, 1, 1, 0, 1, 2, 0, 0, -1, 1, 1, -1]);
         let nefpart = Vec::new();
-        let intnum_idxpairs = vec![(0, 0), (0, 1), (1, 1)].iter().cloned().collect();
+        let intnum_idxpairs = [(0, 0), (0, 1), (1, 1)].iter().cloned().collect();
 
         let fp = compute_omega(&poly_props, &sg, &q, &nefpart, &intnum_idxpairs);
         assert!(fp.is_ok());
         let fp = fp.unwrap();
 
         let intnums = dmatrix![ 0, 0, 0, 1;
                                 0, 0,  1,  1;
@@ -366,15 +366,15 @@
             (6958792, 1),
             (-168359184, 1),
             (-7042450329_i64, 4_i64),
             (33379857, 1),
         ];
         let inst0_coeffs: HashSet<_> = inst0_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.inst[0].nonzero.len(), inst0_size);
         assert_eq!(
             inst_data.inst[0]
                 .coeffs
                 .clone()
                 .into_values()
@@ -397,15 +397,15 @@
             (-7042450329_i64, 2_i64),
             (-336718368, 1),
             (-3, 8),
             (32846391, 1),
         ];
         let inst1_coeffs: HashSet<_> = inst1_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.inst[1].nonzero.len(), inst1_size);
         assert_eq!(
             inst_data.inst[1]
                 .coeffs
                 .clone()
                 .into_values()
@@ -415,15 +415,15 @@
 
         let expalpha_pos0_size = 10;
         let expalpha_pos0_coeffs = vec![
             1, 60, 3312, -5130, 2772, 343440, 981560, -42569280, 17579592, -240879255,
         ];
         let expalpha_pos0_coeffs: HashSet<_> = expalpha_pos0_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.expalpha[0].0.nonzero.len(), expalpha_pos0_size);
         assert_eq!(
             inst_data.expalpha[0]
                 .0
                 .coeffs
                 .clone()
@@ -434,15 +434,15 @@
 
         let expalpha_pos1_size = 11;
         let expalpha_pos1_coeffs = vec![
             1, -60, -540, 8730, 540, -112320, -1813160, 38230920, -2269350, 60, 453347355,
         ];
         let expalpha_pos1_coeffs: HashSet<_> = expalpha_pos1_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.expalpha[1].0.nonzero.len(), expalpha_pos1_size);
         assert_eq!(
             inst_data.expalpha[1]
                 .0
                 .coeffs
                 .clone()
@@ -453,15 +453,15 @@
 
         let expalpha_neg0_size = 10;
         let expalpha_neg0_coeffs = vec![
             1, -60, 8730, -3312, -2772, -1813160, 54000, 14031360, -6277608, 453347355,
         ];
         let expalpha_neg0_coeffs: HashSet<_> = expalpha_neg0_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.expalpha[0].1.nonzero.len(), expalpha_neg0_size);
         assert_eq!(
             inst_data.expalpha[0]
                 .1
                 .coeffs
                 .clone()
@@ -472,15 +472,15 @@
 
         let expalpha_neg1_size = 11;
         let expalpha_neg1_coeffs = vec![
             1, 60, -5130, 540, -540, 981560, 177120, -28348920, 2496150, -240879255, -60,
         ];
         let expalpha_neg1_coeffs: HashSet<_> = expalpha_neg1_coeffs
             .into_iter()
-            .map(|c| Rational::from(c))
+            .map(Rational::from)
             .collect();
         assert_eq!(inst_data.expalpha[1].1.nonzero.len(), expalpha_neg1_size);
         assert_eq!(
             inst_data.expalpha[1]
                 .1
                 .coeffs
                 .clone()
```

### Comparing `cygv-0.0.1/src/lib.rs` & `cygv-0.0.2/src/lib.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
 // Re-export python module
 #[doc(inline)]
 pub use python::cygv;
 
 // Re-export main functions
 #[doc(inline)]
-pub use hkty::*;
+pub use hkty::*;
```

### Comparing `cygv-0.0.1/src/misc/error.rs` & `cygv-0.0.2/src/misc/error.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/misc.rs` & `cygv-0.0.2/src/misc.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/polynomial/coefficient.rs` & `cygv-0.0.2/src/polynomial/coefficient.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/polynomial/error.rs` & `cygv-0.0.2/src/polynomial/error.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/polynomial/prettyprint.rs` & `cygv-0.0.2/src/polynomial/prettyprint.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/polynomial/properties.rs` & `cygv-0.0.2/src/polynomial/properties.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/polynomial.rs` & `cygv-0.0.2/src/polynomial.rs`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     pub fn clone(&self, coeff_pool: &mut NumberPool<T>) -> Self {
         let mut res = Self::new();
         for (i, c) in self.coeffs.iter() {
             let mut coeff = coeff_pool.pop();
             coeff.assign(c);
             res.coeffs.insert(*i, coeff);
         }
-        res.nonzero = self.nonzero.clone();
+        res.nonzero.clone_from(&self.nonzero);
         res
     }
 
     /// Move all data into another polynomial.
     pub fn move_into(self, other: &mut Self, coeff_pool: &mut NumberPool<T>) {
         for (_, c) in other.coeffs.drain() {
             coeff_pool.push(c);
```

### Comparing `cygv-0.0.1/src/pool.rs` & `cygv-0.0.2/src/pool.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/semigroup/error.rs` & `cygv-0.0.2/src/semigroup/error.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/semigroup.rs` & `cygv-0.0.2/src/semigroup.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/series_inversion/error.rs` & `cygv-0.0.2/src/series_inversion/error.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/src/series_inversion.rs` & `cygv-0.0.2/src/series_inversion.rs`

 * *Files 2% similar despite different names*

```diff
@@ -75,30 +75,42 @@
         closest_curve.nonzero.push(t as u32);
         closest_curve_diff
             .iter_mut()
             .zip(poly_props.semigroup.elements.column(t).iter())
             .for_each(|(d, s)| *d = *s);
         closest_dist = closest_curve_diff
             .iter()
-            .map(|d| (*d as f32).abs().log2() + 1_f32)
+            .map(|d| {
+                if *d == 0 {
+                    0_f32
+                } else {
+                    (*d as f32).abs().log2() + 1_f32
+                }
+            })
             .sum();
         // Now check to see if there is a better starting curve
         for (prev_inds, prev_qns) in previous_qn_ind.iter().zip(previous_qn.iter()) {
             for i in prev_inds {
                 poly_props
                     .semigroup
                     .elements
                     .column(t)
                     .iter()
                     .zip(poly_props.semigroup.elements.column(*i).iter())
                     .zip(tmp_curve_diff.iter_mut())
                     .for_each(|((s1, s2), d)| *d = s1 - s2);
                 tmp_dist = tmp_curve_diff
                     .iter()
-                    .map(|d| (*d as f32).abs().log2() + 1_f32)
+                    .map(|d| {
+                        if *d == 0 {
+                            0_f32
+                        } else {
+                            (*d as f32).abs().log2() + 1_f32
+                        }
+                    })
                     .sum();
                 if tmp_dist < closest_dist {
                     let Some(ind) = poly_props.monomial_map.get(&tmp_curve_diff.as_view()) else {
                         continue;
                     };
                     let mut tmp_poly = Polynomial::new();
                     let mut tmp_num = np.pop();
```

### Comparing `cygv-0.0.1/tests/full_hkty.rs` & `cygv-0.0.2/tests/full_hkty.rs`

 * *Files identical despite different names*

### Comparing `cygv-0.0.1/Cargo.lock` & `cygv-0.0.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cygv"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "itertools",
  "nalgebra",
  "pyo3",
  "rug",
 ]
 
@@ -77,17 +77,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.155"
@@ -420,17 +420,17 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "wide"
-version = "0.7.19"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aab6594190de06d718a5dbc5fa781ab62f8903797056480e549ca74add6b7065"
+checksum = "21e005a4cc35784183a9e39cb22e9a9c46353ef6a7f113fd8d36ddc58c15ef3c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "windows-sys"
```

### Comparing `cygv-0.0.1/pyproject.toml` & `cygv-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -39,10 +39,13 @@
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest",
 ]
 
+[project.urls]
+Repository = "https://github.com/ariostas/cygv"
+
 [tool.maturin]
 python-source = "python"
 features = ["pyo3/extension-module"]
```

### Comparing `cygv-0.0.1/PKG-INFO` & `cygv-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cygv
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -29,18 +29,19 @@
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: Compute GV and GW invariants of CY manifolds.
 Author: Andres Rios Tascon
 License: MIT OR Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/ariostas/cygv
 
 # cygv
 
-[![Rust CI](https://github.com/ariostas/cygv/actions/workflows/rust.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/rust.yml)
+[![Rust CI](https://github.com/ariostas/cygv/actions/workflows/rust.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/rust.yml) [![Python CI](https://github.com/ariostas/cygv/actions/workflows/python.yml/badge.svg)](https://github.com/ariostas/cygv/actions/workflows/python.yml) [![Crates.io Version](https://img.shields.io/crates/v/cygv)](https://crates.io/crates/cygv) [![PyPI - Version](https://img.shields.io/pypi/v/cygv)](https://pypi.org/project/cygv/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/cygv)](https://pypi.org/project/cygv/)
 
 > [!WARNING]
 > This project is still in early stages. The code and documentation are under active development and may change significantly.
 
 This project implements an efficient algorithm to perform the HKTY procedure [[1], [2]] to compute Gopakumar-Vafa (GV) and Gromov-Witten (GW) invariants of Calabi-Yau (CY) manifolds obtained as hypersurfaces or complete intersections in toric varieties. This project is based on the work presented in the paper "[Computational Mirror Symmetry]", but written in the Rust programming language and with some additional improvements.
 
 ## License
```

