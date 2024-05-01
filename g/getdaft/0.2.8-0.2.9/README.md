# Comparing `tmp/getdaft-0.2.8.tar.gz` & `tmp/getdaft-0.2.9.tar.gz`

## Comparing `getdaft-0.2.8.tar` & `getdaft-0.2.9.tar`

### file list

```diff
@@ -1,769 +1,769 @@
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-dsl/Cargo.toml
--rw-r--r--   0      501       20      273 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/README.md
--rw-r--r--   0      501       20     1454 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/arithmetic.rs
--rw-r--r--   0      501       20    24007 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/expr.rs
--rw-r--r--   0      501       20     1479 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
--rw-r--r--   0      501       20      592 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/float/mod.rs
--rw-r--r--   0      501       20     2731 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/crop.rs
--rw-r--r--   0      501       20     1353 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/decode.rs
--rw-r--r--   0      501       20     1790 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/encode.rs
--rw-r--r--   0      501       20     1586 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/mod.rs
--rw-r--r--   0      501       20     2524 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/resize.rs
--rw-r--r--   0      501       20     1033 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/explode.rs
--rw-r--r--   0      501       20     2359 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/join.rs
--rw-r--r--   0      501       20     1493 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/lengths.rs
--rw-r--r--   0      501       20     1151 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/mod.rs
--rw-r--r--   0      501       20     2251 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/mod.rs
--rw-r--r--   0      501       20     1197 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
--rw-r--r--   0      501       20      585 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
--rw-r--r--   0      501       20     2208 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/partitioning/evaluators.rs
--rw-r--r--   0      501       20     1389 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/partitioning/mod.rs
--rw-r--r--   0      501       20      694 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/mod.rs
--rw-r--r--   0      501       20     2565 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2793 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/udf.rs
--rw-r--r--   0      501       20     1347 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/date.rs
--rw-r--r--   0      501       20     1344 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs
--rw-r--r--   0      501       20     1373 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1349 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/hour.rs
--rw-r--r--   0      501       20     1925 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1355 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs
--rw-r--r--   0      501       20     1349 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs
--rw-r--r--   0      501       20     2317 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/uri/download.rs
--rw-r--r--   0      501       20     1084 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs
--rw-r--r--   0      501       20     1652 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1651 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1370 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs
--rw-r--r--   0      501       20     1812 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1659 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/split.rs
--rw-r--r--   0      501       20     1661 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
--rw-r--r--   0      501       20      920 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/lib.rs
--rw-r--r--   0      501       20     7739 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/lit.rs
--rw-r--r--   0      501       20     2097 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/optimization.rs
--rw-r--r--   0      501       20     2508 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/pyobject.rs
--rw-r--r--   0      501       20    12025 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/python.rs
--rw-r--r--   0      501       20     3729 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-dsl/src/treenode.rs
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/common-error/Cargo.toml
--rw-r--r--   0      501       20     3650 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-error/src/error.rs
--rw-r--r--   0      501       20       64 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-error/src/lib.rs
--rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-core/Cargo.toml
--rw-r--r--   0      501       20      191 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/boolean.rs
--rw-r--r--   0      501       20     6283 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/fixed_size_list_array.rs
--rw-r--r--   0      501       20     6935 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/from.rs
--rw-r--r--   0      501       20     1327 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/from_iter.rs
--rw-r--r--   0      501       20     6419 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/arrow_growable.rs
--rw-r--r--   0      501       20     1216 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/bitmap_growable.rs
--rw-r--r--   0      501       20     3013 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/fixed_size_list_growable.rs
--rw-r--r--   0      501       20     3655 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/list_growable.rs
--rw-r--r--   0      501       20     3075 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/logical_growable.rs
--rw-r--r--   0      501       20     7888 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/mod.rs
--rw-r--r--   0      501       20     2027 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/python_growable.rs
--rw-r--r--   0      501       20     3336 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/struct_growable.rs
--rw-r--r--   0      501       20      734 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/iterator.rs
--rw-r--r--   0      501       20     4907 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/list_array.rs
--rw-r--r--   0      501       20     3325 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/mod.rs
--rw-r--r--   0      501       20      269 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/abs.rs
--rw-r--r--   0      501       20      738 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/apply.rs
--rw-r--r--   0      501       20      860 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arange.rs
--rw-r--r--   0      501       20     7353 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3055 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     2031 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20     3084 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    75218 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/cast.rs
--rw-r--r--   0      501       20    13907 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    57653 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     4259 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/concat.rs
--rw-r--r--   0      501       20    10434 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     4566 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/count.rs
--rw-r--r--   0      501       20     5502 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/date.rs
--rw-r--r--   0      501       20     4086 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1271 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/float.rs
--rw-r--r--   0      501       20     5357 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/from_arrow.rs
--rw-r--r--   0      501       20     8630 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/full.rs
--rw-r--r--   0      501       20     7191 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/get.rs
--rw-r--r--   0      501       20     4408 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1861 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/hash.rs
--rw-r--r--   0      501       20     5304 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/if_else.rs
--rw-r--r--   0      501       20    33802 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/image.rs
--rw-r--r--   0      501       20     2197 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/len.rs
--rw-r--r--   0      501       20     6189 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/list.rs
--rw-r--r--   0      501       20     4344 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1730 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2756 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/mod.rs
--rw-r--r--   0      501       20     3127 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/null.rs
--rw-r--r--   0      501       20     3826 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20    13502 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/repr.rs
--rw-r--r--   0      501       20      491 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    20392 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2396 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/sum.rs
--rw-r--r--   0      501       20     7379 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/take.rs
--rw-r--r--   0      501       20      456 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/tensor.rs
--rw-r--r--   0      501       20     9823 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13618 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2490 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20     6545 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/serdes.rs
--rw-r--r--   0      501       20     4986 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/array/struct_array.rs
--rw-r--r--   0      501       20     2294 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/count_mode.rs
--rw-r--r--   0      501       20    11287 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/binary_ops.rs
--rw-r--r--   0      501       20    17006 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     3661 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/field.rs
--rw-r--r--   0      501       20     3153 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/image_format.rs
--rw-r--r--   0      501       20     6404 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/image_mode.rs
--rw-r--r--   0      501       20     5835 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/logical.rs
--rw-r--r--   0      501       20     8852 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/matching.rs
--rw-r--r--   0      501       20     9276 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1041 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20     6039 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/kernels/mod.rs
--rw-r--r--   0      501       20    14629 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3905 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/kernels/utf8.rs
--rw-r--r--   0      501       20      832 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/lib.rs
--rw-r--r--   0      501       20    11194 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/python/datatype.rs
--rw-r--r--   0      501       20     1098 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/python/field.rs
--rw-r--r--   0      501       20      610 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/python/mod.rs
--rw-r--r--   0      501       20     2278 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/python/schema.rs
--rw-r--r--   0      501       20    15815 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/python/series.rs
--rw-r--r--   0      501       20     6524 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/schema.rs
--rw-r--r--   0      501       20    10715 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs
--rw-r--r--   0      501       20     7955 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     8237 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      220 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     6396 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/nested_array.rs
--rw-r--r--   0      501       20     1984 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/from.rs
--rw-r--r--   0      501       20     2875 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/mod.rs
--rw-r--r--   0      501       20      910 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5355 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/agg.rs
--rw-r--r--   0      501       20     3462 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1967 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      205 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/cast.rs
--rw-r--r--   0      501       20      682 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1173 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/concat.rs
--rw-r--r--   0      501       20     3694 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/date.rs
--rw-r--r--   0      501       20     2415 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      693 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/filter.rs
--rw-r--r--   0      501       20      440 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/float.rs
--rw-r--r--   0      501       20      468 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/groups.rs
--rw-r--r--   0      501       20      445 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/hash.rs
--rw-r--r--   0      501       20      324 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/if_else.rs
--rw-r--r--   0      501       20     3250 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/image.rs
--rw-r--r--   0      501       20      297 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/len.rs
--rw-r--r--   0      501       20     1994 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/list.rs
--rw-r--r--   0      501       20     2563 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/mod.rs
--rw-r--r--   0      501       20      477 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/not.rs
--rw-r--r--   0      501       20      160 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/null.rs
--rw-r--r--   0      501       20     4081 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/partitioning.rs
--rw-r--r--   0      501       20      703 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1562 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/sort.rs
--rw-r--r--   0      501       20      704 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/take.rs
--rw-r--r--   0      501       20     1856 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/utf8.rs
--rw-r--r--   0      501       20    13838 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/serdes.rs
--rw-r--r--   0      501       20     2333 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/series/series_like.rs
--rw-r--r--   0      501       20     5474 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/utils/arrow.rs
--rw-r--r--   0      501       20     6787 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/utils/display_table.rs
--rw-r--r--   0      501       20      582 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/utils/hashable_float_wrapper.rs
--rw-r--r--   0      501       20     1267 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/utils/mod.rs
--rw-r--r--   0      501       20     9991 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-json/Cargo.toml
--rw-r--r--   0      501       20    20709 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/decoding.rs
--rw-r--r--   0      501       20     8265 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/inference.rs
--rw-r--r--   0      501       20     2159 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/lib.rs
--rw-r--r--   0      501       20     6287 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/options.rs
--rw-r--r--   0      501       20     2212 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/python.rs
--rw-r--r--   0      501       20    46050 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/read.rs
--rw-r--r--   0      501       20    15346 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/src/schema.rs
--rw-r--r--   0      501       20     1130 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/dtypes.jsonl
--rw-r--r--   0      501       20     2000 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl
--rw-r--r--   0      501       20      176 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.br
--rw-r--r--   0      501       20      228 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.bz2
--rw-r--r--   0      501       20      258 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.gz
--rw-r--r--   0      501       20      202 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.lzma
--rw-r--r--   0      501       20      248 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.xz
--rw-r--r--   0      501       20      230 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.zl
--rw-r--r--   0      501       20      228 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl.zst
--rw-r--r--   0      501       20      606 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny_all_null_column.jsonl
--rw-r--r--   0      501       20      199 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny_conflicting_dtypes.jsonl
--rw-r--r--   0      501       20      600 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny_nulls.jsonl
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-parquet/Cargo.toml
--rw-r--r--   0      501       20    29429 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/file.rs
--rw-r--r--   0      501       20     5359 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/lib.rs
--rw-r--r--   0      501       20     3537 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/metadata.rs
--rw-r--r--   0      501       20     9787 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/python.rs
--rw-r--r--   0      501       20    23584 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/read.rs
--rw-r--r--   0      501       20     9080 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/read_planner.rs
--rw-r--r--   0      501       20    16750 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/column_range.rs
--rw-r--r--   0      501       20     1506 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/mod.rs
--rw-r--r--   0      501       20     1950 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/table_stats.rs
--rw-r--r--   0      501       20     1586 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/utils.rs
--rw-r--r--   0      501       20     8638 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-parquet/src/stream_reader.rs
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-decoding/Cargo.toml
--rw-r--r--   0      501       20    13365 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-decoding/src/deserialize.rs
--rw-r--r--   0      501       20     3958 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-decoding/src/inference.rs
--rw-r--r--   0      501       20      151 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-decoding/src/lib.rs
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-io/Cargo.toml
--rw-r--r--   0      501       20    21636 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/azure_blob.rs
--rw-r--r--   0      501       20    13465 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/google_cloud.rs
--rw-r--r--   0      501       20    12872 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/http.rs
--rw-r--r--   0      501       20    15481 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/lib.rs
--rw-r--r--   0      501       20    15641 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/local.rs
--rw-r--r--   0      501       20     4445 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/object_io.rs
--rw-r--r--   0      501       20    27058 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/object_store_glob.rs
--rw-r--r--   0      501       20     2592 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/python.rs
--rw-r--r--   0      501       20    37315 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/s3_like.rs
--rw-r--r--   0      501       20     3138 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/stats.rs
--rw-r--r--   0      501       20      801 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-io/src/stream_utils.rs
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/common-daft-config/Cargo.toml
--rw-r--r--   0      501       20     1915 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-daft-config/src/lib.rs
--rw-r--r--   0      501       20     4347 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-daft-config/src/python.rs
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/Cargo.toml
--rw-r--r--   0      501       20     1436 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/lib.rs
--rw-r--r--   0      501       20    34909 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/micropartition.rs
--rw-r--r--   0      501       20     1066 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/agg.rs
--rw-r--r--   0      501       20     1526 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/cast_to_schema.rs
--rw-r--r--   0      501       20     1816 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/concat.rs
--rw-r--r--   0      501       20     3229 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/eval_expressions.rs
--rw-r--r--   0      501       20     1465 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/filter.rs
--rw-r--r--   0      501       20     2255 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/join.rs
--rw-r--r--   0      501       20      131 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/mod.rs
--rw-r--r--   0      501       20     3355 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/partition.rs
--rw-r--r--   0      501       20     1829 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/slice.rs
--rw-r--r--   0      501       20     1390 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/sort.rs
--rw-r--r--   0      501       20     2671 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/take.rs
--rw-r--r--   0      501       20    24470 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-micropartition/src/python.rs
--rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-plan/Cargo.toml
--rw-r--r--   0      501       20    15953 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/builder.rs
--rw-r--r--   0      501       20     4444 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/display.rs
--rw-r--r--   0      501       20     2084 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/join.rs
--rw-r--r--   0      501       20     1774 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/lib.rs
--rw-r--r--   0      501       20     2433 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/agg.rs
--rw-r--r--   0      501       20      890 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/concat.rs
--rw-r--r--   0      501       20      275 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/distinct.rs
--rw-r--r--   0      501       20     1583 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/explode.rs
--rw-r--r--   0      501       20      942 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/filter.rs
--rw-r--r--   0      501       20     5244 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/join.rs
--rw-r--r--   0      501       20      550 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/limit.rs
--rw-r--r--   0      501       20      436 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/mod.rs
--rw-r--r--   0      501       20    18977 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/project.rs
--rw-r--r--   0      501       20     1614 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/repartition.rs
--rw-r--r--   0      501       20     1950 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/sink.rs
--rw-r--r--   0      501       20     2409 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/sort.rs
--rw-r--r--   0      501       20     2820 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/source.rs
--rw-r--r--   0      501       20    11763 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/logical_plan.rs
--rw-r--r--   0      501       20     8286 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/logical_plan_tracker.rs
--rw-r--r--   0      501       20      111 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/mod.rs
--rw-r--r--   0      501       20    22700 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/optimizer.rs
--rw-r--r--   0      501       20     3718 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/drop_repartition.rs
--rw-r--r--   0      501       20      333 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/mod.rs
--rw-r--r--   0      501       20    29770 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_filter.rs
--rw-r--r--   0      501       20    14914 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_limit.rs
--rw-r--r--   0      501       20    30117 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_projection.rs
--rw-r--r--   0      501       20     2301 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/rule.rs
--rw-r--r--   0      501       20     2675 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/partitioning.rs
--rw-r--r--   0      501       20      638 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/agg.rs
--rw-r--r--   0      501       20      840 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/broadcast_join.rs
--rw-r--r--   0      501       20      530 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/coalesce.rs
--rw-r--r--   0      501       20      396 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/concat.rs
--rw-r--r--   0      501       20     1292 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/csv.rs
--rw-r--r--   0      501       20      448 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/empty_scan.rs
--rw-r--r--   0      501       20      418 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/explode.rs
--rw-r--r--   0      501       20     1367 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/fanout.rs
--rw-r--r--   0      501       20      447 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/filter.rs
--rw-r--r--   0      501       20      331 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/flatten.rs
--rw-r--r--   0      501       20      724 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/hash_join.rs
--rw-r--r--   0      501       20      610 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/in_memory.rs
--rw-r--r--   0      501       20     1296 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/json.rs
--rw-r--r--   0      501       20      573 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/limit.rs
--rw-r--r--   0      501       20      955 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/mod.rs
--rw-r--r--   0      501       20     1330 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/parquet.rs
--rw-r--r--   0      501       20    11110 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/project.rs
--rw-r--r--   0      501       20      339 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/reduce.rs
--rw-r--r--   0      501       20      475 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/scan.rs
--rw-r--r--   0      501       20      635 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/sort.rs
--rw-r--r--   0      501       20      582 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/split.rs
--rw-r--r--   0      501       20    32052 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/physical_plan.rs
--rw-r--r--   0      501       20    33623 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/planner.rs
--rw-r--r--   0      501       20     3710 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/resource_request.rs
--rw-r--r--   0      501       20      873 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/sink_info.rs
--rw-r--r--   0      501       20     5242 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/source_info/file_info.rs
--rw-r--r--   0      501       20     3846 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/source_info/mod.rs
--rw-r--r--   0      501       20     1919 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-plan/src/test/mod.rs
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/common-treenode/Cargo.toml
--rw-r--r--   0      501       20    11886 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-treenode/src/lib.rs
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/common-io-config/Cargo.toml
--rw-r--r--   0      501       20      631 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/azure.rs
--rw-r--r--   0      501       20      560 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/config.rs
--rw-r--r--   0      501       20      536 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/gcs.rs
--rw-r--r--   0      501       20      170 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/lib.rs
--rw-r--r--   0      501       20    15730 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/python.rs
--rw-r--r--   0      501       20     2437 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/common-io-config/src/s3.rs
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-csv/Cargo.toml
--rw-r--r--   0      501       20     1940 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/compression.rs
--rw-r--r--   0      501       20     2179 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/lib.rs
--rw-r--r--   0      501       20    21037 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/metadata.rs
--rw-r--r--   0      501       20    10370 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/options.rs
--rw-r--r--   0      501       20     2104 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/python.rs
--rw-r--r--   0      501       20    58138 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/read.rs
--rw-r--r--   0      501       20     1396 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/src/schema.rs
--rw-r--r--   0      501       20      536 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv
--rw-r--r--   0      501       20      161 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.br
--rw-r--r--   0      501       20      193 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.bz2
--rw-r--r--   0      501       20      177 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.deflate
--rw-r--r--   0      501       20      205 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.gz
--rw-r--r--   0      501       20      183 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.lzma
--rw-r--r--   0      501       20      228 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.xz
--rw-r--r--   0      501       20      179 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.zl
--rw-r--r--   0      501       20      201 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv.zst
--rw-r--r--   0      501       20      191 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_all_null_column.csv
--rw-r--r--   0      501       20      536 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_bar_delimiter.csv
--rw-r--r--   0      501       20      533 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_comment.csv
--rw-r--r--   0      501       20      121 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_conflicting_dtypes.csv
--rw-r--r--   0      501       20      551 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_double_quote.csv
--rw-r--r--   0      501       20      140 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_empty_lines.csv
--rw-r--r--   0      501       20      548 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_escape.csv
--rw-r--r--   0      501       20      111 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_invalid_header_cols_mismatch.csv
--rw-r--r--   0      501       20       54 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_invalid_no_header_variable_num_cols.csv
--rw-r--r--   0      501       20      468 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_no_headers.csv
--rw-r--r--   0      501       20      190 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_nulls.csv
--rw-r--r--   0      501       20      536 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_single_quote.csv
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-table/Cargo.toml
--rw-r--r--   0      501       20     2798 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ffi.rs
--rw-r--r--   0      501       20    19163 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/lib.rs
--rw-r--r--   0      501       20     2168 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/agg.rs
--rw-r--r--   0      501       20     3750 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/explode.rs
--rw-r--r--   0      501       20     4402 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/groups.rs
--rw-r--r--   0      501       20     2898 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/hash.rs
--rw-r--r--   0      501       20     2631 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     6068 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/joins/mod.rs
--rw-r--r--   0      501       20      134 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/mod.rs
--rw-r--r--   0      501       20     3478 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/partition.rs
--rw-r--r--   0      501       20     1808 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/search_sorted.rs
--rw-r--r--   0      501       20      998 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/ops/sort.rs
--rw-r--r--   0      501       20    11273 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-table/src/python.rs
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-compression/Cargo.toml
--rw-r--r--   0      501       20     1940 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-compression/src/compression.rs
--rw-r--r--   0      501       20      108 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-compression/src/lib.rs
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-stats/Cargo.toml
--rw-r--r--   0      501       20     1490 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/arithmetic.rs
--rw-r--r--   0      501       20     6868 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/comparison.rs
--rw-r--r--   0      501       20     2363 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/logical.rs
--rw-r--r--   0      501       20    10073 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/mod.rs
--rw-r--r--   0      501       20     1184 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/lib.rs
--rw-r--r--   0      501       20      946 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/partition_spec.rs
--rw-r--r--   0      501       20      138 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/table_metadata.rs
--rw-r--r--   0      501       20     6285 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-stats/src/table_stats.rs
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 getdaft-0.2.8/local_dependencies/daft-scan/Cargo.toml
--rw-r--r--   0      501       20     2472 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/anonymous.rs
--rw-r--r--   0      501       20     7116 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/expr_rewriter.rs
--rw-r--r--   0      501       20     7766 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/file_format.rs
--rw-r--r--   0      501       20     9635 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/glob.rs
--rw-r--r--   0      501       20    16223 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/lib.rs
--rw-r--r--   0      501       20     2864 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/py_object_serde.rs
--rw-r--r--   0      501       20    14267 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/python.rs
--rw-r--r--   0      501       20     5026 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/scan_task_iters.rs
--rw-r--r--   0      501       20     4233 2023-12-22 00:03:44.000000 getdaft-0.2.8/local_dependencies/daft-scan/src/storage_config.rs
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 getdaft-0.2.8/Cargo.toml
--rw-r--r--   0      501       20      834 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      431 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/dependabot.yml
--rw-r--r--   0      501       20     1221 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/release-drafter.yml
--rw-r--r--   0      501       20     1515 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3521 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/build-artifact-s3.yml
--rw-r--r--   0      501       20     3075 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     4705 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/nightlies-tests.yml
--rw-r--r--   0      501       20     1661 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     1958 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    23872 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     7545 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2416 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20     2696 2023-12-22 00:03:44.000000 getdaft-0.2.8/.github/workflows/release-drafter.yml
--rw-r--r--   0      501       20      306 2023-12-22 00:03:44.000000 getdaft-0.2.8/.gitignore
--rw-r--r--   0      501       20     3025 2023-12-22 00:03:44.000000 getdaft-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-12-22 00:03:44.000000 getdaft-0.2.8/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-12-22 00:03:44.000000 getdaft-0.2.8/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-12-22 00:03:44.000000 getdaft-0.2.8/LICENSE
--rw-r--r--   0      501       20     1305 2023-12-22 00:03:44.000000 getdaft-0.2.8/Makefile
--rw-r--r--   0      501       20     8826 2023-12-22 00:03:44.000000 getdaft-0.2.8/README.rst
--rw-r--r--   0      501       20      172 2023-12-22 00:03:44.000000 getdaft-0.2.8/SECURITY.md
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/__init__.py
--rw-r--r--   0      501       20      925 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/README.md
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/__init__.py
--rw-r--r--   0      501       20       89 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/benchmark-requirements.txt
--rw-r--r--   0      501       20     3270 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/conftest.py
--rw-r--r--   0      501       20     1104 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/test_bulk_reads.py
--rw-r--r--   0      501       20     2019 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/parquet/test_num_rowgroups.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20    11217 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12362 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4599 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     2598 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/ray_job_runner.py
--rw-r--r--   0      501       20     2654 2023-12-22 00:03:44.000000 getdaft-0.2.8/benchmarking/tpch/subprefix_s3_files.py
--rw-r--r--   0      501       20     1446 2023-12-22 00:03:44.000000 getdaft-0.2.8/ci/upload_wheels.sh
--rw-r--r--   0      501       20      446 2023-12-22 00:03:44.000000 getdaft-0.2.8/codecov.yml
--rw-r--r--   0      501       20     2182 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/__init__.py
--rw-r--r--   0      501       20     6725 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/analytics.py
--rw-r--r--   0      501       20     4126 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/arrow_utils.py
--rw-r--r--   0      501       20     9412 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/context.py
--rw-r--r--   0      501       20     3412 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/convert.py
--rw-r--r--   0      501       20    38089 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/daft.pyi
--rw-r--r--   0      501       20       94 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    58550 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      324 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/dataframe/preview.py
--rw-r--r--   0      501       20     1430 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/dataframe/to_torch.py
--rw-r--r--   0      501       20    20321 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/errors.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/execution/__init__.py
--rw-r--r--   0      501       20    30323 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/execution/execution_step.py
--rw-r--r--   0      501       20    38542 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     9520 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/execution/rust_physical_plan_shim.py
--rw-r--r--   0      501       20      170 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/expressions/__init__.py
--rw-r--r--   0      501       20    32796 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/expressions/testing.py
--rw-r--r--   0      501       20    12102 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/iceberg/__init__.py
--rw-r--r--   0      501       20     6394 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/iceberg/iceberg_scan.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/internal/gpu.py
--rw-r--r--   0      501       20      911 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/__init__.py
--rw-r--r--   0      501       20     3783 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/_csv.py
--rw-r--r--   0      501       20     2911 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/_iceberg.py
--rw-r--r--   0      501       20     2380 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/_json.py
--rw-r--r--   0      501       20     2941 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/_parquet.py
--rw-r--r--   0      501       20     3393 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/common.py
--rw-r--r--   0      501       20      237 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/config.py
--rw-r--r--   0      501       20     2378 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/file_path.py
--rw-r--r--   0      501       20     1275 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/io/scan.py
--rw-r--r--   0      501       20      558 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/logging.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/logical/__init__.py
--rw-r--r--   0      501       20     8192 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/logical/builder.py
--rw-r--r--   0      501       20     1537 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20     6515 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/pickle/pickle.py
--rw-r--r--   0      501       20      151 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/plan_scheduler/__init__.py
--rw-r--r--   0      501       20      736 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/plan_scheduler/physical_plan_scheduler.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/py.typed
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/__init__.py
--rw-r--r--   0      501       20     6998 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1516 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/profiler.py
--rw-r--r--   0      501       20     2522 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/progress_bar.py
--rw-r--r--   0      501       20    12939 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    32667 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/ray_runner.py
--rw-r--r--   0      501       20     2131 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/runner.py
--rw-r--r--   0      501       20     2571 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/runners/runner_io.py
--rw-r--r--   0      501       20    26794 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/series.py
--rw-r--r--   0      501       20      589 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/table/__init__.py
--rw-r--r--   0      501       20    15885 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/table/micropartition.py
--rw-r--r--   0      501       20     5069 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/table/schema_inference.py
--rw-r--r--   0      501       20    22696 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/table/table.py
--rw-r--r--   0      501       20    16616 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/table/table_io.py
--rw-r--r--   0      501       20     7967 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/udf.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3313 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     3194 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/utils.py
--rw-r--r--   0      501       20      183 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/viz/__init__.py
--rw-r--r--   0      501       20     1951 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1522 2023-12-22 00:03:44.000000 getdaft-0.2.8/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20      148 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/Makefile
--rw-r--r--   0      501       20    73229 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20      583 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/dataframe-comp-table.csv
--rw-r--r--   0      501       20    25200 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20     9142 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/tpch-1000sf.html
--rw-r--r--   0      501       20     9647 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/tpch-100sf.html
--rw-r--r--   0      501       20     8757 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
--rw-r--r--   0      501       20      856 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_templates/layout.html
--rw-r--r--   0      501       20     1179 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20     1129 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      573 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2759 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     2318 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/datatype.rst
--rw-r--r--   0      501       20      139 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
--rw-r--r--   0      501       20      430 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
--rw-r--r--   0      501       20      151 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
--rw-r--r--   0      501       20      333 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
--rw-r--r--   0      501       20     4857 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      816 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      146 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     2431 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20      273 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/series/daft.Series.rst
--rw-r--r--   0      501       20      492 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/series.rst
--rw-r--r--   0      501       20       88 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20    14528 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/benchmarks/index.rst
--rw-r--r--   0      501       20     4211 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/conf.py
--rw-r--r--   0      501       20     5098 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1723 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/index.rst
--rw-r--r--   0      501       20     1356 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/install.rst
--rw-r--r--   0      501       20      896 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7830 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1783 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     7009 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     5280 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/datatypes.rst
--rw-r--r--   0      501       20     9481 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     8241 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20     4507 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/memory.rst
--rw-r--r--   0      501       20      206 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3251 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8859 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1600 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     6628 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-12-22 00:03:44.000000 getdaft-0.2.8/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1960 2023-12-22 00:03:44.000000 getdaft-0.2.8/pyproject.toml
--rw-r--r--   0      501       20     1566 2023-12-22 00:03:44.000000 getdaft-0.2.8/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-12-22 00:03:44.000000 getdaft-0.2.8/rust-toolchain.toml
--rw-r--r--   0      501       20     1920 2023-12-22 00:03:44.000000 getdaft-0.2.8/src/lib.rs
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/__init__.py
--rw-r--r--   0      501       20     9882 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/parquet-data/mvp.parquet
--rw-r--r--   0      501       20      762 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/parquet-data/parquet-with-schema-metadata.parquet
--rw-r--r--   0      501       20    55644 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/parquet-data/sampled-tpch-with-stats.parquet
--rw-r--r--   0      501       20    13534 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/sampled-tpch.csv
--rw-r--r--   0      501       20    39258 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/sampled-tpch.jsonl
--rw-r--r--   0      501       20      544 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20      357 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_concat.py
--rw-r--r--   0      501       20     1227 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     4610 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_filter.py
--rw-r--r--   0      501       20     5604 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     4590 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_if_else.py
--rw-r--r--   0      501       20     7292 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     3669 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/benchmarks/test_take.py
--rw-r--r--   0      501       20     5427 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      924 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/images/0000.jpg
--rw-r--r--   0      501       20      941 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/images/0007.jpg
--rw-r--r--   0      501       20     2740 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/images/0018.png
--rw-r--r--   0      501       20     7462 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/assets/images/0025.tiff
--rw-r--r--   0      501       20     1338 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1786 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     5427 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     2930 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_image.py
--rw-r--r--   0      501       20     3810 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      684 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10103 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20      575 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_concat.py
--rw-r--r--   0      501       20    33792 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1456 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_decimals.py
--rw-r--r--   0      501       20     1839 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1297 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1004 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     3201 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_iter.py
--rw-r--r--   0      501       20     4947 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20     3644 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20      405 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_repartition.py
--rw-r--r--   0      501       20    11449 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      802 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_select.py
--rw-r--r--   0      501       20     2299 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6418 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     7941 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      837 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     4494 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4295 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5114 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     8419 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      814 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1620 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/__init__.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/__init__.py
--rw-r--r--   0      501       20     1858 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/conftest.py
--rw-r--r--   0      501       20     2941 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/Dockerfile
--rwxr-xr-x   0      501       20     2529 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/check-license
--rw-r--r--   0      501       20     1008 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose-azurite.yml
--rw-r--r--   0      501       20     1059 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose-gcs-server.yml
--rw-r--r--   0      501       20     2490 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose.yml
--rwxr-xr-x   0      501       20      932 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/entrypoint.sh
--rw-r--r--   0      501       20     9280 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/provision.py
--rwxr-xr-x   0      501       20     1198 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-azurite.sh
--rw-r--r--   0      501       20     1218 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-gcs-server.sh
--rwxr-xr-x   0      501       20     1194 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-minio.sh
--rw-r--r--   0      501       20     1525 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/docker-compose/spark-defaults.conf
--rw-r--r--   0      501       20     6744 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/test_partition_pruning.py
--rw-r--r--   0      501       20     2077 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/iceberg/test_table_load.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/__init__.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/benchmarks/__init__.py
--rw-r--r--   0      501       20     7890 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/benchmarks/test_benchmark_glob.py
--rw-r--r--   0      501       20     6821 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/conftest.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/csv/__init__.py
--rw-r--r--   0      501       20     1977 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/csv/test_read_pushdowns.py
--rw-r--r--   0      501       20      110 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/Dockerfile.nginx
--rw-r--r--   0      501       20      314 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/Dockerfile.s3_retry_server
--rw-r--r--   0      501       20      935 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/docker-compose.yml
--rw-r--r--   0      501       20     1006 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/nginx-serve-static-files.conf
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/__init__.py
--rw-r--r--   0      501       20     1246 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/main.py
--rw-r--r--   0      501       20      357 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/retry-server-requirements.txt
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/__init__.py
--rw-r--r--   0      501       20     1908 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/get_retries_parquet_bucket.py
--rw-r--r--   0      501       20     1909 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/head_retries_parquet_bucket.py
--rw-r--r--   0      501       20     1192 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/rate_limited_echo_gets_bucket.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/utils/__init__.py
--rw-r--r--   0      501       20      362 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/utils/parquet_generation.py
--rw-r--r--   0      501       20      465 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/utils/responses.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/jsonl/__init__.py
--rw-r--r--   0      501       20     1231 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/jsonl/test_read_pushdown.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/parquet/__init__.py
--rw-r--r--   0      501       20     2319 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/parquet/test_read_pushdowns.py
--rw-r--r--   0      501       20     2074 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/parquet/test_reads_local_fixtures.py
--rw-r--r--   0      501       20    15264 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/parquet/test_reads_public_data.py
--rw-r--r--   0      501       20     1671 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/parquet/test_reads_s3_minio.py
--rw-r--r--   0      501       20     2607 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_list_files_azure.py
--rw-r--r--   0      501       20     2649 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_list_files_gcs.py
--rw-r--r--   0      501       20     4683 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_list_files_http.py
--rw-r--r--   0      501       20    15376 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_list_files_s3_minio.py
--rw-r--r--   0      501       20     2210 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_http.py
--rw-r--r--   0      501       20     1410 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_private_aws_s3.py
--rw-r--r--   0      501       20     3637 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_public_aws_s3.py
--rw-r--r--   0      501       20      527 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_public_azure.py
--rw-r--r--   0      501       20      549 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_s3_local_retry_server.py
--rw-r--r--   0      501       20      462 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_url_download_s3_minio.py
--rw-r--r--   0      501       20     1052 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/io/test_write_files_s3_minio.py
--rw-r--r--   0      501       20     4424 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/__init__.py
--rw-r--r--   0      501       20     2802 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/test_csv_roundtrip.py
--rw-r--r--   0      501       20     4823 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/test_list_files_local.py
--rw-r--r--   0      501       20     2559 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/test_merge_scan_tasks.py
--rw-r--r--   0      501       20     4239 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/test_parquet_roundtrip.py
--rw-r--r--   0      501       20     1829 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/io/test_url_download_local.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/ray/__init__.py
--rw-r--r--   0      501       20     1932 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/ray/runner.py
--rw-r--r--   0      501       20     5375 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/ray/test_dask.py
--rw-r--r--   0      501       20     9396 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20    24050 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_cast.py
--rw-r--r--   0      501       20    23179 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7773 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_concat.py
--rw-r--r--   0      501       20      889 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6157 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_float.py
--rw-r--r--   0      501       20     3892 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_hash.py
--rw-r--r--   0      501       20    21396 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_if_else.py
--rw-r--r--   0      501       20    22626 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_image.py
--rw-r--r--   0      501       20      889 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     4537 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_partitioning.py
--rw-r--r--   0      501       20     5740 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_series.py
--rw-r--r--   0      501       20     9049 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2187 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_sort.py
--rw-r--r--   0      501       20     6020 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_take.py
--rw-r--r--   0      501       20     4372 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4570 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_tensor.py
--rw-r--r--   0      501       20     7816 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/__init__.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/image/__init__.py
--rw-r--r--   0      501       20     4856 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/image/test_crop.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/list/__init__.py
--rw-r--r--   0      501       20     1201 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/list/test_list_join.py
--rw-r--r--   0      501       20      388 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/list/test_list_lengths.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/table_io/__init__.py
--rw-r--r--   0      501       20    12697 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/table_io/test_csv.py
--rw-r--r--   0      501       20     6270 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/table_io/test_json.py
--rw-r--r--   0      501       20    14743 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/table_io/test_parquet.py
--rw-r--r--   0      501       20     2194 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/table_io/test_read_time_cast.py
--rw-r--r--   0      501       20     1097 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      817 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2447 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_concat.py
--rw-r--r--   0      501       20     4990 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_eval.py
--rw-r--r--   0      501       20     4011 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7535 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_filter.py
--rw-r--r--   0      501       20    24306 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_from_py.py
--rw-r--r--   0      501       20      860 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_head.py
--rw-r--r--   0      501       20    11243 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_joins.py
--rw-r--r--   0      501       20      798 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_micropartition.py
--rw-r--r--   0      501       20    12519 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_partitioning.py
--rw-r--r--   0      501       20     1582 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    15041 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_sorting.py
--rw-r--r--   0      501       20    24533 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20     8299 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1183 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      339 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20      944 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/table/utf8/test_split.py
--rw-r--r--   0      501       20     3533 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/test_datatypes.py
--rw-r--r--   0      501       20     6776 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/test_resource_requests.py
--rw-r--r--   0      501       20     4601 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     4093 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      417 2023-12-22 00:03:44.000000 getdaft-0.2.8/tests/utils.py
--rw-r--r--   0      501       20        0 2023-12-22 00:03:44.000000 getdaft-0.2.8/tools/__init__.py
--rwxr-xr-x   0      501       20       69 2023-12-22 00:03:44.000000 getdaft-0.2.8/tools/check_for_rustls.sh
--rw-r--r--   0      501       20     1051 2023-12-22 00:03:44.000000 getdaft-0.2.8/tools/generate_whl_html_manifest.py
--rw-r--r--   0      501       20     1899 2023-12-22 00:03:44.000000 getdaft-0.2.8/tools/patch_package_version.py
--rw-r--r--   0      501       20       19 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/.gitignore
--rw-r--r--   0      501       20    19921 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20        5 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/flyte/.dockerignore
--rw-r--r--   0      501       20       98 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/flyte/Dockerfile
--rw-r--r--   0      501       20      604 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/flyte/README.md
--rw-r--r--   0      501       20     2309 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/flyte/app.py
--rw-r--r--   0      501       20     2874 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/flyte/notebook.ipynb
--rw-r--r--   0      501       20    12882 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20   461430 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/intro.ipynb
--rw-r--r--   0      501       20    98730 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/mnist.ipynb
--rw-r--r--   0      501       20     7166 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/talks_and_demos/pydata_global_2023.ipynb
--rw-r--r--   0      501       20    11673 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9279 2023-12-22 00:03:44.000000 getdaft-0.2.8/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20   101607 2023-12-22 00:05:21.000000 getdaft-0.2.8/Cargo.lock
--rw-r--r--   0        0        0    10212 1970-01-01 00:00:00.000000 getdaft-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-io/Cargo.toml
+-rw-r--r--   0      501       20    21636 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/azure_blob.rs
+-rw-r--r--   0      501       20    13465 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/google_cloud.rs
+-rw-r--r--   0      501       20    12872 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/http.rs
+-rw-r--r--   0      501       20    15489 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/lib.rs
+-rw-r--r--   0      501       20    15641 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/local.rs
+-rw-r--r--   0      501       20     4445 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/object_io.rs
+-rw-r--r--   0      501       20    27058 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/object_store_glob.rs
+-rw-r--r--   0      501       20     2592 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/python.rs
+-rw-r--r--   0      501       20    37315 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/s3_like.rs
+-rw-r--r--   0      501       20     3138 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/stats.rs
+-rw-r--r--   0      501       20      801 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-io/src/stream_utils.rs
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/common-daft-config/Cargo.toml
+-rw-r--r--   0      501       20     1915 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-daft-config/src/lib.rs
+-rw-r--r--   0      501       20     4347 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-daft-config/src/python.rs
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-csv/Cargo.toml
+-rw-r--r--   0      501       20     1940 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/compression.rs
+-rw-r--r--   0      501       20     2179 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/lib.rs
+-rw-r--r--   0      501       20    21037 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/metadata.rs
+-rw-r--r--   0      501       20    10370 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/options.rs
+-rw-r--r--   0      501       20     2104 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/python.rs
+-rw-r--r--   0      501       20    58138 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/read.rs
+-rw-r--r--   0      501       20     1396 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/src/schema.rs
+-rw-r--r--   0      501       20      536 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv
+-rw-r--r--   0      501       20      161 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.br
+-rw-r--r--   0      501       20      193 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.bz2
+-rw-r--r--   0      501       20      177 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.deflate
+-rw-r--r--   0      501       20      205 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.gz
+-rw-r--r--   0      501       20      183 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.lzma
+-rw-r--r--   0      501       20      228 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.xz
+-rw-r--r--   0      501       20      179 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.zl
+-rw-r--r--   0      501       20      201 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv.zst
+-rw-r--r--   0      501       20      191 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_all_null_column.csv
+-rw-r--r--   0      501       20      536 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_bar_delimiter.csv
+-rw-r--r--   0      501       20      533 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_comment.csv
+-rw-r--r--   0      501       20      121 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_conflicting_dtypes.csv
+-rw-r--r--   0      501       20      551 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_double_quote.csv
+-rw-r--r--   0      501       20      140 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_empty_lines.csv
+-rw-r--r--   0      501       20      548 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_escape.csv
+-rw-r--r--   0      501       20      111 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_invalid_header_cols_mismatch.csv
+-rw-r--r--   0      501       20       54 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_invalid_no_header_variable_num_cols.csv
+-rw-r--r--   0      501       20      468 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_no_headers.csv
+-rw-r--r--   0      501       20      190 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_nulls.csv
+-rw-r--r--   0      501       20      536 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_single_quote.csv
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/Cargo.toml
+-rw-r--r--   0      501       20     1436 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/lib.rs
+-rw-r--r--   0      501       20    34909 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/micropartition.rs
+-rw-r--r--   0      501       20     1066 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/agg.rs
+-rw-r--r--   0      501       20     1526 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/cast_to_schema.rs
+-rw-r--r--   0      501       20     1816 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/concat.rs
+-rw-r--r--   0      501       20     3229 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/eval_expressions.rs
+-rw-r--r--   0      501       20     1465 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/filter.rs
+-rw-r--r--   0      501       20     2255 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/join.rs
+-rw-r--r--   0      501       20      131 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/mod.rs
+-rw-r--r--   0      501       20     3355 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/partition.rs
+-rw-r--r--   0      501       20     1829 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/slice.rs
+-rw-r--r--   0      501       20     1390 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/sort.rs
+-rw-r--r--   0      501       20     2671 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/take.rs
+-rw-r--r--   0      501       20    24470 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-micropartition/src/python.rs
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-decoding/Cargo.toml
+-rw-r--r--   0      501       20    13365 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-decoding/src/deserialize.rs
+-rw-r--r--   0      501       20     3958 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-decoding/src/inference.rs
+-rw-r--r--   0      501       20      151 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-decoding/src/lib.rs
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-parquet/Cargo.toml
+-rw-r--r--   0      501       20    29429 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/file.rs
+-rw-r--r--   0      501       20     5359 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/lib.rs
+-rw-r--r--   0      501       20     3537 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/metadata.rs
+-rw-r--r--   0      501       20     9787 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/python.rs
+-rw-r--r--   0      501       20    23584 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/read.rs
+-rw-r--r--   0      501       20     9080 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/read_planner.rs
+-rw-r--r--   0      501       20    16750 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/column_range.rs
+-rw-r--r--   0      501       20     1506 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/mod.rs
+-rw-r--r--   0      501       20     1950 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/table_stats.rs
+-rw-r--r--   0      501       20     1586 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/utils.rs
+-rw-r--r--   0      501       20     8638 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-parquet/src/stream_reader.rs
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-json/Cargo.toml
+-rw-r--r--   0      501       20    20709 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/decoding.rs
+-rw-r--r--   0      501       20     8265 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/inference.rs
+-rw-r--r--   0      501       20     2159 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/lib.rs
+-rw-r--r--   0      501       20     6287 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/options.rs
+-rw-r--r--   0      501       20     2212 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/python.rs
+-rw-r--r--   0      501       20    46050 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/read.rs
+-rw-r--r--   0      501       20    15346 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/src/schema.rs
+-rw-r--r--   0      501       20     1130 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/dtypes.jsonl
+-rw-r--r--   0      501       20     2000 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl
+-rw-r--r--   0      501       20      176 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.br
+-rw-r--r--   0      501       20      228 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.bz2
+-rw-r--r--   0      501       20      258 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.gz
+-rw-r--r--   0      501       20      202 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.lzma
+-rw-r--r--   0      501       20      248 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.xz
+-rw-r--r--   0      501       20      230 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.zl
+-rw-r--r--   0      501       20      228 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl.zst
+-rw-r--r--   0      501       20      606 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny_all_null_column.jsonl
+-rw-r--r--   0      501       20      199 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny_conflicting_dtypes.jsonl
+-rw-r--r--   0      501       20      600 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny_nulls.jsonl
+-rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-plan/Cargo.toml
+-rw-r--r--   0      501       20    15953 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/builder.rs
+-rw-r--r--   0      501       20     4444 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/display.rs
+-rw-r--r--   0      501       20     2084 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/join.rs
+-rw-r--r--   0      501       20     1774 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/lib.rs
+-rw-r--r--   0      501       20     2433 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/agg.rs
+-rw-r--r--   0      501       20      890 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/concat.rs
+-rw-r--r--   0      501       20      275 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/distinct.rs
+-rw-r--r--   0      501       20     1583 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/explode.rs
+-rw-r--r--   0      501       20      942 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/filter.rs
+-rw-r--r--   0      501       20     5244 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/join.rs
+-rw-r--r--   0      501       20      550 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/limit.rs
+-rw-r--r--   0      501       20      436 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/mod.rs
+-rw-r--r--   0      501       20    18977 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/project.rs
+-rw-r--r--   0      501       20     1614 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/repartition.rs
+-rw-r--r--   0      501       20     1950 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/sink.rs
+-rw-r--r--   0      501       20     2409 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/sort.rs
+-rw-r--r--   0      501       20     2820 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/source.rs
+-rw-r--r--   0      501       20    11763 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/logical_plan.rs
+-rw-r--r--   0      501       20     8286 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/logical_plan_tracker.rs
+-rw-r--r--   0      501       20      111 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/mod.rs
+-rw-r--r--   0      501       20    22700 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/optimizer.rs
+-rw-r--r--   0      501       20     3718 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/drop_repartition.rs
+-rw-r--r--   0      501       20      333 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/mod.rs
+-rw-r--r--   0      501       20    29770 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_filter.rs
+-rw-r--r--   0      501       20    14914 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_limit.rs
+-rw-r--r--   0      501       20    30117 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_projection.rs
+-rw-r--r--   0      501       20     2301 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/rule.rs
+-rw-r--r--   0      501       20     2675 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/partitioning.rs
+-rw-r--r--   0      501       20      638 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/agg.rs
+-rw-r--r--   0      501       20      840 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/broadcast_join.rs
+-rw-r--r--   0      501       20      530 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/coalesce.rs
+-rw-r--r--   0      501       20      396 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/concat.rs
+-rw-r--r--   0      501       20     1292 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/csv.rs
+-rw-r--r--   0      501       20      448 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/empty_scan.rs
+-rw-r--r--   0      501       20      418 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/explode.rs
+-rw-r--r--   0      501       20     1367 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/fanout.rs
+-rw-r--r--   0      501       20      447 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/filter.rs
+-rw-r--r--   0      501       20      331 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/flatten.rs
+-rw-r--r--   0      501       20      724 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/hash_join.rs
+-rw-r--r--   0      501       20      610 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/in_memory.rs
+-rw-r--r--   0      501       20     1296 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/json.rs
+-rw-r--r--   0      501       20      573 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/limit.rs
+-rw-r--r--   0      501       20      955 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/mod.rs
+-rw-r--r--   0      501       20     1330 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/parquet.rs
+-rw-r--r--   0      501       20    11110 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/project.rs
+-rw-r--r--   0      501       20      339 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/reduce.rs
+-rw-r--r--   0      501       20      475 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/scan.rs
+-rw-r--r--   0      501       20      635 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/sort.rs
+-rw-r--r--   0      501       20      582 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/split.rs
+-rw-r--r--   0      501       20    32052 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/physical_plan.rs
+-rw-r--r--   0      501       20    33623 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/planner.rs
+-rw-r--r--   0      501       20     3710 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/resource_request.rs
+-rw-r--r--   0      501       20      873 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/sink_info.rs
+-rw-r--r--   0      501       20     5242 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/source_info/file_info.rs
+-rw-r--r--   0      501       20     3846 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/source_info/mod.rs
+-rw-r--r--   0      501       20     1919 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-plan/src/test/mod.rs
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/common-io-config/Cargo.toml
+-rw-r--r--   0      501       20      631 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/azure.rs
+-rw-r--r--   0      501       20      560 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/config.rs
+-rw-r--r--   0      501       20      536 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/gcs.rs
+-rw-r--r--   0      501       20      170 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/lib.rs
+-rw-r--r--   0      501       20    15730 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/python.rs
+-rw-r--r--   0      501       20     2437 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-io-config/src/s3.rs
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-compression/Cargo.toml
+-rw-r--r--   0      501       20     1940 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-compression/src/compression.rs
+-rw-r--r--   0      501       20      108 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-compression/src/lib.rs
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-dsl/Cargo.toml
+-rw-r--r--   0      501       20      273 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/README.md
+-rw-r--r--   0      501       20     1454 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/arithmetic.rs
+-rw-r--r--   0      501       20    24007 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/expr.rs
+-rw-r--r--   0      501       20     1479 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      592 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/float/mod.rs
+-rw-r--r--   0      501       20     2731 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/crop.rs
+-rw-r--r--   0      501       20     1353 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/decode.rs
+-rw-r--r--   0      501       20     1790 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/encode.rs
+-rw-r--r--   0      501       20     1586 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/mod.rs
+-rw-r--r--   0      501       20     2524 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/resize.rs
+-rw-r--r--   0      501       20     1033 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/explode.rs
+-rw-r--r--   0      501       20     2359 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/join.rs
+-rw-r--r--   0      501       20     1493 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/lengths.rs
+-rw-r--r--   0      501       20     1151 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/mod.rs
+-rw-r--r--   0      501       20     2251 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/mod.rs
+-rw-r--r--   0      501       20     1197 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      585 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
+-rw-r--r--   0      501       20     2208 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/partitioning/evaluators.rs
+-rw-r--r--   0      501       20     1389 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/partitioning/mod.rs
+-rw-r--r--   0      501       20      694 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/mod.rs
+-rw-r--r--   0      501       20     2565 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2793 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/udf.rs
+-rw-r--r--   0      501       20     1347 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/date.rs
+-rw-r--r--   0      501       20     1344 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1373 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1349 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/hour.rs
+-rw-r--r--   0      501       20     1925 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1355 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1349 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/year.rs
+-rw-r--r--   0      501       20     2317 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/uri/download.rs
+-rw-r--r--   0      501       20     1084 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/uri/mod.rs
+-rw-r--r--   0      501       20     1652 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1651 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1370 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1812 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1659 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/split.rs
+-rw-r--r--   0      501       20     1661 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20      920 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/lib.rs
+-rw-r--r--   0      501       20     7739 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/lit.rs
+-rw-r--r--   0      501       20     2097 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/optimization.rs
+-rw-r--r--   0      501       20     2508 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/pyobject.rs
+-rw-r--r--   0      501       20    12025 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/python.rs
+-rw-r--r--   0      501       20     3729 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-dsl/src/treenode.rs
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-scan/Cargo.toml
+-rw-r--r--   0      501       20     2472 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/anonymous.rs
+-rw-r--r--   0      501       20     7116 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/expr_rewriter.rs
+-rw-r--r--   0      501       20     7766 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/file_format.rs
+-rw-r--r--   0      501       20     9635 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/glob.rs
+-rw-r--r--   0      501       20    16223 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/lib.rs
+-rw-r--r--   0      501       20     2864 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/py_object_serde.rs
+-rw-r--r--   0      501       20    14267 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/python.rs
+-rw-r--r--   0      501       20     5026 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/scan_task_iters.rs
+-rw-r--r--   0      501       20     4233 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-scan/src/storage_config.rs
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-table/Cargo.toml
+-rw-r--r--   0      501       20     2798 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ffi.rs
+-rw-r--r--   0      501       20    19163 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/lib.rs
+-rw-r--r--   0      501       20     2168 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/agg.rs
+-rw-r--r--   0      501       20     3750 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/explode.rs
+-rw-r--r--   0      501       20     4402 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/groups.rs
+-rw-r--r--   0      501       20     2898 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/hash.rs
+-rw-r--r--   0      501       20     2631 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     6068 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/joins/mod.rs
+-rw-r--r--   0      501       20      134 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/mod.rs
+-rw-r--r--   0      501       20     3478 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/partition.rs
+-rw-r--r--   0      501       20     1808 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/search_sorted.rs
+-rw-r--r--   0      501       20      998 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/ops/sort.rs
+-rw-r--r--   0      501       20    11273 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-table/src/python.rs
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/common-error/Cargo.toml
+-rw-r--r--   0      501       20     3650 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-error/src/error.rs
+-rw-r--r--   0      501       20       64 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-error/src/lib.rs
+-rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/common-treenode/Cargo.toml
+-rw-r--r--   0      501       20    11886 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/common-treenode/src/lib.rs
+-rw-r--r--   0        0        0     1558 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-core/Cargo.toml
+-rw-r--r--   0      501       20      191 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/boolean.rs
+-rw-r--r--   0      501       20     6283 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/fixed_size_list_array.rs
+-rw-r--r--   0      501       20     6935 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/from.rs
+-rw-r--r--   0      501       20     1327 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/from_iter.rs
+-rw-r--r--   0      501       20     6419 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/arrow_growable.rs
+-rw-r--r--   0      501       20     1216 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/bitmap_growable.rs
+-rw-r--r--   0      501       20     3013 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/fixed_size_list_growable.rs
+-rw-r--r--   0      501       20     3655 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/list_growable.rs
+-rw-r--r--   0      501       20     3075 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/logical_growable.rs
+-rw-r--r--   0      501       20     7888 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/mod.rs
+-rw-r--r--   0      501       20     2027 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/python_growable.rs
+-rw-r--r--   0      501       20     3336 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/struct_growable.rs
+-rw-r--r--   0      501       20      734 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/iterator.rs
+-rw-r--r--   0      501       20     4907 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/list_array.rs
+-rw-r--r--   0      501       20     3325 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/mod.rs
+-rw-r--r--   0      501       20      269 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      738 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      860 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     7353 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3055 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     2031 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20     3084 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    75218 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    13907 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    57653 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     4259 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/concat.rs
+-rw-r--r--   0      501       20    10434 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     4566 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/count.rs
+-rw-r--r--   0      501       20     5502 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/date.rs
+-rw-r--r--   0      501       20     4086 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1271 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/float.rs
+-rw-r--r--   0      501       20     5357 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/from_arrow.rs
+-rw-r--r--   0      501       20     8630 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/full.rs
+-rw-r--r--   0      501       20     7191 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/get.rs
+-rw-r--r--   0      501       20     4408 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1861 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/hash.rs
+-rw-r--r--   0      501       20     5304 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    33802 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/image.rs
+-rw-r--r--   0      501       20     2197 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/len.rs
+-rw-r--r--   0      501       20     6189 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/list.rs
+-rw-r--r--   0      501       20     4344 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1730 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2756 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     3127 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3826 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20    13502 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/repr.rs
+-rw-r--r--   0      501       20      491 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    20392 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2396 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/sum.rs
+-rw-r--r--   0      501       20     7379 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/take.rs
+-rw-r--r--   0      501       20      456 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/tensor.rs
+-rw-r--r--   0      501       20     9823 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13618 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2490 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20     6545 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/serdes.rs
+-rw-r--r--   0      501       20     4986 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/array/struct_array.rs
+-rw-r--r--   0      501       20     2294 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/count_mode.rs
+-rw-r--r--   0      501       20    11287 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/binary_ops.rs
+-rw-r--r--   0      501       20    17006 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     3661 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/field.rs
+-rw-r--r--   0      501       20     3153 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/image_format.rs
+-rw-r--r--   0      501       20     6404 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     5835 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     8852 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     9276 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1041 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20     6039 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/kernels/mod.rs
+-rw-r--r--   0      501       20    14629 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3905 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/kernels/utf8.rs
+-rw-r--r--   0      501       20      832 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/lib.rs
+-rw-r--r--   0      501       20    11194 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/python/datatype.rs
+-rw-r--r--   0      501       20     1098 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/python/field.rs
+-rw-r--r--   0      501       20      610 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/python/mod.rs
+-rw-r--r--   0      501       20     2278 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/python/schema.rs
+-rw-r--r--   0      501       20    15815 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/python/series.rs
+-rw-r--r--   0      501       20     6524 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/schema.rs
+-rw-r--r--   0      501       20    10715 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs
+-rw-r--r--   0      501       20     7955 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     8237 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      220 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     6396 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/nested_array.rs
+-rw-r--r--   0      501       20     1984 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/from.rs
+-rw-r--r--   0      501       20     2875 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/mod.rs
+-rw-r--r--   0      501       20      910 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5355 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     3462 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1967 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      205 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/cast.rs
+-rw-r--r--   0      501       20      682 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1173 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     3694 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/date.rs
+-rw-r--r--   0      501       20     2415 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      693 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      440 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/float.rs
+-rw-r--r--   0      501       20      468 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      445 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      324 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     3250 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/image.rs
+-rw-r--r--   0      501       20      297 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/len.rs
+-rw-r--r--   0      501       20     1994 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2563 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      477 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/not.rs
+-rw-r--r--   0      501       20      160 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/null.rs
+-rw-r--r--   0      501       20     4081 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/partitioning.rs
+-rw-r--r--   0      501       20      703 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1562 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      704 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1856 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20    13838 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/serdes.rs
+-rw-r--r--   0      501       20     2333 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/series/series_like.rs
+-rw-r--r--   0      501       20     5474 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/utils/arrow.rs
+-rw-r--r--   0      501       20     6787 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/utils/display_table.rs
+-rw-r--r--   0      501       20      582 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/utils/hashable_float_wrapper.rs
+-rw-r--r--   0      501       20     1267 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/utils/mod.rs
+-rw-r--r--   0      501       20     9991 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 getdaft-0.2.9/local_dependencies/daft-stats/Cargo.toml
+-rw-r--r--   0      501       20     1490 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/arithmetic.rs
+-rw-r--r--   0      501       20     6868 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/comparison.rs
+-rw-r--r--   0      501       20     2363 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/logical.rs
+-rw-r--r--   0      501       20    10073 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/mod.rs
+-rw-r--r--   0      501       20     1184 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/lib.rs
+-rw-r--r--   0      501       20      946 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/partition_spec.rs
+-rw-r--r--   0      501       20      138 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/table_metadata.rs
+-rw-r--r--   0      501       20     6285 2024-01-06 00:34:15.000000 getdaft-0.2.9/local_dependencies/daft-stats/src/table_stats.rs
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 getdaft-0.2.9/Cargo.toml
+-rw-r--r--   0      501       20      834 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      431 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/dependabot.yml
+-rw-r--r--   0      501       20     1221 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/release-drafter.yml
+-rw-r--r--   0      501       20     1515 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3521 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/build-artifact-s3.yml
+-rw-r--r--   0      501       20     3075 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     4705 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/nightlies-tests.yml
+-rw-r--r--   0      501       20     1661 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     1958 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    23872 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     7545 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2416 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20     2696 2024-01-06 00:34:15.000000 getdaft-0.2.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0      501       20      306 2024-01-06 00:34:15.000000 getdaft-0.2.9/.gitignore
+-rw-r--r--   0      501       20     3025 2024-01-06 00:34:15.000000 getdaft-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2024-01-06 00:34:15.000000 getdaft-0.2.9/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2024-01-06 00:34:15.000000 getdaft-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2024-01-06 00:34:15.000000 getdaft-0.2.9/LICENSE
+-rw-r--r--   0      501       20     1305 2024-01-06 00:34:15.000000 getdaft-0.2.9/Makefile
+-rw-r--r--   0      501       20     8826 2024-01-06 00:34:15.000000 getdaft-0.2.9/README.rst
+-rw-r--r--   0      501       20      172 2024-01-06 00:34:15.000000 getdaft-0.2.9/SECURITY.md
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/__init__.py
+-rw-r--r--   0      501       20      925 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/README.md
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/__init__.py
+-rw-r--r--   0      501       20       89 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/benchmark-requirements.txt
+-rw-r--r--   0      501       20     3270 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/conftest.py
+-rw-r--r--   0      501       20     1104 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/test_bulk_reads.py
+-rw-r--r--   0      501       20     2019 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/parquet/test_num_rowgroups.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20    11217 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12362 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4599 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     2598 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/ray_job_runner.py
+-rw-r--r--   0      501       20     2654 2024-01-06 00:34:15.000000 getdaft-0.2.9/benchmarking/tpch/subprefix_s3_files.py
+-rw-r--r--   0      501       20     1446 2024-01-06 00:34:15.000000 getdaft-0.2.9/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      446 2024-01-06 00:34:15.000000 getdaft-0.2.9/codecov.yml
+-rw-r--r--   0      501       20     2182 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/__init__.py
+-rw-r--r--   0      501       20     6725 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/analytics.py
+-rw-r--r--   0      501       20     4126 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/arrow_utils.py
+-rw-r--r--   0      501       20     9412 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/context.py
+-rw-r--r--   0      501       20     3412 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/convert.py
+-rw-r--r--   0      501       20    38089 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    58550 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      324 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/dataframe/preview.py
+-rw-r--r--   0      501       20     1430 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/dataframe/to_torch.py
+-rw-r--r--   0      501       20    20321 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/datatype.py
+-rw-r--r--   0      501       20       84 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/errors.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/execution/__init__.py
+-rw-r--r--   0      501       20    30323 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/execution/execution_step.py
+-rw-r--r--   0      501       20    38542 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     9520 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/execution/rust_physical_plan_shim.py
+-rw-r--r--   0      501       20      170 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    32796 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12102 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/iceberg/__init__.py
+-rw-r--r--   0      501       20     6394 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/iceberg/iceberg_scan.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/internal/gpu.py
+-rw-r--r--   0      501       20      911 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/__init__.py
+-rw-r--r--   0      501       20     3783 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/_csv.py
+-rw-r--r--   0      501       20     2911 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/_iceberg.py
+-rw-r--r--   0      501       20     2380 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/_json.py
+-rw-r--r--   0      501       20     2941 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/_parquet.py
+-rw-r--r--   0      501       20     3393 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/common.py
+-rw-r--r--   0      501       20      237 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/config.py
+-rw-r--r--   0      501       20     2378 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/file_path.py
+-rw-r--r--   0      501       20     1275 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/io/scan.py
+-rw-r--r--   0      501       20      558 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/logging.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8192 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/logical/builder.py
+-rw-r--r--   0      501       20     1537 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20     6515 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/pickle/pickle.py
+-rw-r--r--   0      501       20      151 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/plan_scheduler/__init__.py
+-rw-r--r--   0      501       20      736 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/plan_scheduler/physical_plan_scheduler.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/py.typed
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/__init__.py
+-rw-r--r--   0      501       20     6998 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1516 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/profiler.py
+-rw-r--r--   0      501       20     2522 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/progress_bar.py
+-rw-r--r--   0      501       20    12939 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    32667 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20     2131 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/runner.py
+-rw-r--r--   0      501       20     2571 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    26794 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/series.py
+-rw-r--r--   0      501       20      589 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/table/__init__.py
+-rw-r--r--   0      501       20    15885 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/table/micropartition.py
+-rw-r--r--   0      501       20     5069 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/table/schema_inference.py
+-rw-r--r--   0      501       20    22696 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/table/table.py
+-rw-r--r--   0      501       20    16616 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/table/table_io.py
+-rw-r--r--   0      501       20     7967 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/udf.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3313 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     3194 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/utils.py
+-rw-r--r--   0      501       20      183 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1951 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1522 2024-01-06 00:34:15.000000 getdaft-0.2.9/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20      148 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/Makefile
+-rw-r--r--   0      501       20    73229 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20      583 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/dataframe-comp-table.csv
+-rw-r--r--   0      501       20    25200 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20     1179 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20     1129 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      573 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2759 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     2318 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20      139 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
+-rw-r--r--   0      501       20      430 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
+-rw-r--r--   0      501       20      151 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
+-rw-r--r--   0      501       20      333 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
+-rw-r--r--   0      501       20     4857 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      816 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      146 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     2431 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20      273 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/series/daft.Series.rst
+-rw-r--r--   0      501       20      492 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/series.rst
+-rw-r--r--   0      501       20       88 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     4211 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/conf.py
+-rw-r--r--   0      501       20     5098 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1723 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/index.rst
+-rw-r--r--   0      501       20     1356 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/install.rst
+-rw-r--r--   0      501       20      896 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7830 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1783 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     7009 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     5280 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9481 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     8241 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20     4507 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/memory.rst
+-rw-r--r--   0      501       20      206 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3251 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8859 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1600 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     6628 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2024-01-06 00:34:15.000000 getdaft-0.2.9/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1960 2024-01-06 00:34:15.000000 getdaft-0.2.9/pyproject.toml
+-rw-r--r--   0      501       20     1566 2024-01-06 00:34:15.000000 getdaft-0.2.9/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2024-01-06 00:34:15.000000 getdaft-0.2.9/rust-toolchain.toml
+-rw-r--r--   0      501       20     1920 2024-01-06 00:34:15.000000 getdaft-0.2.9/src/lib.rs
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/__init__.py
+-rw-r--r--   0      501       20      299 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/__init__.py
+-rw-r--r--   0      501       20     9882 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/parquet-data/mvp.parquet
+-rw-r--r--   0      501       20      762 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/parquet-data/parquet-with-schema-metadata.parquet
+-rw-r--r--   0      501       20    55644 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/parquet-data/sampled-tpch-with-stats.parquet
+-rw-r--r--   0      501       20    13534 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/sampled-tpch.csv
+-rw-r--r--   0      501       20    39258 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/sampled-tpch.jsonl
+-rw-r--r--   0      501       20      544 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20      357 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_concat.py
+-rw-r--r--   0      501       20     1227 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     4610 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_filter.py
+-rw-r--r--   0      501       20     5604 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     4590 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_if_else.py
+-rw-r--r--   0      501       20     7292 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     3669 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/benchmarks/test_take.py
+-rw-r--r--   0      501       20     5427 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/conftest.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      924 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/images/0000.jpg
+-rw-r--r--   0      501       20      941 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/images/0007.jpg
+-rw-r--r--   0      501       20     2740 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/images/0018.png
+-rw-r--r--   0      501       20     7462 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/assets/images/0025.tiff
+-rw-r--r--   0      501       20     1338 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1786 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     5427 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     2930 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_image.py
+-rw-r--r--   0      501       20     3810 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      684 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10103 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20      575 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_concat.py
+-rw-r--r--   0      501       20    33792 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1456 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_decimals.py
+-rw-r--r--   0      501       20     1839 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1297 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1004 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     3201 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_iter.py
+-rw-r--r--   0      501       20     4947 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     3644 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      405 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20    11449 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      802 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20     2299 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6418 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     7941 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      837 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     4494 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4295 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5114 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     8419 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      814 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1620 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/__init__.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/__init__.py
+-rw-r--r--   0      501       20     1858 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/conftest.py
+-rw-r--r--   0      501       20     2941 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/Dockerfile
+-rwxr-xr-x   0      501       20     2529 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/check-license
+-rw-r--r--   0      501       20     1008 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose-azurite.yml
+-rw-r--r--   0      501       20     1059 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose-gcs-server.yml
+-rw-r--r--   0      501       20     2490 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose.yml
+-rwxr-xr-x   0      501       20      932 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/entrypoint.sh
+-rw-r--r--   0      501       20     9280 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/provision.py
+-rwxr-xr-x   0      501       20     1198 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-azurite.sh
+-rw-r--r--   0      501       20     1218 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-gcs-server.sh
+-rwxr-xr-x   0      501       20     1194 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-minio.sh
+-rw-r--r--   0      501       20     1525 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/docker-compose/spark-defaults.conf
+-rw-r--r--   0      501       20     6744 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/test_partition_pruning.py
+-rw-r--r--   0      501       20     2077 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/iceberg/test_table_load.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/__init__.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/benchmarks/__init__.py
+-rw-r--r--   0      501       20     7890 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/benchmarks/test_benchmark_glob.py
+-rw-r--r--   0      501       20     6926 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/conftest.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/csv/__init__.py
+-rw-r--r--   0      501       20     1977 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/csv/test_read_pushdowns.py
+-rw-r--r--   0      501       20      110 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/Dockerfile.nginx
+-rw-r--r--   0      501       20      314 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/Dockerfile.s3_retry_server
+-rw-r--r--   0      501       20      935 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/docker-compose.yml
+-rw-r--r--   0      501       20     1006 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/nginx-serve-static-files.conf
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/__init__.py
+-rw-r--r--   0      501       20     1246 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/main.py
+-rw-r--r--   0      501       20      357 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/retry-server-requirements.txt
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/__init__.py
+-rw-r--r--   0      501       20     1908 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/get_retries_parquet_bucket.py
+-rw-r--r--   0      501       20     1909 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/head_retries_parquet_bucket.py
+-rw-r--r--   0      501       20     1192 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/rate_limited_echo_gets_bucket.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/utils/__init__.py
+-rw-r--r--   0      501       20      362 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/utils/parquet_generation.py
+-rw-r--r--   0      501       20      465 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/utils/responses.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/jsonl/__init__.py
+-rw-r--r--   0      501       20     1231 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/jsonl/test_read_pushdown.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/parquet/__init__.py
+-rw-r--r--   0      501       20     2319 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/parquet/test_read_pushdowns.py
+-rw-r--r--   0      501       20     2074 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/parquet/test_reads_local_fixtures.py
+-rw-r--r--   0      501       20    15430 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/parquet/test_reads_public_data.py
+-rw-r--r--   0      501       20     1671 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/parquet/test_reads_s3_minio.py
+-rw-r--r--   0      501       20     2607 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_list_files_azure.py
+-rw-r--r--   0      501       20     2649 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_list_files_gcs.py
+-rw-r--r--   0      501       20     4683 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_list_files_http.py
+-rw-r--r--   0      501       20    16378 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_list_files_s3_minio.py
+-rw-r--r--   0      501       20     2210 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_http.py
+-rw-r--r--   0      501       20     1411 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_private_aws_s3.py
+-rw-r--r--   0      501       20     3642 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_public_aws_s3.py
+-rw-r--r--   0      501       20      527 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_public_azure.py
+-rw-r--r--   0      501       20      549 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_s3_local_retry_server.py
+-rw-r--r--   0      501       20      462 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_url_download_s3_minio.py
+-rw-r--r--   0      501       20     1052 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/io/test_write_files_s3_minio.py
+-rw-r--r--   0      501       20     4424 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/__init__.py
+-rw-r--r--   0      501       20     2802 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/test_csv_roundtrip.py
+-rw-r--r--   0      501       20     4823 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/test_list_files_local.py
+-rw-r--r--   0      501       20     2559 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/test_merge_scan_tasks.py
+-rw-r--r--   0      501       20     4239 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/test_parquet_roundtrip.py
+-rw-r--r--   0      501       20     1829 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/io/test_url_download_local.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/ray/__init__.py
+-rw-r--r--   0      501       20     1932 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/ray/runner.py
+-rw-r--r--   0      501       20     5375 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     9396 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20    24050 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_cast.py
+-rw-r--r--   0      501       20    23179 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7773 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_concat.py
+-rw-r--r--   0      501       20      889 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6157 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_float.py
+-rw-r--r--   0      501       20     3892 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21396 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_if_else.py
+-rw-r--r--   0      501       20    22626 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     4537 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_partitioning.py
+-rw-r--r--   0      501       20     5740 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_series.py
+-rw-r--r--   0      501       20     9049 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2187 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6020 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_take.py
+-rw-r--r--   0      501       20     4372 2024-01-06 00:34:15.000000 getdaft-0.2.9/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4570 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/series/test_tensor.py
+-rw-r--r--   0      501       20     7816 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/__init__.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/image/__init__.py
+-rw-r--r--   0      501       20     4856 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/image/test_crop.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/list/__init__.py
+-rw-r--r--   0      501       20     1201 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/list/test_list_join.py
+-rw-r--r--   0      501       20      388 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/list/test_list_lengths.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/table_io/__init__.py
+-rw-r--r--   0      501       20    12697 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/table_io/test_csv.py
+-rw-r--r--   0      501       20     6270 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/table_io/test_json.py
+-rw-r--r--   0      501       20    14743 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/table_io/test_parquet.py
+-rw-r--r--   0      501       20     2194 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/table_io/test_read_time_cast.py
+-rw-r--r--   0      501       20     1097 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      817 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2447 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4990 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_eval.py
+-rw-r--r--   0      501       20     4011 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7535 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_filter.py
+-rw-r--r--   0      501       20    24306 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      860 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_head.py
+-rw-r--r--   0      501       20    11243 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_joins.py
+-rw-r--r--   0      501       20      798 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_micropartition.py
+-rw-r--r--   0      501       20    12519 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20     1582 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    15041 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    24533 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20     8299 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1183 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      339 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20      944 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/table/utf8/test_split.py
+-rw-r--r--   0      501       20     3533 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/test_datatypes.py
+-rw-r--r--   0      501       20     6776 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/test_resource_requests.py
+-rw-r--r--   0      501       20     4601 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     4093 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      417 2024-01-06 00:34:16.000000 getdaft-0.2.9/tests/utils.py
+-rw-r--r--   0      501       20        0 2024-01-06 00:34:16.000000 getdaft-0.2.9/tools/__init__.py
+-rwxr-xr-x   0      501       20       69 2024-01-06 00:34:16.000000 getdaft-0.2.9/tools/check_for_rustls.sh
+-rw-r--r--   0      501       20     1051 2024-01-06 00:34:16.000000 getdaft-0.2.9/tools/generate_whl_html_manifest.py
+-rw-r--r--   0      501       20     1899 2024-01-06 00:34:16.000000 getdaft-0.2.9/tools/patch_package_version.py
+-rw-r--r--   0      501       20       19 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/.gitignore
+-rw-r--r--   0      501       20    19921 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20        5 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/flyte/.dockerignore
+-rw-r--r--   0      501       20       98 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/flyte/Dockerfile
+-rw-r--r--   0      501       20      604 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/flyte/README.md
+-rw-r--r--   0      501       20     2309 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/flyte/app.py
+-rw-r--r--   0      501       20     2874 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/flyte/notebook.ipynb
+-rw-r--r--   0      501       20    12882 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20   461430 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/intro.ipynb
+-rw-r--r--   0      501       20    98730 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20     7166 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/talks_and_demos/pydata_global_2023.ipynb
+-rw-r--r--   0      501       20    11673 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9279 2024-01-06 00:34:16.000000 getdaft-0.2.9/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20   101607 2024-01-06 00:35:20.000000 getdaft-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0    10212 1970-01-01 00:00:00.000000 getdaft-0.2.9/PKG-INFO
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-dsl/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python", "daft-io/python", "common-io-config/python", "common-treenode/python"]
 
 [package]
 edition = "2021"
 name = "daft-dsl"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.bincode]
 version = "1.3.3"
 
 [dependencies.pyo3]
 features = [ "extension-module", "multiple-pymethods", "abi3-py37",]
 version = "0.19.2"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/arithmetic.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/expr.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/float/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/crop.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/crop.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/decode.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/decode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/encode.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/encode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/image/resize.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/image/resize.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/explode.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/join.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/lengths.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/lengths.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/list/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/list/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/partitioning/evaluators.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/partitioning/evaluators.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/partitioning/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/partitioning/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/python/udf.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/date.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/hour.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/hour.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/temporal/year.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/uri/download.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/uri/download.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/uri/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/length.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/split.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/split.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/lit.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/optimization.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/pyobject.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-dsl/src/treenode.rs` & `getdaft-0.2.9/local_dependencies/daft-dsl/src/treenode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-error/src/error.rs` & `getdaft-0.2.9/local_dependencies/common-error/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:numpy", "common-error/python"]
 
 [package]
 edition = "2021"
 name = "daft-core"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.arrow2]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 rev = "d5685eebf1d65c3f3d854370ad39f93dcd91971a"
 features = ["chrono-tz", "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc"]
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/fixed_size_list_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/fixed_size_list_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/from.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/from_iter.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/from_iter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/arrow_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/arrow_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/bitmap_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/bitmap_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/fixed_size_list_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/fixed_size_list_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/list_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/list_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/logical_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/logical_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/python_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/python_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/growable/struct_growable.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/growable/struct_growable.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/iterator.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/list_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/list_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/apply.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arange.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/as_arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/broadcast.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/cast.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/cast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/comparison.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/concat.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/count.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/date.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/filter.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/float.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/from_arrow.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/from_arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/full.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/get.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/get.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/groups.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/hash.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/if_else.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/if_else.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/image.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/image.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/len.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/list.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/list_agg.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/mean.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/null.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/pairwise.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/repr.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/repr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/sum.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/take.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/ops/utf8.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/serdes.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/serdes.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/array/struct_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/array/struct_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/count_mode.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/count_mode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/binary_ops.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/binary_ops.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/dtype.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/field.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/image_format.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/image_format.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/image_mode.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/image_mode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/logical.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/logical.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/matching.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/matching.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/datatypes/time_unit.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/ffi.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/kernels/hashing.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/kernels/search_sorted.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/kernels/utf8.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/python/datatype.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/python/datatype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/python/field.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/python/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/python/schema.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/python/series.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/python/series.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/schema.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/data_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/logical_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/array_impl/nested_array.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/array_impl/nested_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/from.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/abs.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/agg.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/arithmetic.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/broadcast.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/comparison.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/concat.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/date.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/downcast.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/filter.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/image.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/image.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/list.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/partitioning.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/partitioning.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/take.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/ops/utf8.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/serdes.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/serdes.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/series/series_like.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/series/series_like.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/utils/arrow.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/utils/display_table.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/utils/display_table.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/utils/hashable_float_wrapper.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/utils/hashable_float_wrapper.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/utils/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-core/src/utils/supertype.rs` & `getdaft-0.2.9/local_dependencies/daft-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-json/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python", "daft-io/python", "daft-table/python", "daft-dsl/python"]
 
 [package]
 edition = "2021"
 name = "daft-json"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.async-compression]
 version = "0.4.5"
 features = [ "tokio", "all-algorithms",]
 
 [dependencies.snafu]
 version = "0.7.4"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/decoding.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/decoding.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/inference.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/inference.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/options.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/options.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/read.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/read.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/src/schema.rs` & `getdaft-0.2.9/local_dependencies/daft-json/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/test/dtypes.jsonl` & `getdaft-0.2.9/local_dependencies/daft-json/test/dtypes.jsonl`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny.jsonl` & `getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny.jsonl`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny_all_null_column.jsonl` & `getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny_all_null_column.jsonl`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-json/test/iris_tiny_nulls.jsonl` & `getdaft-0.2.9/local_dependencies/daft-json/test/iris_tiny_nulls.jsonl`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-parquet/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python", "daft-io/python", "daft-table/python", "daft-stats/python", "daft-dsl/python"]
 
 [package]
 edition = "2021"
 name = "daft-parquet"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.tokio]
 version = "1.32.0"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/file.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/file.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/metadata.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/read.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/read.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/read_planner.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/read_planner.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/column_range.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/column_range.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/table_stats.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/table_stats.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/statistics/utils.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/statistics/utils.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-parquet/src/stream_reader.rs` & `getdaft-0.2.9/local_dependencies/daft-parquet/src/stream_reader.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-decoding/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-decoding/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 chrono = "0.4.26"
 chrono-tz = "0.8.4"
 url = "2.4.0"
 
 [package]
 edition = "2021"
 name = "daft-decoding"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.async-compression]
 version = "0.4.5"
 features = [ "tokio", "all-algorithms",]
 
 [dependencies.tokio]
 version = "1.32.0"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-decoding/src/deserialize.rs` & `getdaft-0.2.9/local_dependencies/daft-decoding/src/deserialize.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-decoding/src/inference.rs` & `getdaft-0.2.9/local_dependencies/daft-decoding/src/inference.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-io/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python", "common-io-config/python"]
 
 [package]
 edition = "2021"
 name = "daft-io"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.tokio]
 version = "1.32.0"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/azure_blob.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/azure_blob.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/google_cloud.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/google_cloud.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/http.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/http.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     }
     .context(InvalidUrlSnafu { path: input })?;
 
     let scheme = url.scheme().to_lowercase();
     match scheme.as_ref() {
         "file" => Ok((SourceType::File, fixed_input)),
         "http" | "https" => Ok((SourceType::Http, fixed_input)),
-        "s3" => Ok((SourceType::S3, fixed_input)),
+        "s3" | "s3a" => Ok((SourceType::S3, fixed_input)),
         "az" | "abfs" => Ok((SourceType::AzureBlob, fixed_input)),
         "gcs" | "gs" => Ok((SourceType::GCS, fixed_input)),
         #[cfg(target_env = "msvc")]
         _ if scheme.len() == 1 && ("a" <= scheme.as_str() && (scheme.as_str() <= "z")) => {
             Ok((SourceType::File, Cow::Owned(format!("file://{input}"))))
         }
         _ => Err(Error::NotImplementedSource { store: scheme }),
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/local.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/local.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/object_io.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/object_io.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/object_store_glob.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/object_store_glob.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/s3_like.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/s3_like.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/stats.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/stats.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-io/src/stream_utils.rs` & `getdaft-0.2.9/local_dependencies/daft-io/src/stream_utils.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-daft-config/Cargo.toml` & `getdaft-0.2.9/local_dependencies/common-daft-config/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-io-config/python"]
 
 [package]
 edition = "2021"
 name = "common-daft-config"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.bincode]
 version = "1.3.3"
 
 [dependencies.lazy_static]
 version = "1.4.0"
```

