# Comparing `tmp/vastdb-0.1.1.tar.gz` & `tmp/vastdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.1.tar", last modified: Tue Apr 16 14:52:46 2024, max compression
+gzip compressed data, was "vastdb-0.1.2.tar", last modified: Thu Apr 25 14:57:33 2024, max compression
```

## Comparing `vastdb-0.1.1.tar` & `vastdb-0.1.2.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.980522 vastdb-0.1.1/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3026 2024-04-16 08:04:31.000000 vastdb-0.1.1/CHANGELOG.md
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    11333 2023-12-17 10:00:47.000000 vastdb-0.1.1/LICENSE
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-14 12:15:26.000000 vastdb-0.1.1/MANIFEST.in
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-16 14:52:46.980368 vastdb-0.1.1/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5891 2024-04-13 15:33:57.000000 vastdb-0.1.1/README.md
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-12 16:51:13.000000 vastdb-0.1.1/requirements.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-16 14:52:46.980587 vastdb-0.1.1/setup.cfg
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1700 2024-04-16 08:04:31.000000 vastdb-0.1.1/setup.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939438 vastdb-0.1.1/vast_flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939565 vastdb-0.1.1/vast_flatbuf/org/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939701 vastdb-0.1.1/vast_flatbuf/org/apache/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939831 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939959 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.956086 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5630 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2212 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1567 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2494 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      182 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4434 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2429 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2520 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      236 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3490 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1059 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2576 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      484 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2258 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      498 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1584 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2850 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3260 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2602 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1515 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      186 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2403 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1487 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2197 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      211 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1578 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4455 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      230 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2309 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3368 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2400 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2797 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      682 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3284 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1723 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2392 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3847 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      349 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2378 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3941 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1526 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2113 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      315 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      217 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3678 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3952 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2221 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5650 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1533 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1593 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2539 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1529 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1051 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7527 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.968767 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1026 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1326 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2310 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      836 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1430 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      155 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1760 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      149 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2855 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3148 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4091 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      410 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      267 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1289 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7048 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1669 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1569 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1541 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6448 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1925 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      180 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1131 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2541 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4486 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      671 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      786 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1054 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      161 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6042 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      162 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5785 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6091 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      226 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6389 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     9409 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1193 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5767 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2149 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2639 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      191 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7925 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      698 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3142 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      147 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1023 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.973477 vastdb-0.1.1/vast_flatbuf/tabular/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2114 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2222 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1618 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1610 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1901 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/Column.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      151 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ColumnType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2516 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1626 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3474 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4655 2024-04-11 20:45:30.000000 vastdb-0.1.1/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2450 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ImportDataRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4240 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3036 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3550 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListTablesResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ObjectDetails.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4450 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/S3File.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2069 2024-04-11 20:45:30.000000 vastdb-0.1.1/vast_flatbuf/tabular/VipRange.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.976905 vastdb-0.1.1/vastdb/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      206 2024-04-13 15:16:53.000000 vastdb-0.1.1/vastdb/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.978057 vastdb-0.1.1/vastdb/bench/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-13 15:33:57.000000 vastdb-0.1.1/vastdb/bench/__init__.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1111 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/bench/test_perf.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2854 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/bucket.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2132 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/conftest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3315 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/errors.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)   101564 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/internal_commands.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3192 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/schema.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1718 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/session.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    20443 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/table.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.980129 vastdb-0.1.1/vastdb/tests/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-14 19:07:27.000000 vastdb-0.1.1/vastdb/tests/__init__.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5033 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_imports.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      951 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_nested.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1254 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_projections.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2958 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_sanity.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1721 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/tests/test_schemas.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    26226 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/tests/test_tables.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      597 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/util.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1796 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/transaction.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2974 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/util.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.977787 vastdb-0.1.1/vastdb.egg-info/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     8994 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        1 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/requires.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       20 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.703902 vastdb-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2024-04-25 14:01:45.000000 vastdb-0.1.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-04-25 14:01:45.000000 vastdb-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-25 14:01:45.000000 vastdb-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-25 14:57:33.703902 vastdb-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2024-04-25 14:01:45.000000 vastdb-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-25 14:01:45.000000 vastdb-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:57:33.703902 vastdb-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2024-04-25 14:01:45.000000 vastdb-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.684903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.695903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.698902 vastdb-0.1.2/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.700903 vastdb-0.1.2/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.701902 vastdb-0.1.2/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)   101273 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/internal_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    20532 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.702902 vastdb-0.1.2/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    25667 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3022 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.702902 vastdb-0.1.2/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9022 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.1/CHANGELOG.md` & `vastdb-0.1.2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.2] (2024-04-25)
+[0.1.2]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.1...v0.1.2
+
+### Added
+ - Allow querying [VAST Catalog](https://www.vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database)
+ - Use [mypy](https://mypy-lang.org/) for type annotation checking
+
+### Fixed
+ - Fix handling HTTPS endpoints [#50]
+ - Optimize `Table.select()` performance
+ - Use `GET` request to retrieve cluster version
+ - Enable `ruff` preview mode
+ - Make sure DuckDB integration fails gracefully when transaction is closed prematurely
+
+### Removed
+ - Don't return row IDs from `Table.insert()`
+
 ## [0.1.1] (2024-04-15)
 [0.1.1]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.0...v0.1.1
 
 ### Added
  - Support date & timestamp predicate pushdown [#25]
 
 ### Fixed
@@ -89,7 +106,8 @@
 [#29]: https://github.com/vast-data/vastdb_sdk/pull/29
 [#30]: https://github.com/vast-data/vastdb_sdk/pull/30
 [#31]: https://github.com/vast-data/vastdb_sdk/pull/31
 [#33]: https://github.com/vast-data/vastdb_sdk/pull/33
 [#42]: https://github.com/vast-data/vastdb_sdk/pull/42
 [#43]: https://github.com/vast-data/vastdb_sdk/pull/43
 [#47]: https://github.com/vast-data/vastdb_sdk/pull/47
+[#50]: https://github.com/vast-data/vastdb_sdk/pull/50
```

### Comparing `vastdb-0.1.1/LICENSE` & `vastdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/README.md` & `vastdb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/setup.py` & `vastdb-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 with [VAST Database](https://vastdata.com/database)
 and [VAST Catalog](https://vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database),
 enabling schema and table management, efficient ingest, query and modification of columnar data.
 
 For more details, see [our whitepaper](https://vastdata.com/whitepaper/#TheVASTDataBase).
 """
 
+
 def _get_version_suffix():
     import subprocess
 
     commit = subprocess.check_output(["git", "rev-parse", "HEAD"])
     print(f"Git commit: {commit}")
     return f".dev1+vast.{commit.decode()[:16]}"
 
+
 suffix = ''
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.1' + suffix,
+    version='0.1.2' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().strip().split('\n'),
     long_description=long_description,
```

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.2/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.2/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.2/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.2/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.2/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.2/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.2/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.2/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.2/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.2/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vastdb/bench/test_perf.py` & `vastdb-0.1.2/vastdb/bench/test_perf.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from vastdb.table import ImportConfig, QueryConfig
 
 log = logging.getLogger(__name__)
 
 
 @pytest.mark.benchmark
 def test_bench(session, clean_bucket_name, parquets_path, crater_path):
-    files = [str(parquets_path/f) for f in (parquets_path.glob('**/*.pq'))]
+    files = [str(parquets_path / f) for f in (parquets_path.glob('**/*.pq'))]
 
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         s = b.create_schema('s1')
         t = util.create_table_from_files(s, 't1', files, config=ImportConfig(import_concurrency=8))
         config = QueryConfig(num_splits=8, num_sub_splits=4)
         s = time.time()
         pa_table = pa.Table.from_batches(t.select(columns=['sid'], predicate=t['sid'] == 10033007, config=config))
         e = time.time()
-        log.info("'SELECT sid from TABLE WHERE sid = 10033007' returned in %s seconds.", e-s)
+        log.info("'SELECT sid from TABLE WHERE sid = 10033007' returned in %s seconds.", e - s)
         if crater_path:
             with open(f'{crater_path}/bench_results', 'a') as f:
-                f.write(f"'SELECT sid FROM TABLE WHERE sid = 10033007' returned in {e-s} seconds")
+                f.write(f"'SELECT sid FROM TABLE WHERE sid = 10033007' returned in {e - s} seconds")
         assert pa_table.num_rows == 255_075
```

### Comparing `vastdb-0.1.1/vastdb/bucket.py` & `vastdb-0.1.2/vastdb/bucket.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING, List, Optional
 
 from . import errors, schema, transaction
 
+if TYPE_CHECKING:
+    from .schema import Schema
+
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Snapshot:
     """VAST bucket-level snapshot."""
 
@@ -23,57 +27,57 @@
 @dataclass
 class Bucket:
     """VAST bucket."""
 
     name: str
     tx: "transaction.Transaction"
 
-    def create_schema(self, path: str, fail_if_exists=True) -> "schema.Schema":
+    def create_schema(self, path: str, fail_if_exists=True) -> "Schema":
         """Create a new schema (a container of tables) under this bucket."""
         if current := self.schema(path, fail_if_missing=False):
             if fail_if_exists:
                 raise errors.SchemaExists(self.name, path)
             else:
                 return current
         self.tx._rpc.api.create_schema(self.name, path, txid=self.tx.txid)
         log.info("Created schema: %s", path)
-        return self.schema(path)
+        return self.schema(path)  # type: ignore[return-value]
 
-    def schema(self, path: str, fail_if_missing=True) -> "schema.Schema":
+    def schema(self, path: str, fail_if_missing=True) -> Optional["Schema"]:
         """Get a specific schema (a container of tables) under this bucket."""
         s = self.schemas(path)
         log.debug("schema: %s", s)
         if not s:
             if fail_if_missing:
                 raise errors.MissingSchema(self.name, path)
             else:
                 return None
         assert len(s) == 1, f"Expected to receive only a single schema, but got: {len(s)}. ({s})"
         log.debug("Found schema: %s", s[0].name)
         return s[0]
 
-    def schemas(self, name: str = None) -> ["schema.Schema"]:
+    def schemas(self, name: Optional[str] = None) -> List["Schema"]:
         """List bucket's schemas."""
         schemas = []
         next_key = 0
         exact_match = bool(name)
         log.debug("list schemas param: schema=%s, exact_match=%s", name, exact_match)
         while True:
-            bucket_name, curr_schemas, next_key, is_truncated, _ = \
+            _bucket_name, curr_schemas, next_key, is_truncated, _ = \
                 self.tx._rpc.api.list_schemas(bucket=self.name, next_key=next_key, txid=self.tx.txid,
                                                name_prefix=name, exact_match=exact_match)
             if not curr_schemas:
                 break
             schemas.extend(curr_schemas)
             if not is_truncated:
                 break
 
         return [schema.Schema(name=name, bucket=self) for name, *_ in schemas]
 
-    def snapshots(self) -> [Snapshot]:
+    def snapshots(self) -> List[Snapshot]:
         """List bucket's snapshots."""
         snapshots = []
         next_key = 0
         while True:
             curr_snapshots, is_truncated, next_key = \
                 self.tx._rpc.api.list_snapshots(bucket=self.name, next_token=next_key)
             if not curr_snapshots:
```

### Comparing `vastdb-0.1.1/vastdb/conftest.py` & `vastdb-0.1.2/vastdb/conftest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vastdb/errors.py` & `vastdb-0.1.2/vastdb/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class HttpError(Exception):
     code: str
     message: str
+    method: str
     url: str
     status: int  # HTTP status
     headers: requests.structures.CaseInsensitiveDict  # HTTP response headers
 
     def __post_init__(self):
         self.args = [vars(self)]
 
@@ -84,14 +85,18 @@
     pass
 
 
 class Missing(Exception):
     pass
 
 
+class MissingTransaction(Missing):
+    pass
+
+
 @dataclass
 class MissingBucket(Missing):
     bucket: str
 
 
 @dataclass
 class MissingSchema(Missing):
@@ -146,29 +151,30 @@
 
 def from_response(res: requests.Response):
     if res.status_code == HttpStatus.SUCCESS.value:
         return None
 
     log.debug("response: url='%s', code=%s, headers=%s, body='%s'", res.request.url, res.status_code, res.headers, res.text)
     # try to parse S3 XML response for the error details:
-    code = None
-    message = None
+    code_str = None
+    message_str = None
     if res.text:
         try:
             root = xml.etree.ElementTree.fromstring(res.text)
             code = root.find('Code')
-            code = code.text if code is not None else None
+            code_str = code.text if code is not None else None
             message = root.find('Message')
-            message = message.text if message is not None else None
+            message_str = message.text if message is not None else None
         except xml.etree.ElementTree.ParseError:
             log.debug("invalid XML: %r", res.text)
 
     kwargs = dict(
-        code=code,
-        message=message,
+        code=code_str,
+        message=message_str,
+        method=res.request.method,
         url=res.request.url,
         status=res.status_code,
         headers=res.headers,
     )
     log.warning("RPC failed: %s", kwargs)
     status = HttpStatus(res.status_code)
     error_type = ERROR_TYPES_MAP.get(status, UnexpectedError)
```

### Comparing `vastdb-0.1.1/vastdb/internal_commands.py` & `vastdb-0.1.2/vastdb/internal_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 import re
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
-from typing import Iterator, Optional, Union
+from typing import Any, Dict, Iterator, List, Optional, Union
 
 import flatbuffers
 import ibis
 import pyarrow as pa
 import pyarrow.parquet as pq
 import requests
 import urllib3
@@ -88,15 +88,15 @@
 from . import errors
 
 UINT64_MAX = 18446744073709551615
 
 TABULAR_KEEP_ALIVE_STREAM_ID = 0xFFFFFFFF
 TABULAR_QUERY_DATA_COMPLETED_STREAM_ID = 0xFFFFFFFF - 1
 TABULAR_QUERY_DATA_FAILED_STREAM_ID = 0xFFFFFFFF - 2
-TABULAR_INVALID_ROW_ID = 0xFFFFFFFFFFFF # (1<<48)-1
+TABULAR_INVALID_ROW_ID = 0xFFFFFFFFFFFF  # (1<<48)-1
 ESTORE_INVALID_EHANDLE = UINT64_MAX
 IMPORTED_OBJECTS_TABLE_NAME = "vastdb-imported-objects"
 
 """
 S3 Tabular API
 """
 
@@ -123,19 +123,19 @@
         'ns': TimeUnit.NANOSECOND,
         'us': TimeUnit.MICROSECOND,
         'ms': TimeUnit.MILLISECOND,
         's': TimeUnit.SECOND
     }
     return unit_to_flatbuff_time_unit[type]
 
+
 class Predicate:
     def __init__(self, schema: 'pa.Schema', expr: ibis.expr.types.BooleanColumn):
         self.schema = schema
         self.expr = expr
-        self.builder = None
 
     def get_field_indexes(self, field: 'pa.Field', field_name_per_index: list) -> None:
         field_name_per_index.append(field.name)
 
         if isinstance(field.type, pa.StructType):
             flat_fields = field.flatten()
         elif isinstance(field.type, pa.MapType):
@@ -153,30 +153,34 @@
         if self._field_name_per_index is None:
             _field_name_per_index = []
             for field in self.schema:
                 self.get_field_indexes(field, _field_name_per_index)
             self._field_name_per_index = {field: index for index, field in enumerate(_field_name_per_index)}
         return self._field_name_per_index
 
-    def get_projections(self, builder: 'flatbuffers.builder.Builder', field_names: list = None):
-        if not field_names:
+    def get_projections(self, builder: 'flatbuffers.builder.Builder', field_names: Optional[List[str]] = None):
+        if field_names is None:
             field_names = self.field_name_per_index.keys()
         projection_fields = []
         for field_name in field_names:
             fb_field_index.Start(builder)
             fb_field_index.AddPosition(builder, self.field_name_per_index[field_name])
             offset = fb_field_index.End(builder)
             projection_fields.append(offset)
         fb_source.StartProjectionVector(builder, len(projection_fields))
         for offset in reversed(projection_fields):
             builder.PrependUOffsetTRelative(offset)
         return builder.EndVector()
 
     def serialize(self, builder: 'flatbuffers.builder.Builder'):
-        from ibis.expr.operations.generic import IsNull, Literal, TableColumn
+        from ibis.expr.operations.generic import (
+            IsNull,
+            Literal,
+            TableColumn,
+        )
         from ibis.expr.operations.logical import (
             And,
             Equals,
             Greater,
             GreaterEqual,
             Less,
             LessEqual,
@@ -194,15 +198,15 @@
             Equals: self.build_equal,
             NotEquals: self.build_not_equal,
             IsNull: self.build_is_null,
             Not: self.build_is_not_null,
             StringContains: self.build_match_substring,
         }
 
-        positions_map = dict((f.name, index) for index, f in enumerate(self.schema)) # TODO: BFS
+        positions_map = dict((f.name, index) for index, f in enumerate(self.schema))  # TODO: BFS
 
         self.builder = builder
 
         offsets = []
 
         if self.expr is not None:
             and_args = list(_flatten_args(self.expr.op(), And))
@@ -211,15 +215,15 @@
                 or_args = list(_flatten_args(op, Or))
                 _logger.debug('OR args: %s op %s', or_args, op)
                 inner_offsets = []
 
                 prev_field_name = None
                 for inner_op in or_args:
                     _logger.debug('inner_op %s', inner_op)
-                    builder_func = builder_map.get(type(inner_op))
+                    builder_func: Any = builder_map.get(type(inner_op))
                     if not builder_func:
                         raise NotImplementedError(inner_op.name)
 
                     if builder_func == self.build_is_null:
                         column, = inner_op.args
                         literal = None
                     elif builder_func == self.build_is_not_null:
@@ -266,28 +270,14 @@
         ref = fb_field_ref.End(self.builder)
 
         fb_expression.Start(self.builder)
         fb_expression.AddImplType(self.builder, ExpressionImpl.FieldRef)
         fb_expression.AddImpl(self.builder, ref)
         return fb_expression.End(self.builder)
 
-    def build_domain(self, column: int, field_name: str):
-        offsets = []
-        filters = self.filters[field_name]
-        if not filters:
-            return self.build_or([self.build_is_not_null(column)])
-
-        field_name, *field_attrs = field_name.split('.')
-        field = self.schema.field(field_name)
-        for attr in field_attrs:
-            field = field.type[attr]
-        for filter_by_name in filters:
-            offsets.append(self.build_range(column=column, field=field, filter_by_name=filter_by_name))
-        return self.build_or(offsets)
-
     def rule_to_operator(self, raw_rule: str):
         operator_matcher = {
             'eq': self.build_equal,
             'ge': self.build_greater_equal,
             'gt': self.build_greater,
             'lt': self.build_less,
             'le': self.build_less_equal,
@@ -335,14 +325,16 @@
 
         fb_expression.Start(self.builder)
         fb_expression.AddImplType(self.builder, ExpressionImpl.Call)
         fb_expression.AddImpl(self.builder, offset_call)
         return fb_expression.End(self.builder)
 
     def build_literal(self, field: pa.Field, value):
+        literal_type: Any
+
         if field.type.equals(pa.int64()):
             literal_type = fb_int64_lit
             literal_impl = LiteralImpl.Int64Literal
 
             field_type_type = Type.Int
             fb_int.Start(self.builder)
             fb_int.AddBitWidth(self.builder, field.type.bit_width)
@@ -547,21 +539,28 @@
     def build_is_not_null(self, column: int):
         return self.build_function('is_valid', column)
 
     def build_match_substring(self, column: int, literal: int):
         return self.build_function('match_substring', column, literal)
 
 
+class FieldNodesState:
+    def __init__(self) -> None:
+        # will be set during by the parser (see below)
+        self.buffers: Dict[int, Any] = defaultdict(lambda: None)  # a list of Arrow buffers (https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout)
+        self.length: Dict[int, Any] = defaultdict(lambda: None)  # each array must have it's length specified (https://arrow.apache.org/docs/python/generated/pyarrow.Array.html#pyarrow.Array.from_buffers)
+
+
 class FieldNode:
     """Helper class for representing nested Arrow fields and handling QueryData requests"""
     def __init__(self, field: pa.Field, index_iter, parent: Optional['FieldNode'] = None, debug: bool = False):
-        self.index = next(index_iter) # we use DFS-first enumeration for communicating the column positions to VAST
+        self.index = next(index_iter)  # we use DFS-first enumeration for communicating the column positions to VAST
         self.field = field
         self.type = field.type
-        self.parent = parent # will be None if this is the top-level field
+        self.parent = parent  # will be None if this is the top-level field
         self.debug = debug
         if isinstance(self.type, pa.StructType):
             self.children = [FieldNode(field, index_iter, parent=self) for field in self.type]
         elif isinstance(self.type, pa.ListType):
             self.children = [FieldNode(self.type.value_field, index_iter, parent=self)]
         elif isinstance(self.type, pa.MapType):
             # Map is represented as List<Struct<K, V>> in Arrow
@@ -570,19 +569,15 @@
             #
             #   if isinstance(self.type, (pa.ListType,  pa.StructType, pa.MapType)):
             #       self.children = [FieldNode(self.type.field(i), index_iter, parent=self) for i in range(self.type.num_fields)]
             #
             field = pa.field('entries', pa.struct([self.type.key_field, self.type.item_field]))
             self.children = [FieldNode(field, index_iter, parent=self)]
         else:
-            self.children = [] # for non-nested types
-
-        # will be set during by the parser (see below)
-        self.buffers = None # a list of Arrow buffers (https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout)
-        self.length = None # each array must have it's length specified (https://arrow.apache.org/docs/python/generated/pyarrow.Array.html#pyarrow.Array.from_buffers)
+            self.children = []  # for non-nested types
 
     def _iter_to_root(self) -> Iterator['FieldNode']:
         yield self
         if self.parent is not None:
             yield from self.parent._iter_to_root()
 
     def _iter_nodes(self) -> Iterator['FieldNode']:
@@ -595,84 +590,79 @@
         """Generate only leaf nodes (i.e. columns having scalar types)."""
         if not self.children:
             yield self
         else:
             for child in self.children:
                 yield from child._iter_leaves()
 
-    def _iter_leaves(self) -> Iterator['FieldNode']:
-        """Generate only leaf nodes (i.e. columns having scalar types)."""
-        if not self.children:
-            yield self
-        else:
-            for child in self.children:
-                yield from child._iter_leaves()
-
     def debug_log(self, level=0):
         """Recursively dump this node state to log."""
         bufs = self.buffers and [b and b.hex() for b in self.buffers]
-        _logger.debug('%s%d: %s, bufs=%s, len=%s', '    '*level, self.index, self.field, bufs, self.length)
+        _logger.debug('%s%d: %s, bufs=%s, len=%s', '    ' * level, self.index, self.field, bufs, self.length)
         for child in self.children:
-            child.debug_log(level=level+1)
+            child.debug_log(level=level + 1)
 
-    def set(self, arr: pa.Array):
+    def set(self, arr: pa.Array, state: FieldNodesState):
         """
         Assign the relevant Arrow buffers from the received array into this node.
 
         VAST can send only a single column at a time - together with its nesting levels.
         For example, `List<List<Int32>>` can be sent in a single go.
 
         Sending `Struct<a: Int32, b: Float64>` is not supported today, so each column is sent separately
         (possibly duplicating the nesting levels above it).
         For example, `Struct<A, B>` is sent as two separate columns: `Struct<A>` and `Struct<B>`.
         Also, `Map<K, V>` is sent (as its underlying representation): `List<Struct<K>>` and `List<Struct<V>>`
         """
-        buffers = arr.buffers()[:arr.type.num_buffers] # slicing is needed because Array.buffers() returns also nested array buffers
+        buffers = arr.buffers()[:arr.type.num_buffers]  # slicing is needed because Array.buffers() returns also nested array buffers
         if self.debug:
             _logger.debug("set: index=%d %s %s", self.index, self.field, [b and b.hex() for b in buffers])
-        if self.buffers is None:
-            self.buffers = buffers
-            self.length = len(arr)
+        if state.buffers[self.index] is None:
+            state.buffers[self.index] = buffers
+            state.length[self.index] = len(arr)
         else:
             # Make sure subsequent assignments are consistent with each other
             if self.debug:
-                if not self.buffers == buffers:
-                    raise ValueError(f'self.buffers: {self.buffers} are not equal with buffers: {buffers}')
-            if not self.length == len(arr):
-                raise ValueError(f'self.length: {self.length} are not equal with len(arr): {len(arr)}')
+                if not state.buffers[self.index] == buffers:
+                    raise ValueError(f'self.buffers: {state.buffers[self.index]} are not equal with buffers: {buffers}')
+            if not state.length[self.index] == len(arr):
+                raise ValueError(f'self.length: {state.length[self.index]} are not equal with len(arr): {len(arr)}')
 
-    def build(self) -> pa.Array:
+    def build(self, state: FieldNodesState) -> pa.Array:
         """Construct an Arrow array from the collected buffers (recursively)."""
-        children = self.children and [node.build() for node in self.children]
-        result = pa.Array.from_buffers(self.type, self.length, buffers=self.buffers, children=children)
+        children = self.children and [node.build(state) for node in self.children]
+        result = pa.Array.from_buffers(self.type, state.length[self.index], buffers=state.buffers[self.index], children=children)
         if self.debug:
             _logger.debug('%s result=%s', self.field, result)
         return result
 
 
 class QueryDataParser:
+    class QueryDataParserState(FieldNodesState):
+        def __init__(self) -> None:
+            super().__init__()
+            self.leaf_offset = 0
+
     """Used to parse VAST QueryData RPC response."""
     def __init__(self, arrow_schema: pa.Schema, *, debug=False):
         self.arrow_schema = arrow_schema
-        index = itertools.count() # used to generate leaf column positions for VAST QueryData RPC
+        index = itertools.count()  # used to generate leaf column positions for VAST QueryData RPC
         self.nodes = [FieldNode(field, index, debug=debug) for field in arrow_schema]
         self.debug = debug
         if self.debug:
             for node in self.nodes:
                 node.debug_log()
         self.leaves = [leaf for node in self.nodes for leaf in node._iter_leaves()]
 
-        self.leaf_offset = 0
-
-    def parse(self, column: pa.Array):
+    def parse(self, column: pa.Array, state: QueryDataParserState):
         """Parse a single column response from VAST (see FieldNode.set for details)"""
-        if not self.leaf_offset < len(self.leaves):
-            raise ValueError(f'self.leaf_offset: {self.leaf_offset} are not < '
+        if not state.leaf_offset < len(self.leaves):
+            raise ValueError(f'state.leaf_offset: {state.leaf_offset} are not < '
                              f'than len(self.leaves): {len(self.leaves)}')
-        leaf = self.leaves[self.leaf_offset]
+        leaf = self.leaves[state.leaf_offset]
 
         # A column response may be sent in multiple chunks, therefore we need to combine
         # it into a single chunk to allow reconstruction using `Array.from_buffers()`.
         column = column.combine_chunks()
 
         if self.debug:
             _logger.debug("parse: index=%d buffers=%s", leaf.index, [b and b.hex() for b in column.buffers()])
@@ -681,123 +671,112 @@
         # Collect all nesting levels, e.g. `List<Struct<A>` will be split into [`List`, `Struct`, `A`].
         # This way we can extract the buffers from each level and assign them to the appropriate node in loop below.
         array_list = list(_iter_nested_arrays(column))
         if len(array_list) != len(node_list):
             raise ValueError(f'len(array_list): {len(array_list)} are not eq '
                              f'with len(node_list): {len(node_list)}')
         for node, arr in zip(node_list, array_list):
-            node.set(arr)
+            node.set(arr, state)
 
-        self.leaf_offset += 1
+        state.leaf_offset += 1
 
-    def build(self) -> Optional[pa.Table]:
+    def build(self, state: QueryDataParserState) -> Optional[pa.Table]:
         """Try to build the resulting Table object (if all columns were parsed)"""
-        if self.leaf_offset < len(self.leaves):
+        if state.leaf_offset < len(self.leaves):
             return None
 
         if self.debug:
             for node in self.nodes:
                 node.debug_log()
 
         result = pa.Table.from_arrays(
-            arrays=[node.build() for node in self.nodes],
+            arrays=[node.build(state) for node in self.nodes],
             schema=self.arrow_schema)
-        result.validate(full=self.debug) # does expensive validation checks only if debug is enabled
+        result.validate(full=self.debug)  # does expensive validation checks only if debug is enabled
         return result
 
+
 def _iter_nested_arrays(column: pa.Array) -> Iterator[pa.Array]:
     """Iterate over a single column response, and recursively generate all of its children."""
     yield column
     if isinstance(column.type, pa.StructType):
         if not column.type.num_fields == 1:  # Note: VAST serializes only a single struct field at a time
             raise ValueError(f'column.type.num_fields: {column.type.num_fields} not eq to 1')
         yield from _iter_nested_arrays(column.field(0))
     elif isinstance(column.type, pa.ListType):
         yield from _iter_nested_arrays(column.values)  # Note: Map is serialized in VAST as a List<Struct<K, V>>
 
 
-TableInfo = namedtuple('table_info', 'name properties handle num_rows size_in_bytes')
+TableInfo = namedtuple('TableInfo', 'name properties handle num_rows size_in_bytes')
+
+
 def _parse_table_info(obj):
 
     name = obj.Name().decode()
     properties = obj.Properties().decode()
     handle = obj.Handle().decode()
     num_rows = obj.NumRows()
     used_bytes = obj.SizeInBytes()
     return TableInfo(name, properties, handle, num_rows, used_bytes)
 
+
 def build_record_batch(column_info, column_values):
     fields = [pa.field(column_name, column_type) for column_type, column_name in column_info]
     schema = pa.schema(fields)
     arrays = [pa.array(column_values[column_type], type=column_type) for column_type, _ in column_info]
     batch = pa.record_batch(arrays, schema)
     return serialize_record_batch(batch)
 
+
 def serialize_record_batch(batch):
     sink = pa.BufferOutputStream()
     with pa.ipc.new_stream(sink, batch.schema) as writer:
         writer.write(batch)
     return sink.getvalue()
 
 # Results that returns from tablestats
-TableStatsResult = namedtuple("TableStatsResult",["num_rows", "size_in_bytes", "is_external_rowid_alloc", "endpoints"])
+
+
+TableStatsResult = namedtuple("TableStatsResult", ["num_rows", "size_in_bytes", "is_external_rowid_alloc", "endpoints"])
+
 
 class VastdbApi:
     # we expect the vast version to be <major>.<minor>.<patch>.<protocol>
     VAST_VERSION_REGEX = re.compile(r'^vast (\d+\.\d+\.\d+\.\d+)$')
 
-    def __init__(self, endpoint, access_key, secret_key, username=None, password=None,
-                 secure=False, auth_type=AuthType.SIGV4):
-        url_dict = urllib3.util.parse_url(endpoint)._asdict()
+    def __init__(self, endpoint, access_key, secret_key, auth_type=AuthType.SIGV4, ssl_verify=True):
+        url = urllib3.util.parse_url(endpoint)
         self.access_key = access_key
         self.secret_key = secret_key
-        self.username = username
-        self.password = password
-        self.secure = secure
-        self.auth_type = auth_type
-        self.executor_hosts = [endpoint]  # TODO: remove
-
-        username = username or ''
-        password = password or ''
-        if not url_dict['port']:
-            url_dict['port'] = 443 if secure else 80
-
-        self.port = url_dict['port']
 
         self.default_max_list_columns_page_size = 1000
         self.session = requests.Session()
-        self.session.verify = False
+        self.session.verify = ssl_verify
         self.session.headers['user-agent'] = "VastData Tabular API 1.0 - 2022 (c)"
-        if auth_type == AuthType.BASIC:
-            self.session.auth = requests.auth.HTTPBasicAuth(username, password)
-        else:
-            if url_dict['port'] != 80 and url_dict['port'] != 443:
-                self.aws_host = '{host}:{port}'.format(**url_dict)
-            else:
-                self.aws_host = '{host}'.format(**url_dict)
-
-            self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
-                                                aws_secret_access_key=secret_key,
-                                                aws_host=self.aws_host,
-                                                aws_region='us-east-1',
-                                                aws_service='s3')
 
-        if not url_dict['scheme']:
-            url_dict['scheme'] = "https" if secure else "http"
+        if url.port in {80, 443, None}:
+            self.aws_host = f'{url.host}'
+        else:
+            self.aws_host = f'{url.host}:{url.port}'
 
-        url = urllib3.util.Url(**url_dict)
         self.url = str(url)
         _logger.debug('url=%s aws_host=%s', self.url, self.aws_host)
 
+        self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
+                                            aws_secret_access_key=secret_key,
+                                            aws_host=self.aws_host,
+                                            aws_region='us-east-1',
+                                            aws_service='s3')
+
         # probe the cluster for its version
         self.vast_version = None
-        res = self.session.options(self.url)
+        res = self.session.get(self.url)
         server_header = res.headers.get("Server")
         if server_header is None:
-            _logger.error("OPTIONS response doesn't contain 'Server' header")
+            _logger.error("Response doesn't contain 'Server' header")
         else:
             _logger.debug("Server header is '%s'", server_header)
             if m := self.VAST_VERSION_REGEX.match(server_header):
                 self.vast_version, = m.groups()
                 return
             else:
                 _logger.error("'Server' header '%s' doesn't match the expected pattern", server_header)
@@ -990,17 +969,16 @@
             is_truncated = list_res['IsTruncated'] == 'true'
             marker = list_res['Marker']
             common_prefixes = list_res['CommonPrefixes'] if 'CommonPrefixes' in list_res else []
             snapshots = [v['Prefix'] for v in common_prefixes]
 
             return snapshots, is_truncated, marker
 
-
     def create_table(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[],
-                     topic_partitions=0, create_imports_table=False):
+                     topic_partitions=0, create_imports_table=False, use_external_row_ids_allocation=False):
         """
         Create a table, use the following request
         POST /bucket/schema/table?table HTTP/1.1
 
         Request Headers
         tabular-txid: <integer> TransactionId
         tabular-client-tag: <string> ClientTag
@@ -1013,14 +991,17 @@
         The request will look like:
         POST /bucket/schema/table?table&sub-table=vastdb-imported-objects HTTP/1.1
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
 
         serialized_schema = arrow_schema.serialize()
         headers['Content-Length'] = str(len(serialized_schema))
+        if use_external_row_ids_allocation:
+            headers['use-external-row-ids-alloc'] = str(use_external_row_ids_allocation)
+
         url_params = {'topic_partitions': str(topic_partitions)} if topic_partitions else {}
         if create_imports_table:
             url_params['sub-table'] = IMPORTED_OBJECTS_TABLE_NAME
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
                                 data=serialized_schema, headers=headers)
         return self._check_res(res, "create_table", expected_retvals)
@@ -1029,64 +1010,67 @@
                                          parquet_bucket_name=None, parquet_object_name=None,
                                          txid=0, client_tags=[], expected_retvals=[]):
 
         # Use pyarrow.parquet.ParquetDataset to open the Parquet file
         if parquet_path:
             parquet_ds = pq.ParquetDataset(parquet_path)
         elif parquet_bucket_name and parquet_object_name:
-            s3fs  = pa.fs.S3FileSystem(access_key=self.access_key, secret_key=self.secret_key, endpoint_override=self.url)
-            parquet_ds = pq.ParquetDataset('/'.join([parquet_bucket_name,parquet_object_name]), filesystem=s3fs)
+            s3fs = pa.fs.S3FileSystem(access_key=self.access_key, secret_key=self.secret_key, endpoint_override=self.url)
+            parquet_ds = pq.ParquetDataset('/'.join([parquet_bucket_name, parquet_object_name]), filesystem=s3fs)
         else:
             raise RuntimeError(f'invalid params parquet_path={parquet_path} parquet_bucket_name={parquet_bucket_name} parquet_object_name={parquet_object_name}')
 
         # Get the schema of the Parquet file
         if isinstance(parquet_ds.schema, pq.ParquetSchema):
             arrow_schema = parquet_ds.schema.to_arrow_schema()
         elif isinstance(parquet_ds.schema, pa.Schema):
             arrow_schema = parquet_ds.schema
         else:
             raise RuntimeError(f'invalid type(parquet_ds.schema) = {type(parquet_ds.schema)}')
 
         # create the table
         return self.create_table(bucket, schema, name, arrow_schema, txid, client_tags, expected_retvals)
 
-
     def get_table_stats(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[]):
         """
         GET /mybucket/myschema/mytable?stats HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats"), headers=headers)
-        if res.status_code == 200:
-            flatbuf = b''.join(res.iter_content(chunk_size=128))
-            stats = get_table_stats.GetRootAs(flatbuf)
-            num_rows = stats.NumRows()
-            size_in_bytes = stats.SizeInBytes()
-            is_external_rowid_alloc = stats.IsExternalRowidAlloc()
-            endpoints = []
-            if stats.VipsLength() == 0:
-                endpoints.append(self.url)
-            else:
-                ip_cls = IPv6Address if (stats.AddressType() == "ipv6") else IPv4Address
-                vips = [stats.Vips(i) for i in range(stats.VipsLength())]
-                ips = []
-                # extract the vips into list of IPs
-                for vip in vips:
-                    start_ip = int(ip_cls(vip.StartAddress().decode()))
-                    ips.extend(ip_cls(start_ip + i) for i  in range(vip.AddressCount()))
-                for ip in ips:
-                    prefix = "http" if not self.secure else "https"
-                    endpoints.append(f"{prefix}://{str(ip)}:{self.port}")
-            return TableStatsResult(num_rows, size_in_bytes, is_external_rowid_alloc, endpoints)
+        self._check_res(res, "get_table_stats", expected_retvals)
+
+        flatbuf = b''.join(res.iter_content(chunk_size=128))
+        stats = get_table_stats.GetRootAs(flatbuf)
+        num_rows = stats.NumRows()
+        size_in_bytes = stats.SizeInBytes()
+        is_external_rowid_alloc = stats.IsExternalRowidAlloc()
+        endpoints = []
+        if stats.VipsLength() == 0:
+            endpoints.append(self.url)
+        else:
+            url = urllib3.util.parse_url(self.url)
 
-        return self._check_res(res, "get_table_stats", expected_retvals)
+            ip_cls = IPv6Address if (stats.AddressType() == "ipv6") else IPv4Address
+            vips = [stats.Vips(i) for i in range(stats.VipsLength())]
+            ips = []
+            # extract the vips into list of IPs
+            for vip in vips:
+                start_ip = int(ip_cls(vip.StartAddress().decode()))
+                ips.extend(ip_cls(start_ip + i) for i in range(vip.AddressCount()))
+            # build a list of endpoint URLs, reusing schema and port (if specified when constructing the session).
+            # it is assumed that the client can access the returned IPs (e.g. if they are part of the VIP pool).
+            for ip in ips:
+                d = url._asdict()
+                d['host'] = str(ip)
+                endpoints.append(str(urllib3.util.Url(**d)))
+        return TableStatsResult(num_rows, size_in_bytes, is_external_rowid_alloc, tuple(endpoints))
 
     def alter_table(self, bucket, schema, name, txid=0, client_tags=[], table_properties="",
                     new_name="", expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?table HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
@@ -1167,15 +1151,14 @@
             tables_length = lists.TablesLength()
             count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else tables_length
             for i in range(tables_length):
                 tables.append(_parse_table_info(lists.Tables(i)))
 
             return bucket_name, schema_name, tables, next_key, is_truncated, count
 
-
     def add_columns(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[]):
         """
         Add a column to table, use the following request
         POST /bucket/schema/table?column HTTP/1.1
 
         Request Headers
         tabular-txid: <integer> TransactionId
@@ -1193,15 +1176,15 @@
         headers['Content-Length'] = str(len(serialized_schema))
 
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=name, command="column"),
                                 data=serialized_schema, headers=headers)
         return self._check_res(res, "add_columns", expected_retvals)
 
     def alter_column(self, bucket, schema, table, name, txid=0, client_tags=[], column_properties="",
-                     new_name="", column_sep = ".", column_stats="", expected_retvals=[]):
+                     new_name="", column_sep=".", column_stats="", expected_retvals=[]):
         """
         PUT /bucket/schema/table?column&tabular-column-name=ColumnName&tabular-new-column-name=NewColumnName HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         tabular-column-sep: ColumnSep
 
@@ -1222,15 +1205,15 @@
         builder.Finish(params)
         alter_column_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['tabular-column-sep'] = column_sep
         headers['Content-Length'] = str(len(alter_column_req))
 
-        url_params = {'tabular-column-name': name }
+        url_params = {'tabular-column-name': name}
         if len(new_name):
             url_params['tabular-new-column-name'] = new_name
 
         res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column", url_params=url_params),
                                data=alter_column_req, headers=headers)
         return self._check_res(res, "alter_column", expected_retvals)
 
@@ -1569,15 +1552,15 @@
                                 data=import_req, headers=headers, stream=True)
         if blocking:
             res = iterate_over_import_data_response(res)
 
         return self._check_res(res, "import_data", expected_retvals)
 
     def _record_batch_slices(self, batch, rows_per_slice=None):
-        max_slice_size_in_bytes = int(0.9*5*1024*1024) # 0.9 * 5MB
+        max_slice_size_in_bytes = int(0.9 * 5 * 1024 * 1024)  # 0.9 * 5MB
         batch_len = len(batch)
         serialized_batch = serialize_record_batch(batch)
         batch_size_in_bytes = len(serialized_batch)
         _logger.debug('max_slice_size_in_bytes=%d batch_len=%d batch_size_in_bytes=%d',
                       max_slice_size_in_bytes, batch_len, batch_size_in_bytes)
 
         if not rows_per_slice:
@@ -1587,29 +1570,29 @@
                 rows_per_slice = int(0.9 * batch_len * max_slice_size_in_bytes / batch_size_in_bytes)
 
         done_slicing = False
         while not done_slicing:
             # Attempt slicing according to the current rows_per_slice
             offset = 0
             serialized_slices = []
-            for i in range(math.ceil(batch_len/rows_per_slice)):
+            for i in range(math.ceil(batch_len / rows_per_slice)):
                 offset = rows_per_slice * i
                 if offset >= batch_len:
-                    done_slicing=True
+                    done_slicing = True
                     break
                 slice_batch = batch.slice(offset, rows_per_slice)
                 serialized_slice_batch = serialize_record_batch(slice_batch)
                 sizeof_serialized_slice_batch = len(serialized_slice_batch)
 
                 if sizeof_serialized_slice_batch <= max_slice_size_in_bytes:
                     serialized_slices.append(serialized_slice_batch)
                 else:
                     _logger.info(f'Using rows_per_slice {rows_per_slice} slice {i} size {sizeof_serialized_slice_batch} exceeds {max_slice_size_in_bytes} bytes, trying smaller rows_per_slice')
                     # We have a slice that is too large
-                    rows_per_slice = int(rows_per_slice/2)
+                    rows_per_slice = int(rows_per_slice / 2)
                     if rows_per_slice < 1:
                         raise ValueError('cannot decrease batch size below 1 row')
                     break
             else:
                 done_slicing = True
 
         return serialized_slices
@@ -1624,15 +1607,16 @@
         Request Body
             RecordBatch
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
                                 data=record_batch, headers=headers, stream=True)
-        return self._check_res(res, "insert_rows", expected_retvals)
+        self._check_res(res, "insert_rows", expected_retvals)
+        res.raw.read()  # flush the response
 
     def update_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
@@ -1640,15 +1624,15 @@
         Request Body
             RecordBatch where first column must be row_id
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
                                 data=record_batch, headers=headers)
-        return self._check_res(res, "update_rows", expected_retvals)
+        self._check_res(res, "update_rows", expected_retvals)
 
     def delete_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[],
                     delete_from_imports_table=False):
         """
         DELETE /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
@@ -1659,15 +1643,15 @@
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if delete_from_imports_table else {}
 
         res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows", url_params=url_params),
                                   data=record_batch, headers=headers)
-        return self._check_res(res, "delete_rows", expected_retvals)
+        self._check_res(res, "delete_rows", expected_retvals)
 
     def create_projection(self, bucket, schema, table, name, columns, txid=0, client_tags=[], expected_retvals=[]):
         """
         Create a table, use the following request
         POST /bucket/schema/table?projection&name=my_projection HTTP/1.1
 
         The user may define several Sorted and/Or Unsorted columns from the original table
@@ -1869,14 +1853,18 @@
                 for f in schema_out:
                     columns.append([f.name, f.type, f.metadata])
                 #   sort_type = f.metadata[b'VAST:sort_type'].decode()
 
             return columns, next_key, is_truncated, count
 
 
+class QueryDataInternalError(Exception):
+    pass
+
+
 def _iter_query_data_response_columns(fileobj, stream_ids=None):
     readers = {}  # {stream_id: pa.ipc.RecordBatchStreamReader}
     while True:
         stream_id_bytes = fileobj.read(4)
         if not stream_id_bytes:
             if readers:
                 raise EOFError(f'no readers ({readers}) should be open at EOF')
@@ -1893,70 +1881,73 @@
             res = fileobj.read()
             _logger.debug("stream_id=%d res=%s (finish)", stream_id, res)
             return
 
         if stream_id == TABULAR_QUERY_DATA_FAILED_STREAM_ID:
             # read the terminating end chunk from socket
             res = fileobj.read()
-            _logger.warning("stream_id=%d res=%s (failed)", stream_id, res)
-            raise IOError(f"Query data stream failed res={res}")
+            _logger.debug("stream_id=%d res=%s (failed)", stream_id, res)
+            raise QueryDataInternalError()  # connection closed by server due to an internal error
 
         next_row_id_bytes = fileobj.read(8)
         next_row_id, = struct.unpack('<Q', next_row_id_bytes)
         _logger.debug("stream_id=%d next_row_id=%d", stream_id, next_row_id)
 
         if stream_id not in readers:
             # we implicitly read 1st message (Arrow schema) when constructing RecordBatchStreamReader
             reader = pa.ipc.RecordBatchStreamReader(fileobj)
             _logger.debug("stream_id=%d schema=%s", stream_id, reader.schema)
             readers[stream_id] = (reader, [])
             continue
 
         (reader, batches) = readers[stream_id]
         try:
-            batch = reader.read_next_batch() # read single-column chunk data
+            batch = reader.read_next_batch()  # read single-column chunk data
             _logger.debug("stream_id=%d rows=%d chunk=%s", stream_id, len(batch), batch)
             batches.append(batch)
         except StopIteration:  # we got an end-of-stream IPC message for a given stream ID
             reader, batches = readers.pop(stream_id)  # end of column
             table = pa.Table.from_batches(batches)  # concatenate all column chunks (as a single)
             _logger.debug("stream_id=%d rows=%d column=%s", stream_id, len(table), table)
             yield (stream_id, next_row_id, table)
 
 
-def parse_query_data_response(conn, schema, stream_ids=None, start_row_ids=None, debug=False):
+def parse_query_data_response(conn, schema, stream_ids=None, start_row_ids=None, debug=False, parser: Optional[QueryDataParser] = None):
     """
     Generates pyarrow.Table objects from QueryData API response stream.
 
     A pyarrow.Table is a helper class that combines a Schema with multiple RecordBatches and allows easy data access.
     """
     if start_row_ids is None:
         start_row_ids = {}
 
     is_empty_projection = (len(schema) == 0)
-    parsers = defaultdict(lambda: QueryDataParser(schema, debug=debug))  # {stream_id: QueryDataParser}
+    if parser is None:
+        parser = QueryDataParser(schema, debug=debug)
+    states: Dict[int, QueryDataParser.QueryDataParserState] = defaultdict(lambda: QueryDataParser.QueryDataParserState())  # {stream_id: QueryDataParser}
 
     for stream_id, next_row_id, table in _iter_query_data_response_columns(conn, stream_ids):
-        parser = parsers[stream_id]
+        state = states[stream_id]
         for column in table.columns:
-            parser.parse(column)
+            parser.parse(column, state)
 
-        parsed_table = parser.build()
+        parsed_table = parser.build(state)
         if parsed_table is not None:  # when we got all columns (and before starting a new "select_rows" cycle)
-            parsers.pop(stream_id)
+            states.pop(stream_id)
             if is_empty_projection:  # VAST returns an empty RecordBatch, with the correct rows' count
                 parsed_table = table
 
             _logger.debug("stream_id=%d rows=%d next_row_id=%d table=%s",
                           stream_id, len(parsed_table), next_row_id, parsed_table)
             start_row_ids[stream_id] = next_row_id
             yield parsed_table  # the result of a single "select_rows()" cycle
 
-    if parsers:
-        raise EOFError(f'all streams should be done before EOF. {parsers}')
+    if states:
+        raise EOFError(f'all streams should be done before EOF. {states}')
+
 
 def get_field_type(builder: flatbuffers.Builder, field: pa.Field):
     if field.type.equals(pa.int64()):
         field_type_type = Type.Int
         fb_int.Start(builder)
         fb_int.AddBitWidth(builder, field.type.bit_width)
         fb_int.AddIsSigned(builder, True)
@@ -2091,14 +2082,15 @@
         field_type = fb_fixed_size_binary.End(builder)
 
     else:
         raise ValueError(f'unsupported predicate for type={field.type}')
 
     return field_type, field_type_type
 
+
 def build_field(builder: flatbuffers.Builder, f: pa.Field, name: str):
     children = None
     if isinstance(f.type, pa.StructType):
         children = [build_field(builder, child, child.name) for child in list(f.type)]
     if isinstance(f.type, pa.ListType):
         children = [build_field(builder, f.type.value_field, "item")]
     if isinstance(f.type, pa.MapType):
@@ -2138,20 +2130,21 @@
     fb_field.AddType(builder, field_type)
     if children is not None:
         fb_field.AddChildren(builder, children)
     return fb_field.End(builder)
 
 
 class QueryDataRequest:
-    def __init__(self, serialized, response_schema):
+    def __init__(self, serialized, response_schema, response_parser):
         self.serialized = serialized
         self.response_schema = response_schema
+        self.response_parser = response_parser
 
 
-def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), predicate: ibis.expr.types.BooleanColumn = None, field_names: list = None):
+def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), predicate: ibis.expr.types.BooleanColumn = None, field_names: Optional[List[str]] = None):
     builder = flatbuffers.Builder(1024)
 
     source_name = builder.CreateString('')  # required
 
     fields = [build_field(builder, f, f.name) for f in schema]
 
     fb_schema.StartFieldsVector(builder, len(fields))
@@ -2197,15 +2190,16 @@
 
     fb_relation.Start(builder)
     fb_relation.AddImplType(builder, rel_impl.RelationImpl.Source)
     fb_relation.AddImpl(builder, source)
     relation = fb_relation.End(builder)
 
     builder.Finish(relation)
-    return QueryDataRequest(serialized=builder.Output(), response_schema=response_schema)
+
+    return QueryDataRequest(serialized=builder.Output(), response_schema=response_schema, response_parser=QueryDataParser(response_schema))
 
 
 def convert_column_types(table: 'pa.Table') -> 'pa.Table':
     """
     Adjusting table values
 
     1. Because the timestamp resolution is too high it is necessary to trim it. ORION-96961
```

### Comparing `vastdb-0.1.1/vastdb/schema.py` & `vastdb-0.1.2/vastdb/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
 import logging
 from dataclasses import dataclass
+from typing import TYPE_CHECKING, List, Optional
 
 import pyarrow as pa
 
 from . import bucket, errors, schema, table
 
+if TYPE_CHECKING:
+    from .table import Table
+
+
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Schema:
     """VAST Schema."""
 
@@ -22,45 +27,45 @@
     bucket: "bucket.Bucket"
 
     @property
     def tx(self):
         """VAST transaction used for this schema."""
         return self.bucket.tx
 
-    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True) -> "table.Table":
+    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True) -> "Table":
         """Create a new table under this schema."""
         if current := self.table(table_name, fail_if_missing=False):
             if fail_if_exists:
                 raise errors.TableExists(self.bucket.name, self.name, table_name)
             else:
                 return current
         self.tx._rpc.api.create_table(self.bucket.name, self.name, table_name, columns, txid=self.tx.txid)
         log.info("Created table: %s", table_name)
-        return self.table(table_name)
+        return self.table(table_name)  # type: ignore[return-value]
 
-    def table(self, name: str, fail_if_missing=True) -> "table.Table":
+    def table(self, name: str, fail_if_missing=True) -> Optional["table.Table"]:
         """Get a specific table under this schema."""
         t = self.tables(table_name=name)
         if not t:
             if fail_if_missing:
                 raise errors.MissingTable(self.bucket.name, self.name, name)
             else:
                 return None
         assert len(t) == 1, f"Expected to receive only a single table, but got: {len(t)}. tables: {t}"
         log.debug("Found table: %s", t[0])
         return t[0]
 
-    def tables(self, table_name=None) -> ["table.Table"]:
+    def tables(self, table_name=None) -> List["Table"]:
         """List all tables under this schema."""
         tables = []
         next_key = 0
         name_prefix = table_name if table_name else ""
         exact_match = bool(table_name)
         while True:
-            bucket_name, schema_name, curr_tables, next_key, is_truncated, _ = \
+            _bucket_name, _schema_name, curr_tables, next_key, is_truncated, _ = \
                 self.tx._rpc.api.list_tables(
                     bucket=self.bucket.name, schema=self.name, next_key=next_key, txid=self.tx.txid,
                     exact_match=exact_match, name_prefix=name_prefix, include_list_stats=exact_match)
             if not curr_tables:
                 break
             tables.extend(curr_tables)
             if not is_truncated:
```

### Comparing `vastdb-0.1.1/vastdb/session.py` & `vastdb-0.1.2/vastdb/session.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vastdb/table.py` & `vastdb-0.1.2/vastdb/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,108 +1,104 @@
 import concurrent.futures
 import logging
 import os
 import queue
 from dataclasses import dataclass, field
 from math import ceil
 from threading import Event
-from typing import List, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import ibis
 import pyarrow as pa
 
-from . import errors, schema
-from .internal_commands import (
-    TABULAR_INVALID_ROW_ID,
-    VastdbApi,
-    build_query_data_request,
-    parse_query_data_response,
-)
+from . import errors, internal_commands, schema
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
 MAX_ROWS_PER_BATCH = 512 * 1024
 # for insert we need a smaller limit due to response amplification
 # for example insert of 512k uint8 result in 512k*8bytes response since row_ids are uint64
 MAX_INSERT_ROWS_PER_PATCH = 512 * 1024
 
+
 @dataclass
 class TableStats:
     num_rows: int
     size_in_bytes: int
     is_external_rowid_alloc: bool = False
-    endpoints: List[str] = None
+    endpoints: Tuple[str, ...] = ()
+
 
 @dataclass
 class QueryConfig:
     num_sub_splits: int = 4
     num_splits: int = 1
-    data_endpoints: [str] = None
+    data_endpoints: Optional[List[str]] = None
     limit_rows_per_sub_split: int = 128 * 1024
     num_row_groups_per_sub_split: int = 8
     use_semi_sorted_projections: bool = True
     rows_per_split: int = 4000000
     query_id: str = ""
 
 
 @dataclass
 class ImportConfig:
     import_concurrency: int = 2
 
+
 class SelectSplitState():
-    def __init__(self, query_data_request, table : "Table", split_id : int, config: QueryConfig) -> None:
+    def __init__(self, query_data_request, table: "Table", split_id: int, config: QueryConfig) -> None:
         self.split_id = split_id
         self.subsplits_state = {i: 0 for i in range(config.num_sub_splits)}
         self.config = config
         self.query_data_request = query_data_request
         self.table = table
 
-    def batches(self, api : VastdbApi):
+    def batches(self, api: internal_commands.VastdbApi):
         while not self.done:
             response = api.query_data(
                             bucket=self.table.bucket.name,
                             schema=self.table.schema.name,
                             table=self.table.name,
                             params=self.query_data_request.serialized,
                             split=(self.split_id, self.config.num_splits, self.config.num_row_groups_per_sub_split),
                             num_sub_splits=self.config.num_sub_splits,
                             response_row_id=False,
                             txid=self.table.tx.txid,
                             limit_rows=self.config.limit_rows_per_sub_split,
                             sub_split_start_row_ids=self.subsplits_state.items(),
                             enable_sorted_projections=self.config.use_semi_sorted_projections)
-            pages_iter = parse_query_data_response(
+            pages_iter = internal_commands.parse_query_data_response(
                 conn=response.raw,
                 schema=self.query_data_request.response_schema,
-                start_row_ids=self.subsplits_state)
+                start_row_ids=self.subsplits_state,
+                parser=self.query_data_request.response_parser)
 
             for page in pages_iter:
                 for batch in page.to_batches():
                     if len(batch) > 0:
                         yield batch
 
-
     @property
     def done(self):
-        return all(row_id == TABULAR_INVALID_ROW_ID for row_id in self.subsplits_state.values())
+        return all(row_id == internal_commands.TABULAR_INVALID_ROW_ID for row_id in self.subsplits_state.values())
+
 
 @dataclass
 class Table:
     name: str
     schema: "schema.Schema"
     handle: int
     stats: TableStats
-    properties: dict = None
     arrow_schema: pa.Schema = field(init=False, compare=False)
     _ibis_table: ibis.Schema = field(init=False, compare=False)
 
     def __post_init__(self):
-        self.properties = self.properties or {}
         self.arrow_schema = self.columns()
 
         table_path = f'{self.schema.bucket.name}/{self.schema.name}/{self.name}'
         self._ibis_table = ibis.table(ibis.Schema.from_pyarrow(self.arrow_schema), table_path)
 
     @property
     def tx(self):
@@ -132,40 +128,40 @@
         projs = self.projections(projection_name=name)
         if not projs:
             raise errors.MissingProjection(self.bucket.name, self.schema.name, self.name, name)
         assert len(projs) == 1, f"Expected to receive only a single projection, but got: {len(projs)}. projections: {projs}"
         log.debug("Found projection: %s", projs[0])
         return projs[0]
 
-    def projections(self, projection_name=None) -> ["Projection"]:
+    def projections(self, projection_name=None) -> List["Projection"]:
         projections = []
         next_key = 0
         name_prefix = projection_name if projection_name else ""
         exact_match = bool(projection_name)
         while True:
-            bucket_name, schema_name, table_name, curr_projections, next_key, is_truncated, _ = \
+            _bucket_name, _schema_name, _table_name, curr_projections, next_key, is_truncated, _ = \
                 self.tx._rpc.api.list_projections(
                     bucket=self.bucket.name, schema=self.schema.name, table=self.name, next_key=next_key, txid=self.tx.txid,
                     exact_match=exact_match, name_prefix=name_prefix)
             if not curr_projections:
                 break
             projections.extend(curr_projections)
             if not is_truncated:
                 break
         return [_parse_projection_info(projection, self) for projection in projections]
 
-    def import_files(self, files_to_import: [str], config: ImportConfig = None) -> None:
+    def import_files(self, files_to_import: List[str], config: Optional[ImportConfig] = None) -> None:
         source_files = {}
         for f in files_to_import:
             bucket_name, object_path = _parse_bucket_and_object_names(f)
             source_files[(bucket_name, object_path)] = b''
 
         self._execute_import(source_files, config=config)
 
-    def import_partitioned_files(self, files_and_partitions: {str: pa.RecordBatch}, config: ImportConfig = None) -> None:
+    def import_partitioned_files(self, files_and_partitions: Dict[str, pa.RecordBatch], config: Optional[ImportConfig] = None) -> None:
         source_files = {}
         for f, record_batch in files_and_partitions.items():
             bucket_name, object_path = _parse_bucket_and_object_names(f)
             serialized_batch = _serialize_record_batch(record_batch)
             source_files = {(bucket_name, object_path): serialized_batch.to_pybytes()}
 
         self._execute_import(source_files, config=config)
@@ -205,74 +201,82 @@
                 raise
 
         futures = []
         with concurrent.futures.ThreadPoolExecutor(
                 max_workers=config.import_concurrency, thread_name_prefix='import_thread') as pool:
             try:
                 for endpoint in endpoints:
-                    session = VastdbApi(endpoint, self.tx._rpc.api.access_key, self.tx._rpc.api.secret_key)
+                    session = internal_commands.VastdbApi(endpoint, self.tx._rpc.api.access_key, self.tx._rpc.api.secret_key)
                     futures.append(pool.submit(import_worker, files_queue, session))
 
                 log.debug("Waiting for import workers to finish")
                 for future in concurrent.futures.as_completed(futures):
                     future.result()
             finally:
                 stop_event.set()
                 # ThreadPoolExecutor will be joined at the end of the context
-    def refresh_stats(self):
+
+    def get_stats(self) -> TableStats:
         stats_tuple = self.tx._rpc.api.get_table_stats(
             bucket=self.bucket.name, schema=self.schema.name, name=self.name, txid=self.tx.txid)
-        self.stats = TableStats(**stats_tuple._asdict())
+        return TableStats(**stats_tuple._asdict())
 
-    def select(self, columns: [str] = None,
+    def select(self, columns: Optional[List[str]] = None,
                predicate: ibis.expr.types.BooleanColumn = None,
-               config: QueryConfig = None,
+               config: Optional[QueryConfig] = None,
                *,
                internal_row_id: bool = False) -> pa.RecordBatchReader:
         if config is None:
             config = QueryConfig()
 
-        self.refresh_stats()
+        # Take a snapshot of enpoints
+        stats = self.get_stats()
+        endpoints = stats.endpoints if config.data_endpoints is None else config.data_endpoints
 
-        if self.stats.num_rows > config.rows_per_split and config.num_splits is None:
-            config.num_splits = self.stats.num_rows // config.rows_per_split
-        log.debug(f"num_rows={self.stats.num_rows} rows_per_splits={config.rows_per_split} num_splits={config.num_splits} ")
+        if stats.num_rows > config.rows_per_split and config.num_splits is None:
+            config.num_splits = stats.num_rows // config.rows_per_split
+        log.debug(f"num_rows={stats.num_rows} rows_per_splits={config.rows_per_split} num_splits={config.num_splits} ")
+
+        if columns is None:
+            columns = [f.name for f in self.arrow_schema]
 
         query_schema = self.arrow_schema
         if internal_row_id:
             queried_fields = [pa.field(INTERNAL_ROW_ID, pa.uint64())]
             queried_fields.extend(column for column in self.arrow_schema)
             query_schema = pa.schema(queried_fields)
             columns.append(INTERNAL_ROW_ID)
 
-        query_data_request = build_query_data_request(
+        query_data_request = internal_commands.build_query_data_request(
             schema=query_schema,
             predicate=predicate,
             field_names=columns)
 
-        splits_queue = queue.Queue()
+        splits_queue: queue.Queue[int] = queue.Queue()
 
         for split in range(config.num_splits):
             splits_queue.put(split)
 
         # this queue shouldn't be large it is marely a pipe through which the results
         # are sent to the main thread. Most of the pages actually held in the
         # threads that fetch the pages.
-        record_batches_queue = queue.Queue(maxsize=2)
+        record_batches_queue: queue.Queue[pa.RecordBatch] = queue.Queue(maxsize=2)
+
         stop_event = Event()
+
         class StoppedException(Exception):
             pass
 
         def check_stop():
             if stop_event.is_set():
                 raise StoppedException
 
-        def single_endpoint_worker(endpoint : str):
+        def single_endpoint_worker(endpoint: str):
             try:
-                host_api = VastdbApi(endpoint=endpoint, access_key=self.tx._rpc.api.access_key, secret_key=self.tx._rpc.api.secret_key)
+                host_api = internal_commands.VastdbApi(endpoint=endpoint, access_key=self.tx._rpc.api.access_key, secret_key=self.tx._rpc.api.secret_key)
                 while True:
                     check_stop()
                     try:
                         split = splits_queue.get_nowait()
                     except queue.Empty:
                         log.debug("splits queue is empty")
                         break
@@ -289,30 +293,29 @@
                 log.debug("stop signal.", exc_info=True)
                 return
             finally:
                 # signal that this thread has ended
                 log.debug("exiting")
                 record_batches_queue.put(None)
 
-        # Take a snapshot of enpoints
-        endpoints = list(self.stats.endpoints) if config.data_endpoints is None else list(config.data_endpoints)
-
         def batches_iterator():
-            def propagate_first_exception(futures : List[concurrent.futures.Future], block = False):
+            def propagate_first_exception(futures: List[concurrent.futures.Future], block=False):
                 done, not_done = concurrent.futures.wait(futures, None if block else 0, concurrent.futures.FIRST_EXCEPTION)
+                if self.tx.txid is None:
+                    raise errors.MissingTransaction()
                 for future in done:
                     future.result()
                 return not_done
 
             threads_prefix = "query-data"
             # This is mainly for testing, it helps to identify running threads in runtime.
             if config.query_id:
                 threads_prefix = threads_prefix + "-" + config.query_id
 
-            with concurrent.futures.ThreadPoolExecutor(max_workers=len(endpoints), thread_name_prefix=threads_prefix) as tp: # TODO: concurrency == enpoints is just a heuristic
+            with concurrent.futures.ThreadPoolExecutor(max_workers=len(endpoints), thread_name_prefix=threads_prefix) as tp:  # TODO: concurrency == enpoints is just a heuristic
                 futures = [tp.submit(single_endpoint_worker, endpoint) for endpoint in endpoints]
                 tasks_running = len(futures)
                 try:
                     while tasks_running > 0:
                         futures = propagate_first_exception(futures, block=False)
 
                         batch = record_batches_queue.get()
@@ -336,24 +339,19 @@
         if hasattr(col, "combine_chunks"):
             return col.combine_chunks()
         else:
             return col
 
     def insert(self, rows: pa.RecordBatch) -> pa.RecordBatch:
         serialized_slices = self.tx._rpc.api._record_batch_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
-        row_ids = []
         for slice in serialized_slices:
-            res = self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
+            self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                                txid=self.tx.txid)
-            (batch,) = pa.RecordBatchStreamReader(res.raw)
-            row_ids.append(batch[INTERNAL_ROW_ID])
-
-        return pa.chunked_array(row_ids)
 
-    def update(self, rows: Union[pa.RecordBatch, pa.Table], columns: list = None) -> None:
+    def update(self, rows: Union[pa.RecordBatch, pa.Table], columns: Optional[List[str]] = None) -> None:
         if columns is not None:
             update_fields = [(INTERNAL_ROW_ID, pa.uint64())]
             update_values = [self._combine_chunks(rows[INTERNAL_ROW_ID])]
             for col in columns:
                 update_fields.append(rows.field(col))
                 update_values.append(self._combine_chunks(rows[col]))
 
@@ -413,15 +411,14 @@
 
 @dataclass
 class Projection:
     name: str
     table: Table
     handle: int
     stats: TableStats
-    properties: dict = None
 
     @property
     def bucket(self):
         return self.table.schema.bucket
 
     @property
     def schema(self):
@@ -434,15 +431,15 @@
     def __repr__(self):
         return f"{type(self).__name__}(name={self.name})"
 
     def columns(self) -> pa.Schema:
         columns = []
         next_key = 0
         while True:
-            curr_columns, next_key, is_truncated, count, _ = \
+            curr_columns, next_key, is_truncated, _count, _ = \
                 self.tx._rpc.api.list_projection_columns(
                     self.bucket.name, self.schema.name, self.table.name, self.name, txid=self.table.tx.txid, next_key=next_key)
             if not curr_columns:
                 break
             columns.extend(curr_columns)
             if not is_truncated:
                 break
@@ -463,17 +460,17 @@
 
 def _parse_projection_info(projection_info, table: "Table"):
     log.info("Projection info %s", str(projection_info))
     stats = TableStats(num_rows=projection_info.num_rows, size_in_bytes=projection_info.size_in_bytes)
     return Projection(name=projection_info.name, table=table, stats=stats, handle=int(projection_info.handle))
 
 
-def _parse_bucket_and_object_names(path: str) -> (str, str):
+def _parse_bucket_and_object_names(path: str) -> Tuple[str, str]:
     if not path.startswith('/'):
-        raise errors.InvalidArgumentError(f"Path {path} must start with a '/'")
+        raise errors.InvalidArgument(f"Path {path} must start with a '/'")
     components = path.split(os.path.sep)
     bucket_name = components[1]
     object_path = os.path.sep.join(components[2:])
     return bucket_name, object_path
 
 
 def _serialize_record_batch(record_batch: pa.RecordBatch) -> pa.lib.Buffer:
```

### Comparing `vastdb-0.1.1/vastdb/tests/test_imports.py` & `vastdb-0.1.2/vastdb/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vastdb/tests/test_nested.py` & `vastdb-0.1.2/vastdb/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.1/vastdb/tests/test_projections.py` & `vastdb-0.1.2/vastdb/tests/test_projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import pyarrow as pa
 
 log = logging.getLogger(__name__)
 
+
 def test_basic_projections(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         columns = pa.schema([
             ('a', pa.int8()),
             ('b', pa.int16()),
             ('c', pa.string()),
```

### Comparing `vastdb-0.1.1/vastdb/tests/test_sanity.py` & `vastdb-0.1.2/vastdb/tests/test_sanity.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,18 @@
             self.end_headers()
 
         def version_string(self):
             version = next(self.versions_iterator)[0]
             return f"vast {version}" if version else "vast"
 
         def log_message(self, format, *args):
-            log.debug(format,*args)
+            log.debug(format, *args)
 
     # start the server on localhost on some available port port
-    server_address =('localhost', 0)
+    server_address = ('localhost', 0)
     httpd = HTTPServer(server_address, MockOptionsHandler)
 
     def start_http_server_in_thread():
         log.info(f"Mock HTTP server is running on port {httpd.server_port}")
         httpd.serve_forever()
         log.info("Mock HTTP server killed")
```

### Comparing `vastdb-0.1.1/vastdb/tests/test_schemas.py` & `vastdb-0.1.2/vastdb/tests/test_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,19 @@
         # implicit commit
 
     with pytest.raises(ZeroDivisionError):
         with session.transaction() as tx:
             b = tx.bucket(clean_bucket_name)
             b.schema("s3").drop()
             assert b.schemas() == []
-            1/0  # rollback schema dropping
+            1 / 0  # rollback schema dropping
 
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         assert b.schemas() != []
 
+
 def test_list_snapshots(session, clean_bucket_name):
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         s = b.snapshots()
         assert s == []
```

### Comparing `vastdb-0.1.1/vastdb/tests/test_tables.py` & `vastdb-0.1.2/vastdb/tests/test_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import decimal
 import logging
 import random
 import threading
 from contextlib import closing
 from tempfile import NamedTemporaryFile
 
-import duckdb
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.parquet as pq
 import pytest
 from requests.exceptions import HTTPError
 
 from .. import errors
@@ -87,15 +86,14 @@
         assert s.tables() == [t]
         assert s.create_table('t', pa.schema([('y', pa.int64())]), fail_if_exists=False) == t
         assert s.tables() == [t]
         assert s.create_table('t', pa.schema([('x', pa.int64())]), fail_if_exists=False) == t
         assert s.tables() == [t]
 
 
-
 def test_update_table(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int64()),
         ('b', pa.float32()),
         ('s', pa.utf8()),
     ])
     expected = pa.table(schema=columns, data=[
@@ -143,20 +141,21 @@
         t.update(update_table.to_batches()[0], columns=['a'])
         actual = pa.Table.from_batches(t.select(columns=['a', 'b']))
         assert actual.to_pydict() == {
             'a': [111, 2222, 333],
             'b': [0.5, 1.5, 2.5]
         }
 
+
 def test_select_with_multisplits(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int32())
     ])
 
-    data = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+    data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
     data = data * 1000
     expected = pa.table(schema=columns, data=[data])
 
     config = QueryConfig()
     config.rows_per_split = 1000
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
@@ -175,23 +174,23 @@
         ('d', pa.decimal128(7, 3)),
         ('bin', pa.binary()),
         ('date', pa.date32()),
         ('t0', pa.time32('s')),
         ('t3', pa.time32('ms')),
         ('t6', pa.time64('us')),
         ('t9', pa.time64('ns')),
-        ('ts0' ,pa.timestamp('s')),
-        ('ts3' ,pa.timestamp('ms')),
-        ('ts6' ,pa.timestamp('us')),
-        ('ts9' ,pa.timestamp('ns')),
+        ('ts0', pa.timestamp('s')),
+        ('ts3', pa.timestamp('ms')),
+        ('ts6', pa.timestamp('us')),
+        ('ts9', pa.timestamp('ns')),
     ])
 
     expected = pa.table(schema=columns, data=[
         [True, True, False],
-        [1 , 2, 4],
+        [1, 2, 4],
         [1999, 2000, 2001],
         [11122221, 222111122, 333333],
         [0.5, 1.5, 2.5],
         ["a", "v", "s"],
         [decimal.Decimal('110.52'), decimal.Decimal('231.15'), decimal.Decimal('3332.44')],
         [b"\x01\x02", b"\x01\x05", b"\x01\x07"],
         [dt.date(2024, 4, 10), dt.date(2024, 4, 11), dt.date(2024, 4, 12)],
@@ -291,45 +290,25 @@
         assert select((t['a'] > 111) & (t['b'] < 2.5)) == expected.filter((pc.field('a') > 111) & (pc.field('b') < 2.5))
         assert select((t['a'] > 111) & (t['a'] < 333)) == expected.filter((pc.field('a') > 111) & (pc.field('a') < 333))
 
         assert select((t['a'] > 111) | (t['a'] < 333)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333))
         assert select(((t['a'] > 111) | (t['a'] < 333)) & (t['b'] < 2.5)) == expected.filter(((pc.field('a') > 111) | (pc.field('a') < 333)) & (pc.field('b') < 2.5))
         with pytest.raises(NotImplementedError):
             assert select((t['a'] > 111) | (t['b'] > 0) | (t['s'] < 'ccc')) == expected.filter((pc.field('a') > 111) | (pc.field('b') > 0) | (pc.field('s') < 'ccc'))
-        assert select((t['a'] > 111) | (t['a'] < 333) | (t['a'] == 777) ) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333) | (pc.field('a') == 777))
+        assert select((t['a'] > 111) | (t['a'] < 333) | (t['a'] == 777)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333) | (pc.field('a') == 777))
 
         assert select(t['s'].isnull()) == expected.filter(pc.field('s').is_null())
         assert select((t['s'].isnull()) | (t['s'] == 'bb'))  == expected.filter((pc.field('s').is_null()) | (pc.field('s') == 'bb'))
         assert select((t['s'].isnull()) & (t['b'] == 3.5))  == expected.filter((pc.field('s').is_null()) & (pc.field('b') == 3.5))
 
         assert select(~t['s'].isnull()) == expected.filter(~pc.field('s').is_null())
         assert select(t['s'].contains('b')) == expected.filter(pc.field('s') == 'bb')
         assert select(t['s'].contains('y')) == expected.filter(pc.field('s') == 'xyz')
 
 
-def test_duckdb(session, clean_bucket_name):
-    columns = pa.schema([
-        ('a', pa.int32()),
-        ('b', pa.float64()),
-    ])
-    data = pa.table(schema=columns, data=[
-        [111, 222, 333],
-        [0.5, 1.5, 2.5],
-    ])
-    with prepare_data(session, clean_bucket_name, 's', 't', data) as t:
-        conn = duckdb.connect()
-        batches = t.select(columns=['a'], predicate=(t['b'] < 2))  # noqa: F841
-        actual = conn.execute('SELECT max(a) as "a_max" FROM batches').arrow()
-        expected = (data
-            .filter(pc.field('b') < 2)
-            .group_by([])
-            .aggregate([('a', 'max')]))
-        assert actual == expected
-
-
 def test_parquet_export(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         columns = pa.schema([
             ('a', pa.int16()),
             ('b', pa.float32()),
             ('s', pa.utf8()),
@@ -340,29 +319,29 @@
 
         rb = pa.record_batch(schema=columns, data=[
             [111, 222],
             [0.5, 1.5],
             ['a', 'b'],
         ])
         expected = pa.Table.from_batches([rb])
-        rb = t.insert(rb)
-        assert rb.to_pylist() == [0, 1]
+        t.insert(rb)
         actual = pa.Table.from_batches(t.select())
         assert actual == expected
 
         table_batches = t.select()
 
         with NamedTemporaryFile() as parquet_file:
             log.info("Writing table into parquet file: '%s'", parquet_file.name)
             with closing(pq.ParquetWriter(parquet_file.name, table_batches.schema)) as parquet_writer:
                 for batch in table_batches:
                     parquet_writer.write_batch(batch)
 
             assert expected == pq.read_table(parquet_file.name)
 
+
 def test_errors(session, clean_bucket_name):
     with pytest.raises(errors.MissingSchema):
         with session.transaction() as tx:
             tx.bucket(clean_bucket_name).schema('s1')
 
     with pytest.raises(errors.MissingBucket):
         with session.transaction() as tx:
@@ -374,15 +353,16 @@
             s = b.create_schema('s1')
             columns = pa.schema([
                 ('a', pa.int16()),
                 ('b', pa.float32()),
                 ('s', pa.utf8()),
             ])
             s.create_table('t1', columns)
-            s.drop() # cannot drop schema without dropping its tables first
+            s.drop()  # cannot drop schema without dropping its tables first
+
 
 def test_rename_schema(session, clean_bucket_name):
 
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s')
 
     with session.transaction() as tx, session.transaction() as tx2:
@@ -432,28 +412,29 @@
         # assert that the new table name is seen in the context
         # in which it was renamed
         assert t.name == 't2'
         with pytest.raises(errors.MissingTable):
             s.table('t')
         t = s.table('t2')
 
-        #assert that other transactions are isolated
+        # assert that other transactions are isolated
         with pytest.raises(errors.MissingTable):
             tx2.bucket(clean_bucket_name).schema('s').table('t2')
         tx2.bucket(clean_bucket_name).schema('s').table('t')
 
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
-        #assert that new transactions see the change
+        # assert that new transactions see the change
         with pytest.raises(errors.MissingTable):
             s.table('t')
         t = s.table('t2')
         t.drop()
         s.drop()
 
+
 def test_add_column(session, clean_bucket_name):
     columns = pa.schema([
             ('a', pa.int16()),
             ('b', pa.float32()),
             ('s', pa.utf8()),
         ])
     new_column = pa.field('aa', pa.int16())
@@ -468,26 +449,26 @@
         assert t.arrow_schema == columns
 
         t.add_column(pa.schema([new_column]))
         # assert that the column is seen in the context
         # in which it was added
         assert t.arrow_schema == new_schema
 
-        #assert that other transactions are isolated
+        # assert that other transactions are isolated
         assert tx2.bucket(clean_bucket_name).schema('s').table('t').arrow_schema == columns
 
-
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
         t = s.table('t')
-        #assert that new transactions see the change
+        # assert that new transactions see the change
         assert t.arrow_schema == new_schema
         t.drop()
         s.drop()
 
+
 def test_drop_column(session, clean_bucket_name):
     columns = pa.schema([
             ('a', pa.int16()),
             ('b', pa.float32()),
             ('s', pa.utf8()),
         ])
     field_idx = columns.get_field_index('a')
@@ -503,72 +484,73 @@
         assert t.arrow_schema == columns
 
         t.drop_column(pa.schema([column_to_drop]))
         # assert that the column is seen in the context
         # in which it was added
         assert t.arrow_schema == new_schema
 
-        #assert that other transactions are isolated
+        # assert that other transactions are isolated
         assert tx2.bucket(clean_bucket_name).schema('s').table('t').arrow_schema == columns
 
-
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
         t = s.table('t')
-        #assert that new transactions see the change
+        # assert that new transactions see the change
         assert t.arrow_schema == new_schema
         t.drop()
         s.drop()
 
+
 def test_rename_column(session, clean_bucket_name):
     columns = pa.schema([
             ('a', pa.int16()),
             ('b', pa.float32()),
             ('s', pa.utf8()),
         ])
-    def prepare_rename_column(schema : pa.Schema, old_name : str, new_name : str) -> pa.Schema:
+
+    def prepare_rename_column(schema: pa.Schema, old_name: str, new_name: str) -> pa.Schema:
         field_idx = schema.get_field_index(old_name)
         column_to_rename = schema.field(field_idx)
         renamed_column = column_to_rename.with_name(new_name)
         return schema.set(field_idx, renamed_column)
 
-    new_schema = prepare_rename_column(columns,'a','aaa')
+    new_schema = prepare_rename_column(columns, 'a', 'aaa')
 
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s')
         s.create_table('t', columns)
 
     with session.transaction() as tx, session.transaction() as tx2:
         t = tx.bucket(clean_bucket_name).schema('s').table('t')
         assert t.arrow_schema == columns
 
         t.rename_column('a', 'aaa')
         # assert that the column is seen in the context
         # in which it was added
         assert t.arrow_schema == new_schema
 
-        #assert that other transactions are isolated
+        # assert that other transactions are isolated
         assert tx2.bucket(clean_bucket_name).schema('s').table('t').arrow_schema == columns
 
-    #assert that new transactions see the change
+    # assert that new transactions see the change
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
         t = s.table('t')
 
         assert t.arrow_schema == new_schema
 
     # simultaneos renames of the same column
     new_schema_tx1 = prepare_rename_column(new_schema, 'b', 'bb')
     new_schema_tx2 = prepare_rename_column(new_schema, 'b', 'bbb')
     with pytest.raises(errors.Conflict):
         with session.transaction() as tx1, session.transaction() as tx2:
             t1 = tx1.bucket(clean_bucket_name).schema('s').table('t')
             t2 = tx2.bucket(clean_bucket_name).schema('s').table('t')
             t1.rename_column('b', 'bb')
-            with pytest.raises(HTTPError, match = '409 Client Error: Conflict'):
+            with pytest.raises(HTTPError, match='409 Client Error: Conflict'):
                 t2.rename_column('b', 'bbb')
 
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
         t = s.table('t')
         # validate that the rename conflicted and rolled back
         assert (t.arrow_schema != new_schema_tx1) and \
@@ -576,14 +558,15 @@
 
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).schema('s')
         t = s.table('t')
         t.drop()
         s.drop()
 
+
 def test_select_stop(session, clean_bucket_name):
     columns = pa.schema([
             ('a', pa.uint8()),
         ])
 
     rb = pa.record_batch(schema=columns, data=[
             list(range(256)),
@@ -598,23 +581,24 @@
 
     num_rows = 2**8
 
     ROWS_PER_GROUP = 2**16
     qc = QueryConfig(num_sub_splits=2, num_splits=4, num_row_groups_per_sub_split=1)
     with session.transaction() as tx:
         t = tx.bucket(clean_bucket_name).schema('s').table('t')
-        t.refresh_stats()
-        qc.data_endpoints = list(t.stats.endpoints) * 2
+        qc.data_endpoints = list(t.get_stats().endpoints) * 2
 
     # Duplicate the table until it is large enough to generate enough batches
     while num_rows < (qc.num_sub_splits * qc.num_splits) * ROWS_PER_GROUP:
+        # We need two separate transactions to prevent an infinite loop that may happen
+        # while appending and reading the same table using a single transaction.
         with session.transaction() as tx_read, session.transaction() as tx_write:
             t_read = tx_read.bucket(clean_bucket_name).schema('s').table('t')
             t_write = tx_write.bucket(clean_bucket_name).schema('s').table('t')
-            for batch in t_read.select(['a'],config=qc):
+            for batch in t_read.select(['a'], config=qc):
                 t_write.insert(batch)
         num_rows = num_rows * 2
         log.info("Num rows: %d", num_rows)
 
     # Validate the number of batches and the number of rows
     read_rows = 0
     read_batches = 0
@@ -623,19 +607,20 @@
         for batch in t.select(['a'], config=qc):
             read_batches += 1
             read_rows += len(batch)
     assert read_rows == num_rows
     # If this assert triggers it just means that the test assumptions about how
     # the tabular server splits the batches is not true anymore and we need to
     # rewrite the test.
-    assert read_batches == qc.num_splits*qc.num_sub_splits
-    qc.query_id = str(random.randint(0,2**32))
+    assert read_batches == qc.num_splits * qc.num_sub_splits
+    qc.query_id = str(random.randint(0, 2**32))
     log.info("query id is: %s", qc.query_id)
+
     def active_threads():
-        log.debug("%s",[t.getName() for t in threading.enumerate() if t.is_alive()])
+        log.debug("%s", [t.getName() for t in threading.enumerate() if t.is_alive()])
         return sum([1 if t.is_alive() and qc.query_id in t.getName() else 0 for t in threading.enumerate()])
 
     assert active_threads() == 0
 
     with session.transaction() as tx:
         t = tx.bucket(clean_bucket_name).schema('s').table('t')
         batches = iter(t.select(['a'], config=qc))
```

### Comparing `vastdb-0.1.1/vastdb/transaction.py` & `vastdb-0.1.2/vastdb/transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,43 +4,47 @@
 
     with session.transaction() as tx:
         tx.bucket("bucket").create_schema("schema")
 """
 
 import logging
 from dataclasses import dataclass
+from typing import Optional
 
 import botocore
 
-from . import bucket, errors, session
+from . import bucket, errors, schema, session, table
 
 log = logging.getLogger(__name__)
 
+
 @dataclass
 class Transaction:
     """A holder of a single VAST transaction."""
 
     _rpc: "session.Session"
-    txid: int = None
+    txid: Optional[int] = None
 
     def __enter__(self):
         """Create a transaction and store its ID."""
         response = self._rpc.api.begin_transaction()
         self.txid = int(response.headers['tabular-txid'])
         log.debug("opened txid=%016x", self.txid)
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         """On success, the transaction is committed. Otherwise, it is rolled back."""
+        txid = self.txid
+        self.txid = None
         if (exc_type, exc_value, exc_traceback) == (None, None, None):
-            log.debug("committing txid=%016x", self.txid)
-            self._rpc.api.commit_transaction(self.txid)
+            log.debug("committing txid=%016x", txid)
+            self._rpc.api.commit_transaction(txid)
         else:
-            log.exception("rolling back txid=%016x due to:", self.txid)
-            self._rpc.api.rollback_transaction(self.txid)
+            log.exception("rolling back txid=%016x due to:", txid)
+            self._rpc.api.rollback_transaction(txid)
 
     def __repr__(self):
         """Don't show the session details."""
         return f'Transaction(id=0x{self.txid:016x})'
 
     def bucket(self, name: str) -> "bucket.Bucket":
         """Return a VAST Bucket, if exists."""
@@ -48,7 +52,13 @@
             self._rpc.s3.head_bucket(Bucket=name)
         except botocore.exceptions.ClientError as e:
             log.warning("res: %s", e.response)
             if e.response['Error']['Code'] == '404':
                 raise errors.MissingBucket(name)
             raise
         return bucket.Bucket(name, self)
+
+    def catalog(self, fail_if_missing=True) -> Optional["table.Table"]:
+        """Return VAST Catalog table."""
+        b = bucket.Bucket("vast-big-catalog-bucket", self)
+        s = schema.Schema("vast_big_catalog_schema", b)
+        return s.table(name="vast_big_catalog_table", fail_if_missing=fail_if_missing)
```

### Comparing `vastdb-0.1.1/vastdb/util.py` & `vastdb-0.1.2/vastdb/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
-from typing import Callable
+from typing import Callable, List, Optional
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 from .errors import InvalidArgument
 from .schema import Schema
 from .table import ImportConfig, Table
 
 log = logging.getLogger(__name__)
 
 
 def create_table_from_files(
-        schema: Schema, table_name: str, parquet_files: [str], schema_merge_func: Callable = None,
-        config: ImportConfig = None) -> Table:
+        schema: Schema, table_name: str, parquet_files: List[str],
+        schema_merge_func: Optional[Callable] = None,
+        config: Optional[ImportConfig] = None) -> Table:
     if not schema_merge_func:
         schema_merge_func = default_schema_merge
     else:
         assert schema_merge_func in [default_schema_merge, strict_schema_merge, union_schema_merge]
     tx = schema.tx
     current_schema = pa.schema([])
     s3fs = pa.fs.S3FileSystem(
```

### Comparing `vastdb-0.1.1/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.2/vastdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 vastdb.egg-info/SOURCES.txt
 vastdb.egg-info/dependency_links.txt
 vastdb.egg-info/requires.txt
 vastdb.egg-info/top_level.txt
 vastdb/bench/__init__.py
 vastdb/bench/test_perf.py
 vastdb/tests/__init__.py
+vastdb/tests/test_duckdb.py
 vastdb/tests/test_imports.py
 vastdb/tests/test_nested.py
 vastdb/tests/test_projections.py
 vastdb/tests/test_sanity.py
 vastdb/tests/test_schemas.py
 vastdb/tests/test_tables.py
 vastdb/tests/util.py
```

