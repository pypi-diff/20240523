# Comparing `tmp/vastdb-0.1.5.tar.gz` & `tmp/vastdb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.5.tar", last modified: Thu May 16 15:22:13 2024, max compression
+gzip compressed data, was "vastdb-0.1.6.tar", last modified: Thu May 23 11:15:59 2024, max compression
```

## Comparing `vastdb-0.1.5.tar` & `vastdb-0.1.6.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     4831 2024-05-16 14:40:09.000000 vastdb-0.1.5/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-16 14:40:09.000000 vastdb-0.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-16 14:40:09.000000 vastdb-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 15:22:13.534700 vastdb-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6037 2024-05-16 14:40:09.000000 vastdb-0.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-16 14:40:09.000000 vastdb-0.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 15:22:13.535700 vastdb-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-16 14:40:09.000000 vastdb-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.498700 vastdb-0.1.5/vast_flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.514700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.525700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.529700 vastdb-0.1.5/vast_flatbuf/tabular/
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ColumnType.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ImportDataRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListTablesResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ObjectDetails.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/S3File.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/VipRange.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.530700 vastdb-0.1.5/vastdb/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.532700 vastdb-0.1.5/vastdb/bench/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vastdb/bench/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/bench/test_perf.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    98490 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/internal_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2603 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/session.py
--rw-rw-rw-   0 root         (0) root         (0)    30031 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/vastdb/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vastdb/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_duckdb.py
--rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_nested.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)    27859 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_tables.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/util.py
--rw-rw-rw-   0 root         (0) root         (0)     2852 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/vastdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9048 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.140398 vastdb-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2024-05-23 11:00:32.000000 vastdb-0.1.6/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-20 13:26:33.000000 vastdb-0.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 13:26:33.000000 vastdb-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 11:15:59.139398 vastdb-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6037 2024-05-20 13:26:33.000000 vastdb-0.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-20 13:26:33.000000 vastdb-0.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 11:15:59.140398 vastdb-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-23 11:00:32.000000 vastdb-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.103397 vastdb-0.1.6/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.103397 vastdb-0.1.6/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.119397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.130398 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.133398 vastdb-0.1.6/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.135398 vastdb-0.1.6/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.137398 vastdb-0.1.6/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4098 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    97586 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/internal_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     5642 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    30646 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.139398 vastdb-0.1.6/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3448 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    28342 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.139398 vastdb-0.1.6/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9048 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.5/CHANGELOG.md` & `vastdb-0.1.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.6] (2024-05-23)
+[0.1.6]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.5...v0.1.6
+
+### Added
+ - Allow listing and querying Catalog snapshots
+ - Support nested schemas
+ - Use automatic split estimation
+
+### Fixed
+ - Allow using specific semi-sorted projection (needs VAST 5.1+ release)
+ - Add a client-side check for too large requests
+
 ## [0.1.5] (2024-05-16)
 [0.1.5]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.4...v0.1.5
 
 ### Added
  - Allow passing `ssl_verify` via `Session` c-tor
  - Retry `requests.exceptions.ConnectionError`
  - Document `QueryConfig` properties
```

### Comparing `vastdb-0.1.5/LICENSE` & `vastdb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/PKG-INFO` & `vastdb-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.5
+Version: 0.1.6
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vastdb-0.1.5/README.md` & `vastdb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/setup.py` & `vastdb-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.5' + suffix,
+    version='0.1.6' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=Path('requirements.txt').read_text().strip().split(),
     long_description=long_description,
```

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.6/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.6/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.6/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.6/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.6/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.6/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.6/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.6/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.6/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.6/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vastdb/bench/test_perf.py` & `vastdb-0.1.6/vastdb/bench/test_perf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import time
 
-import pyarrow as pa
 import pytest
 
 from vastdb import util
 from vastdb.table import ImportConfig, QueryConfig
 
 log = logging.getLogger(__name__)
 
@@ -16,14 +15,14 @@
 
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         s = b.create_schema('s1')
         t = util.create_table_from_files(s, 't1', files, config=ImportConfig(import_concurrency=8))
         config = QueryConfig(num_splits=8, num_sub_splits=4)
         s = time.time()
-        pa_table = pa.Table.from_batches(t.select(columns=['sid'], predicate=t['sid'] == 10033007, config=config))
+        pa_table = t.select(columns=['sid'], predicate=t['sid'] == 10033007, config=config).read_all()
         e = time.time()
         log.info("'SELECT sid from TABLE WHERE sid = 10033007' returned in %s seconds.", e - s)
         if crater_path:
             with open(f'{crater_path}/bench_results', 'a') as f:
                 f.write(f"'SELECT sid FROM TABLE WHERE sid = 10033007' returned in {e - s} seconds")
         assert pa_table.num_rows == 255_075
```