### Comparing `getdaft-0.2.8/local_dependencies/common-daft-config/src/lib.rs` & `getdaft-0.2.9/local_dependencies/common-daft-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-daft-config/src/python.rs` & `getdaft-0.2.9/local_dependencies/common-daft-config/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-micropartition/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-error/python", "daft-core/python", "daft-dsl/python", "daft-table/python", "daft-io/python", "daft-parquet/python", "daft-scan/python", "daft-stats/python"]
 
 [package]
 edition = "2021"
 name = "daft-micropartition"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.arrow2]
 git = "https://github.com/Eventual-Inc/arrow2"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/micropartition.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/micropartition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/agg.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/cast_to_schema.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/cast_to_schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/concat.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/eval_expressions.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/eval_expressions.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/filter.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/join.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/partition.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/slice.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/slice.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/ops/take.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-micropartition/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-micropartition/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-plan/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-error/python", "common-io-config/python", "common-daft-config/python", "daft-core/python", "daft-dsl/python", "daft-table/python"]
 
 [package]
 edition = "2021"
 name = "daft-plan"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.arrow2]
 git = "https://github.com/Eventual-Inc/arrow2"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/builder.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/builder.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/display.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/display.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/join.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/agg.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/concat.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/explode.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/filter.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/join.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/limit.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/limit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/project.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/project.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/repartition.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/repartition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/sink.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/sink.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_ops/source.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_ops/source.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/logical_plan.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/logical_plan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/logical_plan_tracker.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/logical_plan_tracker.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/optimizer.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/optimizer.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/drop_repartition.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/drop_repartition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_filter.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_limit.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_limit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/push_down_projection.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/push_down_projection.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/optimization/rules/rule.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/optimization/rules/rule.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/partitioning.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/partitioning.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/agg.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/broadcast_join.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/broadcast_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/coalesce.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/coalesce.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/csv.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/csv.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/fanout.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/fanout.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/hash_join.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/in_memory.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/in_memory.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/json.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/json.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/limit.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/limit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/parquet.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/parquet.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/project.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/project.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_ops/split.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_ops/split.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/physical_plan.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/physical_plan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/planner.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/planner.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/resource_request.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/resource_request.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/sink_info.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/sink_info.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/source_info/file_info.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/source_info/file_info.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/source_info/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/source_info/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-plan/src/test/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-plan/src/test/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-treenode/src/lib.rs` & `getdaft-0.2.9/local_dependencies/common-treenode/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-io-config/src/azure.rs` & `getdaft-0.2.9/local_dependencies/common-io-config/src/azure.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-io-config/src/config.rs` & `getdaft-0.2.9/local_dependencies/common-io-config/src/config.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-io-config/src/gcs.rs` & `getdaft-0.2.9/local_dependencies/common-io-config/src/gcs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-io-config/src/python.rs` & `getdaft-0.2.9/local_dependencies/common-io-config/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/common-io-config/src/s3.rs` & `getdaft-0.2.9/local_dependencies/common-io-config/src/s3.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-csv/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python", "daft-io/python", "daft-table/python", "daft-dsl/python"]
 
 [package]
 edition = "2021"
 name = "daft-csv"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.async-compression]
 version = "0.4.5"
 features = [ "tokio", "all-algorithms",]
 
 [dependencies.snafu]
 version = "0.7.4"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/compression.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/compression.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/metadata.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/options.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/options.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/read.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/read.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/src/schema.rs` & `getdaft-0.2.9/local_dependencies/daft-csv/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_bar_delimiter.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_bar_delimiter.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_comment.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_comment.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_double_quote.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_double_quote.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_escape.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_escape.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-csv/test/iris_tiny_single_quote.csv` & `getdaft-0.2.9/local_dependencies/daft-csv/test/iris_tiny_single_quote.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-table/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-error/python", "daft-core/python", "daft-dsl/python"]
 
 [package]
 edition = "2021"
 name = "daft-table"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.arrow2]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 rev = "d5685eebf1d65c3f3d854370ad39f93dcd91971a"
 
 [dependencies.pyo3]
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ffi.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/agg.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/explode.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/groups.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/hash.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/joins/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/partition.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/search_sorted.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/ops/sort.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-table/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-table/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-compression/src/compression.rs` & `getdaft-0.2.9/local_dependencies/daft-compression/src/compression.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-stats/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-error/python", "daft-core/python", "daft-dsl/python", "daft-table/python"]
 
 [package]
 edition = "2021"
 name = "daft-stats"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.pyo3]
 features = [ "extension-module", "multiple-pymethods", "abi3-py37",]
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/arithmetic.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/comparison.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/logical.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/logical.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/column_stats/mod.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/column_stats/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/partition_spec.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/partition_spec.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-stats/src/table_stats.rs` & `getdaft-0.2.9/local_dependencies/daft-stats/src/table_stats.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/Cargo.toml` & `getdaft-0.2.9/local_dependencies/daft-scan/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [features]
 default = ["python"]
 python = ["dep:pyo3", "common-error/python", "daft-core/python", "daft-dsl/python", "daft-table/python", "daft-stats/python", "common-io-config/python"]
 
 [package]
 edition = "2021"
 name = "daft-scan"
-version = "0.2.8"
+version = "0.2.9"
 
 [dependencies.snafu]
 version = "0.7.4"
 features = [ "futures",]
 
 [dependencies.tokio]
 version = "1.32.0"
```

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/anonymous.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/anonymous.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/expr_rewriter.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/expr_rewriter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/file_format.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/file_format.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/glob.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/glob.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/lib.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/py_object_serde.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/py_object_serde.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/python.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/scan_task_iters.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/scan_task_iters.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/local_dependencies/daft-scan/src/storage_config.rs` & `getdaft-0.2.9/local_dependencies/daft-scan/src/storage_config.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/Cargo.toml` & `getdaft-0.2.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 crate-type = [ "cdylib",]
 name = "daft"
 
 [package]
 edition = "2021"
 name = "daft"
 publish = false
-version = "0.2.8"
+version = "0.2.9"
 
 [workspace]
 members = ["local_dependencies/daft-core", "local_dependencies/daft-io", "local_dependencies/daft-parquet", "local_dependencies/daft-csv", "local_dependencies/daft-json", "local_dependencies/daft-dsl", "local_dependencies/daft-table", "local_dependencies/daft-plan", "local_dependencies/daft-micropartition", "local_dependencies/daft-scan"]
 
 [dependencies.common-daft-config]
 path = "local_dependencies/common-daft-config"
 default-features = false
@@ -103,15 +103,15 @@
 rstest = "0.18.2"
 serde_json = "1.0.108"
 tokio-util = "0.7.8"
 url = "2.4.0"
 
 [workspace.package]
 edition = "2021"
-version = "0.2.8"
+version = "0.2.9"
 
 [patch.crates-io.parquet2]
 git = "https://github.com/Eventual-Inc/parquet2"
 rev = "d4c24086c4cc824fbabef093ab2fda95d3aacb78"
 
 [workspace.dependencies.async-compression]
 version = "0.4.5"
```