### Comparing `vastdb-0.1.5/vastdb/conftest.py` & `vastdb-0.1.6/vastdb/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,31 @@
 
 
 @pytest.fixture(scope="session")
 def test_bucket_name(request):
     return request.config.getoption("--tabular-bucket-name")
 
 
+def iter_schemas(s):
+    """Recusively scan all schemas."""
+    children = s.schemas()
+    for c in children:
+        yield from iter_schemas(c)
+    yield s
+
+
 @pytest.fixture(scope="function")
 def clean_bucket_name(request, test_bucket_name, session):
     with session.transaction() as tx:
         b = tx.bucket(test_bucket_name)
-        for s in b.schemas():
-            for t in s.tables():
-                t.drop()
-            s.drop()
+        for top_schema in b.schemas():
+            for s in iter_schemas(top_schema):
+                for t in s.tables():
+                    t.drop()
+                s.drop()
     return test_bucket_name
 
 
 @pytest.fixture(scope="session")
 def s3(request):
     return boto3.client(
         's3',
```

### Comparing `vastdb-0.1.5/vastdb/errors.py` & `vastdb-0.1.6/vastdb/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,19 @@
     error_dict: dict
 
 
 class InvalidArgument(Exception):
     pass
 
 
-class TooWideRow(InvalidArgument):
+class TooLargeRequest(InvalidArgument):
+    pass
+
+
+class TooWideRow(TooLargeRequest):
     pass
 
 
 class Missing(Exception):
     pass
```

### Comparing `vastdb-0.1.5/vastdb/internal_commands.py` & `vastdb-0.1.6/vastdb/internal_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import logging
 import re
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
 from enum import Enum
-from ipaddress import IPv4Address, IPv6Address
 from typing import Any, Dict, Iterator, List, Optional, Union
 
 import flatbuffers
 import ibis
 import pyarrow as pa
 import pyarrow.parquet as pq
 import requests
@@ -1027,33 +1026,15 @@
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats", url_params=url_params), headers=headers)
         self._check_res(res, "get_table_stats", expected_retvals)
 
         stats = get_table_stats.GetRootAs(res.content)
         num_rows = stats.NumRows()
         size_in_bytes = stats.SizeInBytes()
         is_external_rowid_alloc = stats.IsExternalRowidAlloc()
-        endpoints = []
-        if stats.VipsLength() == 0:
-            endpoints.append(self.url)
-        else:
-            url = urllib3.util.parse_url(self.url)
-
-            ip_cls = IPv6Address if (stats.AddressType() == "ipv6") else IPv4Address
-            vips = [stats.Vips(i) for i in range(stats.VipsLength())]
-            ips = []
-            # extract the vips into list of IPs
-            for vip in vips:
-                start_ip = int(ip_cls(vip.StartAddress().decode()))
-                ips.extend(ip_cls(start_ip + i) for i in range(vip.AddressCount()))
-            # build a list of endpoint URLs, reusing schema and port (if specified when constructing the session).
-            # it is assumed that the client can access the returned IPs (e.g. if they are part of the VIP pool).
-            for ip in ips:
-                d = url._asdict()
-                d['host'] = str(ip)
-                endpoints.append(str(urllib3.util.Url(**d)))
+        endpoints = [self.url]  # we cannot replace the host by a VIP address in HTTPS-based URLs
         return TableStatsResult(num_rows, size_in_bytes, is_external_rowid_alloc, tuple(endpoints))
 
     def alter_table(self, bucket, schema, name, txid=0, client_tags=[], table_properties="",
                     new_name="", expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?table HTTP/1.1
         Content-Length: ContentLength
```

### Comparing `vastdb-0.1.5/vastdb/schema.py` & `vastdb-0.1.6/vastdb/transaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,89 @@
-"""VAST Database schema (a container of tables).
+"""VAST Database transaction.
 
-VAST S3 buckets can be used to create Database schemas and tables.
-It is possible to list and access VAST snapshots generated over a bucket.
+A transcation is used as a context manager, since every Database-related operation in VAST requires a transaction.
+
+    with session.transaction() as tx:
+        tx.bucket("bucket").create_schema("schema")
 """
 
 import logging
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, List, Optional
 
-import pyarrow as pa
+import botocore
 
-from . import bucket, errors, schema, table
+from . import bucket, errors, schema, session
 
 if TYPE_CHECKING:
-    from .table import Table
+    from bucket import Bucket
+    from table import Table
 
 
 log = logging.getLogger(__name__)
 
+VAST_CATALOG_BUCKET_NAME = "vast-big-catalog-bucket"
+VAST_CATALOG_SCHEMA_NAME = 'vast_big_catalog_schema'
+VAST_CATALOG_TABLE_NAME = 'vast_big_catalog_table'
+
+AUDIT_LOG_BUCKET_NAME = "vast-audit-log-bucket"
+AUDIT_LOG_SCHEMA_NAME = 'vast_audit_log_schema'
+AUDIT_LOG_TABLE_NAME = 'vast_audit_log_table'
+
 
 @dataclass
-class Schema:
-    """VAST Schema."""
+class Transaction:
+    """A holder of a single VAST transaction."""
 
-    name: str
-    bucket: "bucket.Bucket"
+    _rpc: "session.Session"
+    txid: Optional[int] = None
 
-    @property
-    def tx(self):
-        """VAST transaction used for this schema."""
-        return self.bucket.tx
-
-    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True) -> "Table":
-        """Create a new table under this schema."""
-        if current := self.table(table_name, fail_if_missing=False):
-            if fail_if_exists:
-                raise errors.TableExists(self.bucket.name, self.name, table_name)
-            else:
-                return current
-        self.tx._rpc.api.create_table(self.bucket.name, self.name, table_name, columns, txid=self.tx.txid)
-        log.info("Created table: %s", table_name)
-        return self.table(table_name)  # type: ignore[return-value]
-
-    def table(self, name: str, fail_if_missing=True) -> Optional["table.Table"]:
-        """Get a specific table under this schema."""
-        t = self.tables(table_name=name)
-        if not t:
-            if fail_if_missing:
-                raise errors.MissingTable(self.bucket.name, self.name, name)
-            else:
-                return None
-        assert len(t) == 1, f"Expected to receive only a single table, but got: {len(t)}. tables: {t}"
-        log.debug("Found table: %s", t[0])
-        return t[0]
-
-    def tables(self, table_name=None) -> List["Table"]:
-        """List all tables under this schema."""
-        tables = []
-        next_key = 0
-        name_prefix = table_name if table_name else ""
-        exact_match = bool(table_name)
-        while True:
-            _bucket_name, _schema_name, curr_tables, next_key, is_truncated, _ = \
-                self.tx._rpc.api.list_tables(
-                    bucket=self.bucket.name, schema=self.name, next_key=next_key, txid=self.tx.txid,
-                    exact_match=exact_match, name_prefix=name_prefix, include_list_stats=exact_match)
-            if not curr_tables:
-                break
-            tables.extend(curr_tables)
-            if not is_truncated:
-                break
-
-        return [_parse_table_info(table, self) for table in tables]
-
-    def drop(self) -> None:
-        """Delete this schema."""
-        self.tx._rpc.api.drop_schema(self.bucket.name, self.name, txid=self.tx.txid)
-        log.info("Dropped schema: %s", self.name)
-
-    def rename(self, new_name) -> None:
-        """Rename this schema."""
-        self.tx._rpc.api.alter_schema(self.bucket.name, self.name, txid=self.tx.txid, new_name=new_name)
-        log.info("Renamed schema: %s to %s", self.name, new_name)
-        self.name = new_name
-
-
-def _parse_table_info(table_info, schema: "schema.Schema"):
-    stats = table.TableStats(num_rows=table_info.num_rows, size_in_bytes=table_info.size_in_bytes)
-    return table.Table(name=table_info.name, schema=schema, handle=int(table_info.handle), stats=stats, _imports_table=False)
+    def __enter__(self):
+        """Create a transaction and store its ID."""
+        response = self._rpc.api.begin_transaction()
+        self.txid = int(response.headers['tabular-txid'])
+        log.debug("opened txid=%016x", self.txid)
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        """On success, the transaction is committed. Otherwise, it is rolled back."""
+        txid = self.txid
+        self.txid = None
+        if (exc_type, exc_value, exc_traceback) == (None, None, None):
+            log.debug("committing txid=%016x", txid)
+            self._rpc.api.commit_transaction(txid)
+        else:
+            log.exception("rolling back txid=%016x due to:", txid)
+            self._rpc.api.rollback_transaction(txid)
+
+    def __repr__(self):
+        """Don't show the session details."""
+        if self.txid is None:
+            return 'InvalidTransaction'
+        return f'Transaction(id=0x{self.txid:016x})'
+
+    def bucket(self, name: str) -> "Bucket":
+        """Return a VAST Bucket, if exists."""
+        try:
+            self._rpc.s3.head_bucket(Bucket=name)
+        except botocore.exceptions.ClientError as e:
+            log.warning("res: %s", e.response)
+            if e.response['Error']['Code'] == '404':
+                raise errors.MissingBucket(name) from e
+            raise
+        return bucket.Bucket(name, self)
+
+    def catalog_snapshots(self) -> List["Bucket"]:
+        """Return VAST Catalog bucket snapshots."""
+        return bucket.Bucket(VAST_CATALOG_BUCKET_NAME, self).snapshots()
+
+    def catalog(self, snapshot: Optional["Bucket"] = None, fail_if_missing=True) -> Optional["Table"]:
+        """Return VAST Catalog table."""
+        b = snapshot or bucket.Bucket(VAST_CATALOG_BUCKET_NAME, self)
+        s = schema.Schema(VAST_CATALOG_SCHEMA_NAME, b)
+        return s.table(name=VAST_CATALOG_TABLE_NAME, fail_if_missing=fail_if_missing)
+
+    def audit_log(self, fail_if_missing=True) -> Optional["Table"]:
+        """Return VAST Audit Log table."""
+        b = bucket.Bucket(AUDIT_LOG_BUCKET_NAME, self)
+        s = schema.Schema(AUDIT_LOG_SCHEMA_NAME, b)
+        return s.table(name=AUDIT_LOG_TABLE_NAME, fail_if_missing=fail_if_missing)
```

### Comparing `vastdb-0.1.5/vastdb/session.py` & `vastdb-0.1.6/vastdb/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,53 @@
 It should be used to interact with a specific VAST cluster.
 For more details see:
 - [Virtual IP pool configured with DNS service](https://support.vastdata.com/s/topic/0TOV40000000FThOAM/configuring-network-access-v50)
 - [S3 access & secret keys on VAST cluster](https://support.vastdata.com/s/article/UUID-4d2e7e23-b2fb-7900-d98f-96c31a499626)
 - [Tabular identity policy with the proper permissions](https://support.vastdata.com/s/article/UUID-14322b60-d6a2-89ac-3df0-3dfbb6974182)
 """
 
+import logging
 import os
 
 import boto3
 
 from . import errors, internal_commands, transaction
 
+log = logging.getLogger()
+
 
 class Features:
     """VAST database features - check if server is already support a feature."""
 
     def __init__(self, vast_version):
         """Save the server version."""
         self.vast_version = vast_version
 
-    def check_imports_table(self):
-        """Check if the feature that support imports table is supported."""
-        if self.vast_version < (5, 2):
-            raise errors.NotSupportedVersion("import_table requires 5.2+", self.vast_version)
-
-    def check_return_row_ids(self):
-        """Check if insert/update/delete can return the row_ids."""
-        if self.vast_version < (5, 1):
-            raise errors.NotSupportedVersion("return_row_ids requires 5.1+", self.vast_version)
+        self.check_imports_table = self._check(
+            "Imported objects' table feature requires 5.2+ VAST release",
+            vast_version >= (5, 2))
+
+        self.check_return_row_ids = self._check(
+            "Returning row IDs requires 5.1+ VAST release",
+            vast_version >= (5, 1))
+
+        self.check_enforce_semisorted_projection = self._check(
+            "Semi-sorted projection enforcement requires 5.1+ VAST release",
+            vast_version >= (5, 1))
+
+    def _check(self, msg, supported):
+        log.debug("%s (current version is %s): supported=%s", msg, self.vast_version, supported)
+        if not supported:
+            def fail():
+                raise errors.NotSupportedVersion(msg, self.vast_version)
+            return fail
+
+        def noop():
+            pass
+        return noop
 
 
 class Session:
     """VAST database session."""
 
     def __init__(self, access=None, secret=None, endpoint=None, ssl_verify=True):
         """Connect to a VAST Database endpoint, using specified credentials."""
```

### Comparing `vastdb-0.1.5/vastdb/table.py` & `vastdb-0.1.6/vastdb/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,34 @@
 class QueryConfig:
     """Query execution configiration."""
 
     # allows server-side parallel processing by issuing multiple reads concurrently for a single RPC
     num_sub_splits: int = 4
 
     # used to split the table into disjoint subsets of rows, to be processed concurrently using multiple RPCs
-    num_splits: int = 1
+    # will be estimated from the table's row count, if not explicitly set
+    num_splits: Optional[int] = None
 
     # each endpoint will be handled by a separate worker thread
     # a single endpoint can be specified more than once to benefit from multithreaded execution
     data_endpoints: Optional[List[str]] = None
 
     # a subsplit fiber will finish after sending this number of rows back to the client
     limit_rows_per_sub_split: int = 128 * 1024
 
     # each fiber will read the following number of rowgroups coninuously before skipping
-    # in order to use semi-sorted projections this value must be 8
+    # in order to use semi-sorted projections this value must be 8 (this is the hard coded size of a row groups per row block).
     num_row_groups_per_sub_split: int = 8
 
     # can be disabled for benchmarking purposes
     use_semi_sorted_projections: bool = True
 
+    # enforce using a specific semi-sorted projection (if enabled above)
+    semi_sorted_projection_name: Optional[str] = None
+
     # used to estimate the number of splits, given the table rows' count
     rows_per_split: int = 4000000
 
     # used for worker threads' naming
     query_id: str = ""
 
     # allows retrying QueryData when the server is overloaded
@@ -113,15 +117,16 @@
                             split=(self.split_id, self.config.num_splits, self.config.num_row_groups_per_sub_split),
                             num_sub_splits=self.config.num_sub_splits,
                             response_row_id=False,
                             txid=self.table.tx.txid,
                             limit_rows=self.config.limit_rows_per_sub_split,
                             sub_split_start_row_ids=self.subsplits_state.items(),
                             enable_sorted_projections=self.config.use_semi_sorted_projections,
-                            query_imports_table=self.table._imports_table)
+                            query_imports_table=self.table._imports_table,
+                            projection=self.config.semi_sorted_projection_name)
             pages_iter = internal_commands.parse_query_data_response(
                 conn=response.raw,
                 schema=self.query_data_request.response_schema,
                 start_row_ids=self.subsplits_state,
                 parser=self.query_data_request.response_parser)
 
             for page in pages_iter:
@@ -309,19 +314,24 @@
         Query-execution configuration options can be specified via the optional `config` argument.
         """
         if config is None:
             config = QueryConfig()
 
         # Take a snapshot of enpoints
         stats = self.get_stats()
+        log.debug("stats: %s", stats)
         endpoints = stats.endpoints if config.data_endpoints is None else config.data_endpoints
+        log.debug("endpoints: %s", endpoints)
+
+        if config.num_splits is None:
+            config.num_splits = max(1, stats.num_rows // config.rows_per_split)
+        log.debug("config: %s", config)
 
-        if stats.num_rows > config.rows_per_split and config.num_splits is None:
-            config.num_splits = stats.num_rows // config.rows_per_split
-        log.debug(f"num_rows={stats.num_rows} rows_per_splits={config.rows_per_split} num_splits={config.num_splits} ")
+        if config.semi_sorted_projection_name:
+            self.tx._rpc.features.check_enforce_semisorted_projection()
 
         if columns is None:
             columns = [f.name for f in self.arrow_schema]
 
         query_schema = self.arrow_schema
         if internal_row_id:
             queried_fields = [INTERNAL_ROW_ID_FIELD]
@@ -338,14 +348,16 @@
         if isinstance(predicate, ibis.common.deferred.Deferred):
             predicate = predicate.resolve(self._ibis_table)  # may raise if the predicate is invalid (e.g. wrong types / missing column)
 
         query_data_request = internal_commands.build_query_data_request(
             schema=query_schema,
             predicate=predicate,
             field_names=columns)
+        if len(query_data_request.serialized) > util.MAX_QUERY_DATA_REQUEST_SIZE:
+            raise errors.TooLargeRequest(f"{len(query_data_request.serialized)} bytes")
 
         splits_queue: queue.Queue[int] = queue.Queue()
 
         for split in range(config.num_splits):
             splits_queue.put(split)
 
         # this queue shouldn't be large it is marely a pipe through which the results
```

### Comparing `vastdb-0.1.5/vastdb/tests/test_duckdb.py` & `vastdb-0.1.6/vastdb/tests/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vastdb/tests/test_imports.py` & `vastdb-0.1.6/vastdb/tests/test_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,21 +34,21 @@
         b = tx.bucket(clean_bucket_name)
         s = b.create_schema('s1')
         t = s.create_table('t1', pa.schema([('num', pa.int64())]))
         with pytest.raises(InternalServerError):
             t.create_imports_table()
         log.info("Starting import of %d files", num_files)
         t.import_files(files)
-        arrow_table = pa.Table.from_batches(t.select(columns=['num']))
+        arrow_table = t.select(columns=['num']).read_all()
         assert arrow_table.num_rows == num_rows * num_files
-        arrow_table = pa.Table.from_batches(t.select(columns=['num'], predicate=t['num'] == 100))
+        arrow_table = t.select(columns=['num'], predicate=t['num'] == 100).read_all()
         assert arrow_table.num_rows == num_files
         import_table = t.imports_table()
         # checking all imports are on the imports table:
-        objects_name = pa.Table.from_batches(import_table.select(columns=["ObjectName"]))
+        objects_name = import_table.select(columns=["ObjectName"]).read_all()
         objects_name = objects_name.to_pydict()
         object_names = set(objects_name['ObjectName'])
         prefix = 'prq'
         numbers = set(range(53))
         assert all(name.startswith(prefix) for name in object_names)
         numbers.issubset(int(name.replace(prefix, '')) for name in object_names)
         assert len(object_names) == len(objects_name['ObjectName'])
```

### Comparing `vastdb-0.1.5/vastdb/tests/test_nested.py` & `vastdb-0.1.6/vastdb/tests/test_nested.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     expected = pa.table(schema=columns, data=[
         [[1], [], [2, 3], None],
         [None, {'a': 2.5}, {'b': 0.25, 'c': 0.025}, {}],
         [{'x': 1, 'y': None}, None, {'x': 2, 'y': 3}, {'x': None, 'y': 4}],
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
-        actual = pa.Table.from_batches(t.select())
+        actual = t.select().read_all()
         assert actual == expected
 
         names = [f.name for f in columns]
         for n in range(len(names) + 1):
             for cols in itertools.permutations(names, n):
-                actual = pa.Table.from_batches(t.select(columns=cols))
+                actual = t.select(columns=cols).read_all()
                 assert actual == expected.select(cols)
 
 
 def test_nested_filter(session, clean_bucket_name):
     columns = pa.schema([
         ('x', pa.int64()),
         ('l', pa.list_(pa.int8())),
@@ -49,24 +49,24 @@
         [None, {'a': 2.5}, {'b': 0.25, 'c': 0.025}, {}],
         [1, None, 2, 3],
         [{'x': 1, 'y': None}, None, {'x': 2, 'y': 3}, {'x': None, 'y': 4}],
         [None, 1, 2, 3],
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
-        actual = pa.Table.from_batches(t.select())
+        actual = t.select().read_all()
         assert actual == expected
 
         names = list('xyzw')
         for n in range(1, len(names) + 1):
             for cols in itertools.permutations(names, n):
                 ibis_predicate = functools.reduce(
                     operator.and_,
                     (t[col] > 2 for col in cols))
-                actual = pa.Table.from_batches(t.select(predicate=ibis_predicate), t.arrow_schema)
+                actual = t.select(predicate=ibis_predicate).read_all()
 
                 arrow_predicate = functools.reduce(
                     operator.and_,
                     (pc.field(col) > 2 for col in cols))
                 assert actual == expected.filter(arrow_predicate)
```

### Comparing `vastdb-0.1.5/vastdb/tests/test_sanity.py` & `vastdb-0.1.6/vastdb/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vastdb/tests/test_tables.py` & `vastdb-0.1.6/vastdb/tests/test_tables.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime as dt
 import decimal
 import logging
 import random
 import threading
-import time
 from contextlib import closing
 from tempfile import NamedTemporaryFile
 
 import ibis
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.parquet as pq
@@ -29,60 +28,60 @@
     ])
     expected = pa.table(schema=columns, data=[
         [111, 222, 333],
         [0.5, 1.5, 2.5],
         ['a', 'bb', 'ccc'],
     ])
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b', 's']))
+        actual = t.select(columns=['a', 'b', 's']).read_all()
         assert actual == expected
 
-        actual = pa.Table.from_batches(t.select())
+        actual = t.select().read_all()
         assert actual == expected
 
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b']))
+        actual = t.select(columns=['a', 'b']).read_all()
         assert actual == expected.select(['a', 'b'])
 
-        actual = pa.Table.from_batches(t.select(columns=['b', 's', 'a']))
+        actual = t.select(columns=['b', 's', 'a']).read_all()
         assert actual == expected.select(['b', 's', 'a'])
 
-        actual = pa.Table.from_batches(t.select(columns=['s']))
+        actual = t.select(columns=['s']).read_all()
         assert actual == expected.select(['s'])
 
-        actual = pa.Table.from_batches(t.select(columns=[]))
+        actual = t.select(columns=[]).read_all()
         assert actual == expected.select([])
 
-        actual = pa.Table.from_batches(t.select(columns=['s'], internal_row_id=True))
+        actual = t.select(columns=['s'], internal_row_id=True).read_all()
         log.debug("actual=%s", actual)
         assert actual.to_pydict() == {
             's': ['a', 'bb', 'ccc'],
             INTERNAL_ROW_ID: [0, 1, 2]
         }
 
         columns_to_delete = pa.schema([(INTERNAL_ROW_ID, pa.uint64())])
         rb = pa.record_batch(schema=columns_to_delete, data=[[0]])  # delete rows 0,1
         t.delete(rb)
 
-        selected_rows = pa.Table.from_batches(t.select(columns=['b'], predicate=(t['a'] == 222), internal_row_id=True))
+        selected_rows = t.select(columns=['b'], predicate=(t['a'] == 222), internal_row_id=True).read_all()
         t.delete(selected_rows)
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b', 's']))
+        actual = t.select(columns=['a', 'b', 's']).read_all()
         assert actual.to_pydict() == {
             'a': [333],
             'b': [2.5],
             's': ['ccc']
         }
 
 
 def test_insert_wide_row(session, clean_bucket_name):
     columns = pa.schema([pa.field(f's{i}', pa.utf8()) for i in range(500)])
     data = [['a' * 10**4] for i in range(500)]
     expected = pa.table(schema=columns, data=data)
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
-        actual = pa.Table.from_batches(t.select())
+        actual = t.select().read_all()
         assert actual == expected
 
 
 def test_exists(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         assert s.tables() == []
@@ -121,41 +120,41 @@
 
         rb = pa.record_batch(schema=columns_to_update, data=[
             [0, 2],  # update rows 0,2
             [1110, 3330]
         ])
 
         t.update(rb)
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b']))
+        actual = t.select(columns=['a', 'b']).read_all()
         assert actual.to_pydict() == {
             'a': [1110, 222, 3330],
             'b': [0.5, 1.5, 2.5]
         }
 
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b'], predicate=(t['a'] < 1000), internal_row_id=True))
+        actual = t.select(columns=['a', 'b'], predicate=(t['a'] < 1000), internal_row_id=True).read_all()
         column_index = actual.column_names.index('a')
         column_field = actual.field(column_index)
         new_data = pc.add(actual.column('a'), 2000)
         update_table = actual.set_column(column_index, column_field, new_data)
 
         t.update(update_table, columns=['a'])
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b']))
+        actual = t.select(columns=['a', 'b']).read_all()
         assert actual.to_pydict() == {
             'a': [1110, 2222, 3330],
             'b': [0.5, 1.5, 2.5]
         }
 
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b'], predicate=(t['a'] != 2222), internal_row_id=True))
+        actual = t.select(columns=['a', 'b'], predicate=(t['a'] != 2222), internal_row_id=True).read_all()
         column_index = actual.column_names.index('a')
         column_field = actual.field(column_index)
         new_data = pc.divide(actual.column('a'), 10)
         update_table = actual.set_column(column_index, column_field, new_data)
 
         t.update(update_table.to_batches()[0], columns=['a'])
-        actual = pa.Table.from_batches(t.select(columns=['a', 'b']))
+        actual = t.select(columns=['a', 'b']).read_all()
         assert actual.to_pydict() == {
             'a': [111, 2222, 333],
             'b': [0.5, 1.5, 2.5]
         }
 
 
 def test_select_with_multisplits(session, clean_bucket_name):
@@ -167,15 +166,15 @@
     data = data * 1000
     expected = pa.table(schema=columns, data=[data])
 
     config = QueryConfig()
     config.rows_per_split = 1000
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
-        actual = pa.Table.from_batches(t.select(columns=['a'], config=config))
+        actual = t.select(columns=['a'], config=config).read_all()
         assert actual == expected
 
 
 def test_types(session, clean_bucket_name):
     columns = pa.schema([
         ('tb', pa.bool_()),
         ('a1', pa.int8()),
@@ -214,15 +213,15 @@
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789000), dt.datetime(2025, 4, 10, 12, 34, 56, 789000), dt.datetime(2026, 4, 10, 12, 34, 56, 789000)],
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as table:
         def select(predicate):
-            return pa.Table.from_batches(table.select(predicate=predicate))
+            return table.select(predicate=predicate).read_all()
 
         assert select(None) == expected
         for t in [table, ibis._]:
             assert select(t['tb'] == False) == expected.filter(pc.field('tb') == False)  # noqa: E712
             assert select(t['a1'] == 2) == expected.filter(pc.field('a1') == 2)
             assert select(t['a2'] == 2000) == expected.filter(pc.field('a2') == 2000)
             assert select(t['a4'] == 222111122) == expected.filter(pc.field('a4') == 222111122)
@@ -270,21 +269,28 @@
         [111, 222, 333, 444, 555],
         [0.5, 1.5, 2.5, 3.5, 4.5],
         ['a', 'bb', 'ccc', None, 'xyz'],
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as table:
         def select(predicate):
-            return pa.Table.from_batches(table.select(predicate=predicate), table.arrow_schema)
+            return table.select(predicate=predicate).read_all()
 
         assert select(None) == expected
         assert select(True) == expected
         assert select(False) == pa.Table.from_batches([], schema=columns)
 
         for t in [table, ibis._]:
+
+            select(t['a'].isin(list(range(100))))
+            select(t['a'].isin(list(range(1000))))
+            select(t['a'].isin(list(range(10000))))
+            with pytest.raises(errors.TooLargeRequest):
+                select(t['a'].isin(list(range(100000))))
+
             assert select(t['a'].between(222, 444)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444))
             assert select((t['a'].between(222, 444)) & (t['b'] > 2.5)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444) & (pc.field('b') > 2.5))
 
             assert select(t['a'] > 222) == expected.filter(pc.field('a') > 222)
             assert select(t['a'] < 222) == expected.filter(pc.field('a') < 222)
             assert select(t['a'] == 222) == expected.filter(pc.field('a') == 222)
             assert select(t['a'] != 222) == expected.filter(pc.field('a') != 222)
@@ -347,15 +353,15 @@
             [111, 222],
             [0.5, 1.5],
             ['a', 'b'],
         ])
         expected = pa.Table.from_batches([rb])
         rb = t.insert(rb)
         assert rb.to_pylist() == [0, 1]
-        actual = pa.Table.from_batches(t.select())
+        actual = t.select().read_all()
         assert actual == expected
 
         table_batches = t.select()
 
         with NamedTemporaryFile() as parquet_file:
             log.info("Writing table into parquet file: '%s'", parquet_file.name)
             with closing(pq.ParquetWriter(parquet_file.name, table_batches.schema)) as parquet_writer:
@@ -663,22 +669,41 @@
     # Check that all threads were killed
     log.info("Active threads: %d", active_threads())
 
     # validate that all query threads were killed.
     assert active_threads() == 0
 
 
-def test_big_catalog_select(session, clean_bucket_name):
+def test_catalog_select(session, clean_bucket_name):
     with session.transaction() as tx:
         bc = tx.catalog()
-        actual = pa.Table.from_batches(bc.select(['name']))
-        assert actual
-        log.info("actual=%s", actual)
+        assert bc.columns()
+        rows = bc.select(['name']).read_all()
+        assert len(rows) > 0, rows
+
+
+class NotReady(Exception):
+    pass
 
 
+@pytest.mark.flaky(retries=30, delay=1, only_on=[NotReady])
 def test_audit_log_select(session, clean_bucket_name):
     with session.transaction() as tx:
         a = tx.audit_log()
-        a.columns()
-        time.sleep(1)
-        actual = pa.Table.from_batches(a.select(), a.arrow_schema)
-        log.info("actual=%s", actual)
+        assert a.columns()
+        rows = a.select().read_all()
+        if len(rows) == 0:
+            raise NotReady
+
+
+@pytest.mark.flaky(retries=30, delay=1, only_on=[NotReady])
+def test_catalog_snapshots_select(session, clean_bucket_name):
+    with session.transaction() as tx:
+        snaps = tx.catalog_snapshots()
+        if not snaps:
+            raise NotReady
+        latest = snaps[-1]
+        t = tx.catalog(latest)
+        assert t.columns()
+        rows = t.select().read_all()
+        if not rows:
+            raise NotReady
```

### Comparing `vastdb-0.1.5/vastdb/tests/test_util.py` & `vastdb-0.1.6/vastdb/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vastdb/tests/util.py` & `vastdb-0.1.6/vastdb/tests/util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.5/vastdb/util.py` & `vastdb-0.1.6/vastdb/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     This function returns a unified schema from potentially two different schemas.
     """
     return pa.unify_schemas([current_schema, new_schema])
 
 
 MAX_TABULAR_REQUEST_SIZE = 5 << 20  # in bytes
 MAX_RECORD_BATCH_SLICE_SIZE = int(0.9 * MAX_TABULAR_REQUEST_SIZE)
+MAX_QUERY_DATA_REQUEST_SIZE = int(0.9 * MAX_TABULAR_REQUEST_SIZE)
 
 
 def iter_serialized_slices(batch: Union[pa.RecordBatch, pa.Table], max_rows_per_slice=None):
     """Iterate over a list of record batch slices."""
 
     rows_per_slice = int(0.9 * len(batch) * MAX_RECORD_BATCH_SLICE_SIZE / batch.nbytes)
     if max_rows_per_slice is not None:
```

### Comparing `vastdb-0.1.5/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.6/vastdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.5
+Version: 0.1.6
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vastdb-0.1.5/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.6/vastdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