### Comparing `getdaft-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/release-drafter.yml` & `getdaft-0.2.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/broken-link-checker.yml` & `getdaft-0.2.9/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/build-artifact-s3.yml` & `getdaft-0.2.9/.github/workflows/build-artifact-s3.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/daft-profiling.yml` & `getdaft-0.2.9/.github/workflows/daft-profiling.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/nightlies-tests.yml` & `getdaft-0.2.9/.github/workflows/nightlies-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/notebook-checker.yml` & `getdaft-0.2.9/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/property-based-tests.yml` & `getdaft-0.2.9/.github/workflows/property-based-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/python-package.yml` & `getdaft-0.2.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/python-publish.yml` & `getdaft-0.2.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/ray-compatibility.yml` & `getdaft-0.2.9/.github/workflows/ray-compatibility.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.github/workflows/release-drafter.yml` & `getdaft-0.2.9/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/.pre-commit-config.yaml` & `getdaft-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/CONTRIBUTING.md` & `getdaft-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/LICENSE` & `getdaft-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/Makefile` & `getdaft-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/README.rst` & `getdaft-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/parquet/README.md` & `getdaft-0.2.9/benchmarking/parquet/README.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/parquet/conftest.py` & `getdaft-0.2.9/benchmarking/parquet/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/parquet/test_bulk_reads.py` & `getdaft-0.2.9/benchmarking/parquet/test_bulk_reads.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/parquet/test_num_rowgroups.py` & `getdaft-0.2.9/benchmarking/parquet/test_num_rowgroups.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/__main__.py` & `getdaft-0.2.9/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/answers.py` & `getdaft-0.2.9/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/data_generation.py` & `getdaft-0.2.9/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.2.9/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/ray_job_runner.py` & `getdaft-0.2.9/benchmarking/tpch/ray_job_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/benchmarking/tpch/subprefix_s3_files.py` & `getdaft-0.2.9/benchmarking/tpch/subprefix_s3_files.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/ci/upload_wheels.sh` & `getdaft-0.2.9/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/__init__.py` & `getdaft-0.2.9/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/analytics.py` & `getdaft-0.2.9/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/api_annotations.py` & `getdaft-0.2.9/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/arrow_utils.py` & `getdaft-0.2.9/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/context.py` & `getdaft-0.2.9/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/convert.py` & `getdaft-0.2.9/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/daft.pyi` & `getdaft-0.2.9/daft/daft.pyi`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/dataframe/dataframe.py` & `getdaft-0.2.9/daft/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/dataframe/to_torch.py` & `getdaft-0.2.9/daft/dataframe/to_torch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/datatype.py` & `getdaft-0.2.9/daft/datatype.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/execution/execution_step.py` & `getdaft-0.2.9/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/execution/physical_plan.py` & `getdaft-0.2.9/daft/execution/physical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/execution/rust_physical_plan_shim.py` & `getdaft-0.2.9/daft/execution/rust_physical_plan_shim.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/expressions/expressions.py` & `getdaft-0.2.9/daft/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/expressions/testing.py` & `getdaft-0.2.9/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/filesystem.py` & `getdaft-0.2.9/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/iceberg/iceberg_scan.py` & `getdaft-0.2.9/daft/iceberg/iceberg_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/__init__.py` & `getdaft-0.2.9/daft/io/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/_csv.py` & `getdaft-0.2.9/daft/io/_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/_iceberg.py` & `getdaft-0.2.9/daft/io/_iceberg.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/_json.py` & `getdaft-0.2.9/daft/io/_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/_parquet.py` & `getdaft-0.2.9/daft/io/_parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/common.py` & `getdaft-0.2.9/daft/io/common.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/file_path.py` & `getdaft-0.2.9/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/io/scan.py` & `getdaft-0.2.9/daft/io/scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/logging.py` & `getdaft-0.2.9/daft/logging.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/logical/builder.py` & `getdaft-0.2.9/daft/logical/builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/logical/map_partition_ops.py` & `getdaft-0.2.9/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/logical/schema.py` & `getdaft-0.2.9/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/pickle/cloudpickle.py` & `getdaft-0.2.9/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/pickle/cloudpickle_fast.py` & `getdaft-0.2.9/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/pickle/compat.py` & `getdaft-0.2.9/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/plan_scheduler/physical_plan_scheduler.py` & `getdaft-0.2.9/daft/plan_scheduler/physical_plan_scheduler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/partitioning.py` & `getdaft-0.2.9/daft/runners/partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/profiler.py` & `getdaft-0.2.9/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/progress_bar.py` & `getdaft-0.2.9/daft/runners/progress_bar.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/pyrunner.py` & `getdaft-0.2.9/daft/runners/pyrunner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/ray_runner.py` & `getdaft-0.2.9/daft/runners/ray_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/runner.py` & `getdaft-0.2.9/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/runners/runner_io.py` & `getdaft-0.2.9/daft/runners/runner_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/series.py` & `getdaft-0.2.9/daft/series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/table/__init__.py` & `getdaft-0.2.9/daft/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/table/micropartition.py` & `getdaft-0.2.9/daft/table/micropartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/table/schema_inference.py` & `getdaft-0.2.9/daft/table/schema_inference.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/table/table.py` & `getdaft-0.2.9/daft/table/table.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/table/table_io.py` & `getdaft-0.2.9/daft/table/table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/udf.py` & `getdaft-0.2.9/daft/udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/udf_library/url_udfs.py` & `getdaft-0.2.9/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/utils.py` & `getdaft-0.2.9/daft/utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/viz/dataframe_display.py` & `getdaft-0.2.9/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/daft/viz/html_viz_hooks.py` & `getdaft-0.2.9/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/Makefile` & `getdaft-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/10-min.ipynb` & `getdaft-0.2.9/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/daft-favicon.png` & `getdaft-0.2.9/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/daft-logo.png` & `getdaft-0.2.9/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/daft_illustration.png` & `getdaft-0.2.9/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/dataframe-comp-table.csv` & `getdaft-0.2.9/docs/source/_static/dataframe-comp-table.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/execution_model.png` & `getdaft-0.2.9/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/header.css` & `getdaft-0.2.9/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/high_level_architecture.png` & `getdaft-0.2.9/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.2.9/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/mobile-menu.js` & `getdaft-0.2.9/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/tpch-1000sf.html` & `getdaft-0.2.9/docs/source/_static/tpch-1000sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/tpch-100sf.html` & `getdaft-0.2.9/docs/source/_static/tpch-100sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html` & `getdaft-0.2.9/docs/source/_static/tpch-nodes-count-daft-1000-sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_templates/layout.html` & `getdaft-0.2.9/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_templates/sections/header.html` & `getdaft-0.2.9/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.2.9/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/context.rst` & `getdaft-0.2.9/docs/source/api_docs/context.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/dataframe.rst` & `getdaft-0.2.9/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/datatype.rst` & `getdaft-0.2.9/docs/source/api_docs/datatype.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/expressions.rst` & `getdaft-0.2.9/docs/source/api_docs/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/groupby.rst` & `getdaft-0.2.9/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/api_docs/input_output.rst` & `getdaft-0.2.9/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/benchmarks/index.rst` & `getdaft-0.2.9/docs/source/benchmarks/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/conf.py` & `getdaft-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/dataframe_comparison.rst` & `getdaft-0.2.9/docs/source/dataframe_comparison.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/index.rst` & `getdaft-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/install.rst` & `getdaft-0.2.9/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/index.rst` & `getdaft-0.2.9/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/key_concepts.rst` & `getdaft-0.2.9/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/tutorials.rst` & `getdaft-0.2.9/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/datatypes.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/datatypes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/memory.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/memory.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides/udf.rst` & `getdaft-0.2.9/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/learn/user_guides.rst` & `getdaft-0.2.9/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/technical_architecture.rst` & `getdaft-0.2.9/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/docs/source/telemetry.rst` & `getdaft-0.2.9/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/pyproject.toml` & `getdaft-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/requirements-dev.txt` & `getdaft-0.2.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/src/lib.rs` & `getdaft-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/parquet-data/mvp.parquet` & `getdaft-0.2.9/tests/assets/parquet-data/mvp.parquet`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/parquet-data/parquet-with-schema-metadata.parquet` & `getdaft-0.2.9/tests/assets/parquet-data/parquet-with-schema-metadata.parquet`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/parquet-data/sampled-tpch-with-stats.parquet` & `getdaft-0.2.9/tests/assets/parquet-data/sampled-tpch-with-stats.parquet`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/sampled-tpch.csv` & `getdaft-0.2.9/tests/assets/sampled-tpch.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/sampled-tpch.jsonl` & `getdaft-0.2.9/tests/assets/sampled-tpch.jsonl`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.2.9/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/conftest.py` & `getdaft-0.2.9/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.2.9/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_file_read.py` & `getdaft-0.2.9/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_filter.py` & `getdaft-0.2.9/tests/benchmarks/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.2.9/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_if_else.py` & `getdaft-0.2.9/tests/benchmarks/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_join.py` & `getdaft-0.2.9/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_repartition.py` & `getdaft-0.2.9/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_sort.py` & `getdaft-0.2.9/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/benchmarks/test_take.py` & `getdaft-0.2.9/tests/benchmarks/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/conftest.py` & `getdaft-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.2.9/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/assets/images/0000.jpg` & `getdaft-0.2.9/tests/cookbook/assets/images/0000.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/assets/images/0007.jpg` & `getdaft-0.2.9/tests/cookbook/assets/images/0007.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/assets/images/0018.png` & `getdaft-0.2.9/tests/cookbook/assets/images/0018.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/assets/images/0025.tiff` & `getdaft-0.2.9/tests/cookbook/assets/images/0025.tiff`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/conftest.py` & `getdaft-0.2.9/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_aggregations.py` & `getdaft-0.2.9/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_computations.py` & `getdaft-0.2.9/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_count_rows.py` & `getdaft-0.2.9/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_dataloading.py` & `getdaft-0.2.9/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_distinct.py` & `getdaft-0.2.9/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_filter.py` & `getdaft-0.2.9/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_image.py` & `getdaft-0.2.9/tests/cookbook/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_joins.py` & `getdaft-0.2.9/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_literals.py` & `getdaft-0.2.9/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.2.9/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_sorting.py` & `getdaft-0.2.9/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/cookbook/test_write.py` & `getdaft-0.2.9/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/conftest.py` & `getdaft-0.2.9/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_accessors.py` & `getdaft-0.2.9/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_aggregations.py` & `getdaft-0.2.9/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_concat.py` & `getdaft-0.2.9/tests/dataframe/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_creation.py` & `getdaft-0.2.9/tests/dataframe/test_creation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_decimals.py` & `getdaft-0.2.9/tests/dataframe/test_decimals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_distinct.py` & `getdaft-0.2.9/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_explode.py` & `getdaft-0.2.9/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_filter.py` & `getdaft-0.2.9/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_getitem.py` & `getdaft-0.2.9/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_iter.py` & `getdaft-0.2.9/tests/dataframe/test_iter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_joins.py` & `getdaft-0.2.9/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_logical_type.py` & `getdaft-0.2.9/tests/dataframe/test_logical_type.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_repr.py` & `getdaft-0.2.9/tests/dataframe/test_repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_select.py` & `getdaft-0.2.9/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_show.py` & `getdaft-0.2.9/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_sort.py` & `getdaft-0.2.9/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_temporals.py` & `getdaft-0.2.9/tests/dataframe/test_temporals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_to_integrations.py` & `getdaft-0.2.9/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/dataframe/test_with_column.py` & `getdaft-0.2.9/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/test_apply.py` & `getdaft-0.2.9/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/test_expressions.py` & `getdaft-0.2.9/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/test_expressions_projection.py` & `getdaft-0.2.9/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/test_udf.py` & `getdaft-0.2.9/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/conftest.py` & `getdaft-0.2.9/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_aggs.py` & `getdaft-0.2.9/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.2.9/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_compare.py` & `getdaft-0.2.9/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_dt.py` & `getdaft-0.2.9/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_float.py` & `getdaft-0.2.9/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_if_else.py` & `getdaft-0.2.9/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_logical.py` & `getdaft-0.2.9/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/expressions/typing/test_str.py` & `getdaft-0.2.9/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/conftest.py` & `getdaft-0.2.9/tests/integration/iceberg/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/Dockerfile` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/Dockerfile`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/check-license` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/check-license`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose-azurite.yml` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose-azurite.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose-gcs-server.yml` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose-gcs-server.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/docker-compose.yml` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/entrypoint.sh` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/provision.py` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/provision.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-azurite.sh` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-azurite.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-gcs-server.sh` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-gcs-server.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/run-minio.sh` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/run-minio.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/docker-compose/spark-defaults.conf` & `getdaft-0.2.9/tests/integration/iceberg/docker-compose/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/test_partition_pruning.py` & `getdaft-0.2.9/tests/integration/iceberg/test_partition_pruning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/iceberg/test_table_load.py` & `getdaft-0.2.9/tests/integration/iceberg/test_table_load.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/benchmarks/test_benchmark_glob.py` & `getdaft-0.2.9/tests/integration/io/benchmarks/test_benchmark_glob.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/conftest.py` & `getdaft-0.2.9/tests/integration/io/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,8 +223,10 @@
     with mount_data_minio(minio_io_config, image_data_folder) as urls:
         yield urls
 
 
 @pytest.fixture(scope="session")
 def small_images_s3_paths() -> list[str]:
     """Paths to small *.jpg files in a public S3 bucket"""
-    return [f"s3://daft-public-data/test_fixtures/small_images/rickroll{i}.jpg" for i in range(6)]
+    return [f"s3://daft-public-data/test_fixtures/small_images/rickroll{i}.jpg" for i in range(6)] + [
+        f"s3a://daft-public-data/test_fixtures/small_images/rickroll{i}.jpg" for i in range(6)
+    ]
```

### Comparing `getdaft-0.2.8/tests/integration/io/csv/test_read_pushdowns.py` & `getdaft-0.2.9/tests/integration/io/csv/test_read_pushdowns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/docker-compose.yml` & `getdaft-0.2.9/tests/integration/io/docker-compose/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/nginx-serve-static-files.conf` & `getdaft-0.2.9/tests/integration/io/docker-compose/nginx-serve-static-files.conf`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/main.py` & `getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/main.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/get_retries_parquet_bucket.py` & `getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/get_retries_parquet_bucket.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/head_retries_parquet_bucket.py` & `getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/head_retries_parquet_bucket.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/docker-compose/retry_server/routers/rate_limited_echo_gets_bucket.py` & `getdaft-0.2.9/tests/integration/io/docker-compose/retry_server/routers/rate_limited_echo_gets_bucket.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/jsonl/test_read_pushdown.py` & `getdaft-0.2.9/tests/integration/io/jsonl/test_read_pushdown.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/parquet/test_read_pushdowns.py` & `getdaft-0.2.9/tests/integration/io/parquet/test_read_pushdowns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/parquet/test_reads_local_fixtures.py` & `getdaft-0.2.9/tests/integration/io/parquet/test_reads_local_fixtures.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/parquet/test_reads_public_data.py` & `getdaft-0.2.9/tests/integration/io/parquet/test_reads_public_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,18 @@
     #     "s3://eventual-dev-benchmarking-fixtures/uncompressed/tpch-dbgen/100_0/32/parquet/lineitem/108417bd-5bee-43d9-bf9a-d6faec6afb2d-0.parquet",
     # ),
     (
         "parquet-benchmarking/mvp",
         "s3://daft-public-data/test_fixtures/parquet-dev/mvp.parquet",
     ),
     (
+        "parquet-benchmarking/s3a-mvp",
+        "s3a://daft-public-data/test_fixtures/parquet-dev/mvp.parquet",
+    ),
+    (
         "azure/mvp",
         "az://public-anonymous/mvp.parquet",
     ),
     (
         "gcs/mvp",
         "gs://daft-public-data-gs/mvp.parquet",
     ),
@@ -194,15 +198,15 @@
 def parquet_file(request) -> tuple[str, str]:
     """Returns a tuple of (`name`, `url`) of files that Daft should be able to handle. URLs may be HTTPs or S3."""
     return request.param
 
 
 def read_parquet_with_pyarrow(path) -> pa.Table:
     kwargs = {}
-    if get_protocol_from_path(path) == "s3":
+    if get_protocol_from_path(path) == "s3" or get_protocol_from_path(path) == "s3a":
         kwargs["anon"] = True
     if get_protocol_from_path(path) == "az":
         kwargs["account_name"] = "dafttestdata"
         kwargs["anon"] = True
 
     fs = get_filesystem_from_path(path, **kwargs)
     table = pq.read_table(path, filesystem=fs)
```

### Comparing `getdaft-0.2.8/tests/integration/io/parquet/test_reads_s3_minio.py` & `getdaft-0.2.9/tests/integration/io/parquet/test_reads_s3_minio.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_list_files_azure.py` & `getdaft-0.2.9/tests/integration/io/test_list_files_azure.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_list_files_gcs.py` & `getdaft-0.2.9/tests/integration/io/test_list_files_gcs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_list_files_http.py` & `getdaft-0.2.9/tests/integration/io/test_list_files_http.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_list_files_s3_minio.py` & `getdaft-0.2.9/tests/integration/io/test_list_files_s3_minio.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 @pytest.mark.integration()
 @pytest.mark.parametrize(
     "path_expect_pair",
     [
         # Exact filepath:
         (f"s3://bucket/a.match", [{"type": "File", "path": "s3://bucket/a.match", "size": 0}]),
+        # Exact filepath but with s3a:
+        (f"s3a://bucket/a.match", [{"type": "File", "path": "s3a://bucket/a.match", "size": 0}]),
         ###
         # `**`: recursive wildcard
         ###
         # All files with **
         (
             f"s3://bucket/**",
             [
@@ -51,14 +53,29 @@
                 {"type": "File", "path": "s3://bucket/nested1/b.nomatch", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested1/c.match", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested2/a.match", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested2/b.nomatch", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested2/c.match", "size": 0},
             ],
         ),
+        # All files with s3a and **
+        (
+            f"s3a://bucket/**",
+            [
+                {"type": "File", "path": "s3a://bucket/a.match", "size": 0},
+                {"type": "File", "path": "s3a://bucket/b.nomatch", "size": 0},
+                {"type": "File", "path": "s3a://bucket/c.match", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested1/a.match", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested1/b.nomatch", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested1/c.match", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested2/a.match", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested2/b.nomatch", "size": 0},
+                {"type": "File", "path": "s3a://bucket/nested2/c.match", "size": 0},
+            ],
+        ),
         # Exact filepath after **
         (
             f"s3://bucket/**/a.match",
             [
                 {"type": "File", "path": "s3://bucket/a.match", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested1/a.match", "size": 0},
                 {"type": "File", "path": "s3://bucket/nested2/a.match", "size": 0},
```

### Comparing `getdaft-0.2.8/tests/integration/io/test_url_download_http.py` & `getdaft-0.2.9/tests/integration/io/test_url_download_http.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_url_download_private_aws_s3.py` & `getdaft-0.2.9/tests/integration/io/test_url_download_private_aws_s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 @pytest.mark.integration()
 def test_url_download_aws_s3_public_bucket_with_creds(small_images_s3_paths, io_config):
     data = {"urls": small_images_s3_paths}
     df = daft.from_pydict(data)
     df = df.with_column("data", df["urls"].url.download(use_native_downloader=True, io_config=io_config))
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
 
 
 @pytest.mark.integration()
 def test_read_parquet_aws_s3_public_bucket_with_creds(io_config):
     filename = "s3://daft-public-data/test_fixtures/parquet-dev/mvp.parquet"
```

### Comparing `getdaft-0.2.8/tests/integration/io/test_url_download_public_aws_s3.py` & `getdaft-0.2.9/tests/integration/io/test_url_download_public_aws_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,63 +10,63 @@
     data = {"urls": small_images_s3_paths}
     df = daft.from_pydict(data)
     df = df.with_column(
         "data", df["urls"].url.download(io_config=daft.io.IOConfig(s3=daft.io.S3Config(anonymous=True)))
     )
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
 
 
 @pytest.mark.integration()
 def test_url_download_aws_s3_public_bucket_custom_s3fs_wrong_region(small_images_s3_paths):
     data = {"urls": small_images_s3_paths}
     df = daft.from_pydict(data)
     df = df.with_column(
         "data", df["urls"].url.download(io_config=daft.io.IOConfig(s3=daft.io.S3Config(anonymous=True)))
     )
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
 
 
 @pytest.mark.integration()
 def test_url_download_aws_s3_public_bucket_native_downloader(aws_public_s3_config, small_images_s3_paths):
     data = {"urls": small_images_s3_paths}
     df = daft.from_pydict(data)
     df = df.with_column("data", df["urls"].url.download(io_config=aws_public_s3_config, use_native_downloader=True))
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
 
 
 @pytest.mark.integration()
 def test_url_download_aws_s3_public_bucket_native_downloader_io_thread_change(
     aws_public_s3_config, small_images_s3_paths
 ):
     data = {"urls": small_images_s3_paths}
     df = daft.from_pydict(data)
     df = df.with_column("data", df["urls"].url.download(io_config=aws_public_s3_config, use_native_downloader=True))
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
     daft.io.set_io_pool_num_threads(2)
     df = daft.from_pydict(data)
     df = df.with_column("data", df["urls"].url.download(io_config=aws_public_s3_config, use_native_downloader=True))
 
     data = df.to_pydict()
-    assert len(data["data"]) == 6
+    assert len(data["data"]) == 12
     for img_bytes in data["data"]:
         assert img_bytes is not None
 
 
 @pytest.mark.integration()
 def test_url_download_aws_s3_public_bucket_native_downloader_with_connect_timeout(small_images_s3_paths):
     data = {"urls": small_images_s3_paths}
```

### Comparing `getdaft-0.2.8/tests/integration/io/test_url_download_public_azure.py` & `getdaft-0.2.9/tests/integration/io/test_url_download_public_azure.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_url_download_s3_local_retry_server.py` & `getdaft-0.2.9/tests/integration/io/test_url_download_s3_local_retry_server.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/io/test_write_files_s3_minio.py` & `getdaft-0.2.9/tests/integration/io/test_write_files_s3_minio.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/integration/test_tpch.py` & `getdaft-0.2.9/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/io/test_csv_roundtrip.py` & `getdaft-0.2.9/tests/io/test_csv_roundtrip.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/io/test_list_files_local.py` & `getdaft-0.2.9/tests/io/test_list_files_local.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/io/test_merge_scan_tasks.py` & `getdaft-0.2.9/tests/io/test_merge_scan_tasks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/io/test_parquet_roundtrip.py` & `getdaft-0.2.9/tests/io/test_parquet_roundtrip.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/io/test_url_download_local.py` & `getdaft-0.2.9/tests/io/test_url_download_local.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/property_based_testing/strategies.py` & `getdaft-0.2.9/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/property_based_testing/test_sort.py` & `getdaft-0.2.9/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/ray/runner.py` & `getdaft-0.2.9/tests/ray/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/ray/test_dask.py` & `getdaft-0.2.9/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/ray/test_datasets.py` & `getdaft-0.2.9/tests/ray/test_datasets.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_arithmetic.py` & `getdaft-0.2.9/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_cast.py` & `getdaft-0.2.9/tests/series/test_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_comparisons.py` & `getdaft-0.2.9/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_concat.py` & `getdaft-0.2.9/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_embedding.py` & `getdaft-0.2.9/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_filter.py` & `getdaft-0.2.9/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_float.py` & `getdaft-0.2.9/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_hash.py` & `getdaft-0.2.9/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_if_else.py` & `getdaft-0.2.9/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_image.py` & `getdaft-0.2.9/tests/series/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_numeric_ops.py` & `getdaft-0.2.9/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_partitioning.py` & `getdaft-0.2.9/tests/series/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_series.py` & `getdaft-0.2.9/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_size_bytes.py` & `getdaft-0.2.9/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_slice.py` & `getdaft-0.2.9/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_sort.py` & `getdaft-0.2.9/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_take.py` & `getdaft-0.2.9/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_temporal_ops.py` & `getdaft-0.2.9/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_tensor.py` & `getdaft-0.2.9/tests/series/test_tensor.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/series/test_utf8_ops.py` & `getdaft-0.2.9/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/__init__.py` & `getdaft-0.2.9/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/image/test_crop.py` & `getdaft-0.2.9/tests/table/image/test_crop.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/list/test_list_join.py` & `getdaft-0.2.9/tests/table/list/test_list_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/table_io/test_csv.py` & `getdaft-0.2.9/tests/table/table_io/test_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/table_io/test_json.py` & `getdaft-0.2.9/tests/table/table_io/test_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/table_io/test_parquet.py` & `getdaft-0.2.9/tests/table/table_io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/table_io/test_read_time_cast.py` & `getdaft-0.2.9/tests/table/table_io/test_read_time_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_blackbox_kernels.py` & `getdaft-0.2.9/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_broadcasts.py` & `getdaft-0.2.9/tests/table/test_broadcasts.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_concat.py` & `getdaft-0.2.9/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_eval.py` & `getdaft-0.2.9/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_explodes.py` & `getdaft-0.2.9/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_filter.py` & `getdaft-0.2.9/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_from_py.py` & `getdaft-0.2.9/tests/table/test_from_py.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_head.py` & `getdaft-0.2.9/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_joins.py` & `getdaft-0.2.9/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_micropartition.py` & `getdaft-0.2.9/tests/table/test_micropartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_partitioning.py` & `getdaft-0.2.9/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_size_bytes.py` & `getdaft-0.2.9/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_sorting.py` & `getdaft-0.2.9/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_table_aggs.py` & `getdaft-0.2.9/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/test_take.py` & `getdaft-0.2.9/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/utf8/test_compares.py` & `getdaft-0.2.9/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/table/utf8/test_split.py` & `getdaft-0.2.9/tests/table/utf8/test_split.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/test_analytics.py` & `getdaft-0.2.9/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/test_datatypes.py` & `getdaft-0.2.9/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/test_resource_requests.py` & `getdaft-0.2.9/tests/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/test_schema.py` & `getdaft-0.2.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tests/udf_library/test_url_udfs.py` & `getdaft-0.2.9/tests/udf_library/test_url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tools/generate_whl_html_manifest.py` & `getdaft-0.2.9/tools/generate_whl_html_manifest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tools/patch_package_version.py` & `getdaft-0.2.9/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.2.9/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/flyte/README.md` & `getdaft-0.2.9/tutorials/flyte/README.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/flyte/app.py` & `getdaft-0.2.9/tutorials/flyte/app.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/flyte/notebook.ipynb` & `getdaft-0.2.9/tutorials/flyte/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.2.9/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/intro.ipynb` & `getdaft-0.2.9/tutorials/intro.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/mnist.ipynb` & `getdaft-0.2.9/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/talks_and_demos/pydata_global_2023.ipynb` & `getdaft-0.2.9/tutorials/talks_and_demos/pydata_global_2023.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.2.9/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.2.9/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.2.8/Cargo.lock` & `getdaft-0.2.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -906,45 +906,45 @@
  "strum",
  "strum_macros",
  "unicode-width",
 ]
 
 [[package]]
 name = "common-daft-config"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bincode",
  "common-io-config",
  "lazy_static",
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "common-error"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "pyo3",
  "serde_json",
 ]
 
 [[package]]
 name = "common-io-config"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "common-error",
  "pyo3",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "common-treenode"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "common-error",
  "pyo3",
 ]
 
 [[package]]
 name = "concurrent-queue"
@@ -1103,15 +1103,15 @@
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "common-daft-config",
  "daft-compression",
  "daft-core",
  "daft-csv",
  "daft-dsl",
  "daft-io",
@@ -1126,24 +1126,24 @@
  "pyo3",
  "pyo3-log",
  "tikv-jemallocator",
 ]
 
 [[package]]
 name = "daft-compression"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "async-compression",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "daft-core"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "base64 0.21.5",
  "bincode",
  "chrono",
  "chrono-tz",
  "comfy-table",
@@ -1165,15 +1165,15 @@
  "serde",
  "serde_json",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "daft-csv"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "async-compat",
  "async-compression",
  "async-stream",
  "bincode",
  "bytes",
@@ -1201,15 +1201,15 @@
  "tokio-stream",
  "tokio-util",
  "url",
 ]
 
 [[package]]
 name = "daft-decoding"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "async-compression",
  "atoi_simd",
  "chrono",
  "chrono-tz",
  "csv-async",
@@ -1217,15 +1217,15 @@
  "simdutf8",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "daft-dsl"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bincode",
  "common-error",
  "common-io-config",
  "common-treenode",
  "daft-core",
  "daft-io",
@@ -1234,15 +1234,15 @@
  "pyo3-log",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "daft-io"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "async-recursion",
  "async-stream",
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "aws-sdk-s3",
@@ -1278,15 +1278,15 @@
  "tokio",
  "tokio-stream",
  "url",
 ]
 
 [[package]]
 name = "daft-json"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "async-compat",
  "async-compression",
  "async-stream",
  "bincode",
  "bytes",
@@ -1316,15 +1316,15 @@
  "tokio-stream",
  "tokio-util",
  "url",
 ]
 
 [[package]]
 name = "daft-micropartition"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "bincode",
  "common-error",
  "daft-core",
  "daft-csv",
  "daft-dsl",
@@ -1341,15 +1341,15 @@
  "pyo3-log",
  "serde",
  "snafu",
 ]
 
 [[package]]
 name = "daft-parquet"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "async-compat",
  "async-stream",
  "bytes",
  "common-error",
  "daft-core",
@@ -1370,15 +1370,15 @@
  "tokio",
  "tokio-stream",
  "tokio-util",
 ]
 
 [[package]]
 name = "daft-plan"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "bincode",
  "common-daft-config",
  "common-error",
  "common-io-config",
  "common-treenode",
@@ -1395,15 +1395,15 @@
  "serde",
  "serde_json",
  "snafu",
 ]
 
 [[package]]
 name = "daft-scan"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "bincode",
  "common-error",
  "common-io-config",
  "daft-core",
  "daft-csv",
  "daft-dsl",
@@ -1419,30 +1419,30 @@
  "serde_json",
  "snafu",
  "tokio",
 ]
 
 [[package]]
 name = "daft-stats"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "common-error",
  "daft-core",
  "daft-dsl",
  "daft-table",
  "indexmap 2.1.0",
  "pyo3",
  "pyo3-log",
  "serde",
  "snafu",
 ]
 
 [[package]]
 name = "daft-table"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "arrow2",
  "comfy-table",
  "common-error",
  "daft-core",
  "daft-dsl",
  "html-escape",
```

### Comparing `getdaft-0.2.8/PKG-INFO` & `getdaft-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.2.8
+Version: 0.2.9
 Requires-Dist: pyarrow >=6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions >=4.0.0 ; python_version < '3.10'
 Requires-Dist: pickle5 >=0.0.12 ; python_version < '3.8'
 Requires-Dist: getdaft[aws,azure,gcp,ray,pandas,numpy,iceberg] ; extra == 'all'
```

