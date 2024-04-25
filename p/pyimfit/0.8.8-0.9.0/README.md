# Comparing `tmp/pyimfit-0.8.8.tar.gz` & `tmp/pyimfit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyimfit-0.8.8.tar", last modified: Mon Aug 26 08:51:32 2019, max compression
+gzip compressed data, was "dist/pyimfit-0.9.0.tar", last modified: Thu Jun  4 12:20:42 2020, max compression
```

## Comparing `pyimfit-0.8.8.tar` & `pyimfit-0.9.0.tar`

### file list

```diff
@@ -1,314 +1,314 @@
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/
--rw-r--r--   0 erwin      (502) staff       (20)      357 2019-07-27 20:05:11.000000 pyimfit-0.8.8/MANIFEST.in
--rw-r--r--   0 erwin      (502) staff       (20)     2578 2019-08-26 08:51:32.000000 pyimfit-0.8.8/PKG-INFO
--rw-r--r--   0 erwin      (502) staff       (20)     6294 2019-08-20 20:31:02.000000 pyimfit-0.8.8/README.md
--rw-r--r--   0 erwin      (502) staff       (20)     1532 2019-08-26 08:31:24.000000 pyimfit-0.8.8/README_pyimfit.md
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/extra_libs/
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/extra_libs/include/
--rw-r--r--   0 erwin      (502) staff       (20)    17900 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/fftw3.h
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/extra_libs/include/gsl/
--rw-r--r--   0 erwin      (502) staff       (20)    21934 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_blas.h
--rw-r--r--   0 erwin      (502) staff       (20)     1579 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_blas_types.h
--rw-r--r--   0 erwin      (502) staff       (20)      580 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block.h
--rw-r--r--   0 erwin      (502) staff       (20)     2290 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     2417 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     2557 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     2767 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     2185 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     2325 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     2255 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     2290 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     2535 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     2325 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     2373 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     2338 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     2373 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     2408 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     3473 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_bspline.h
--rw-r--r--   0 erwin      (502) staff       (20)    33677 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_cblas.h
--rw-r--r--   0 erwin      (502) staff       (20)     7373 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_cdf.h
--rw-r--r--   0 erwin      (502) staff       (20)     4509 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_chebyshev.h
--rw-r--r--   0 erwin      (502) staff       (20)     1579 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_check_range.h
--rw-r--r--   0 erwin      (502) staff       (20)     2866 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_combination.h
--rw-r--r--   0 erwin      (502) staff       (20)     3374 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_complex.h
--rw-r--r--   0 erwin      (502) staff       (20)     6048 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_complex_math.h
--rw-r--r--   0 erwin      (502) staff       (20)     1056 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const.h
--rw-r--r--   0 erwin      (502) staff       (20)     6232 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_cgs.h
--rw-r--r--   0 erwin      (502) staff       (20)     6779 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_cgsm.h
--rw-r--r--   0 erwin      (502) staff       (20)     6929 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_mks.h
--rw-r--r--   0 erwin      (502) staff       (20)     7034 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_mksa.h
--rw-r--r--   0 erwin      (502) staff       (20)     1761 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_num.h
--rw-r--r--   0 erwin      (502) staff       (20)     1564 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_deriv.h
--rw-r--r--   0 erwin      (502) staff       (20)     1814 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_dft_complex.h
--rw-r--r--   0 erwin      (502) staff       (20)     1854 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_dft_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     2629 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_dht.h
--rw-r--r--   0 erwin      (502) staff       (20)     1558 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_diff.h
--rw-r--r--   0 erwin      (502) staff       (20)    13274 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_eigen.h
--rw-r--r--   0 erwin      (502) staff       (20)     5965 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_errno.h
--rw-r--r--   0 erwin      (502) staff       (20)     1402 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft.h
--rw-r--r--   0 erwin      (502) staff       (20)     4830 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_complex.h
--rw-r--r--   0 erwin      (502) staff       (20)     5349 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     3028 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_halfcomplex.h
--rw-r--r--   0 erwin      (502) staff       (20)     3234 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_halfcomplex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     2232 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_real.h
--rw-r--r--   0 erwin      (502) staff       (20)     2382 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_real_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     4147 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_filter.h
--rw-r--r--   0 erwin      (502) staff       (20)     2764 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_fit.h
--rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_heapsort.h
--rw-r--r--   0 erwin      (502) staff       (20)     4140 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_histogram.h
--rw-r--r--   0 erwin      (502) staff       (20)     5642 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_histogram2d.h
--rw-r--r--   0 erwin      (502) staff       (20)     2715 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_ieee_utils.h
--rw-r--r--   0 erwin      (502) staff       (20)     2463 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_inline.h
--rw-r--r--   0 erwin      (502) staff       (20)    13855 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_integration.h
--rw-r--r--   0 erwin      (502) staff       (20)     6961 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_interp.h
--rw-r--r--   0 erwin      (502) staff       (20)     8795 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_interp2d.h
--rw-r--r--   0 erwin      (502) staff       (20)    28560 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_linalg.h
--rw-r--r--   0 erwin      (502) staff       (20)     3805 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_machine.h
--rw-r--r--   0 erwin      (502) staff       (20)     4345 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_math.h
--rw-r--r--   0 erwin      (502) staff       (20)      598 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix.h
--rw-r--r--   0 erwin      (502) staff       (20)    12323 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_char.h
--rw-r--r--   0 erwin      (502) staff       (20)    12844 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)    14076 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)    15378 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)    11363 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_double.h
--rw-r--r--   0 erwin      (502) staff       (20)    12550 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_float.h
--rw-r--r--   0 erwin      (502) staff       (20)    12096 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_int.h
--rw-r--r--   0 erwin      (502) staff       (20)    12323 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_long.h
--rw-r--r--   0 erwin      (502) staff       (20)    13912 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)    12550 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_short.h
--rw-r--r--   0 erwin      (502) staff       (20)    12710 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)    12483 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)    12710 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)    12937 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     2420 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_message.h
--rw-r--r--   0 erwin      (502) staff       (20)     4039 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_min.h
--rw-r--r--   0 erwin      (502) staff       (20)     2632 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_minmax.h
--rw-r--r--   0 erwin      (502) staff       (20)     2405 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_mode.h
--rw-r--r--   0 erwin      (502) staff       (20)     1601 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte.h
--rw-r--r--   0 erwin      (502) staff       (20)     2662 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_miser.h
--rw-r--r--   0 erwin      (502) staff       (20)     1884 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_plain.h
--rw-r--r--   0 erwin      (502) staff       (20)     3234 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_vegas.h
--rw-r--r--   0 erwin      (502) staff       (20)     6083 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_movstat.h
--rw-r--r--   0 erwin      (502) staff       (20)    14549 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit.h
--rw-r--r--   0 erwin      (502) staff       (20)    11357 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit_nlin.h
--rw-r--r--   0 erwin      (502) staff       (20)    12064 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit_nlinear.h
--rw-r--r--   0 erwin      (502) staff       (20)     5411 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multilarge.h
--rw-r--r--   0 erwin      (502) staff       (20)    12990 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multilarge_nlinear.h
--rw-r--r--   0 erwin      (502) staff       (20)     6795 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multimin.h
--rw-r--r--   0 erwin      (502) staff       (20)     6152 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multiroots.h
--rw-r--r--   0 erwin      (502) staff       (20)     2784 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_multiset.h
--rw-r--r--   0 erwin      (502) staff       (20)     1335 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_nan.h
--rw-r--r--   0 erwin      (502) staff       (20)     2149 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_ntuple.h
--rw-r--r--   0 erwin      (502) staff       (20)     7760 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_odeiv.h
--rw-r--r--   0 erwin      (502) staff       (20)    13781 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_odeiv2.h
--rw-r--r--   0 erwin      (502) staff       (20)     3346 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permutation.h
--rw-r--r--   0 erwin      (502) staff       (20)      614 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute.h
--rw-r--r--   0 erwin      (502) staff       (20)     1430 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     1509 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1515 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1563 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1432 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1438 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1422 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1430 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     1486 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)      733 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix.h
--rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     1407 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1414 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1456 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1344 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     1400 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     1365 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     1438 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     1446 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     1462 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)      733 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector.h
--rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     1527 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1546 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1600 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1455 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1456 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     1528 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     1483 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     5408 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_poly.h
--rw-r--r--   0 erwin      (502) staff       (20)     2301 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_pow_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1780 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_precision.h
--rw-r--r--   0 erwin      (502) staff       (20)     2355 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_qrng.h
--rw-r--r--   0 erwin      (502) staff       (20)    10347 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_randist.h
--rw-r--r--   0 erwin      (502) staff       (20)     6957 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_rng.h
--rw-r--r--   0 erwin      (502) staff       (20)     3728 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_roots.h
--rw-r--r--   0 erwin      (502) staff       (20)     2896 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_rstat.h
--rw-r--r--   0 erwin      (502) staff       (20)     1106 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf.h
--rw-r--r--   0 erwin      (502) staff       (20)     3709 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_airy.h
--rw-r--r--   0 erwin      (502) staff       (20)    14165 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_bessel.h
--rw-r--r--   0 erwin      (502) staff       (20)     1467 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_clausen.h
--rw-r--r--   0 erwin      (502) staff       (20)     4402 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_coulomb.h
--rw-r--r--   0 erwin      (502) staff       (20)     4165 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_coupling.h
--rw-r--r--   0 erwin      (502) staff       (20)     1402 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_dawson.h
--rw-r--r--   0 erwin      (502) staff       (20)     2303 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_debye.h
--rw-r--r--   0 erwin      (502) staff       (20)     4171 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_dilog.h
--rw-r--r--   0 erwin      (502) staff       (20)     1657 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_elementary.h
--rw-r--r--   0 erwin      (502) staff       (20)     4159 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_ellint.h
--rw-r--r--   0 erwin      (502) staff       (20)     1364 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_elljac.h
--rw-r--r--   0 erwin      (502) staff       (20)     2295 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_erf.h
--rw-r--r--   0 erwin      (502) staff       (20)     3847 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_exp.h
--rw-r--r--   0 erwin      (502) staff       (20)     4397 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_expint.h
--rw-r--r--   0 erwin      (502) staff       (20)     3413 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_fermi_dirac.h
--rw-r--r--   0 erwin      (502) staff       (20)     7750 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_gamma.h
--rw-r--r--   0 erwin      (502) staff       (20)     2154 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_gegenbauer.h
--rw-r--r--   0 erwin      (502) staff       (20)     4030 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_hermite.h
--rw-r--r--   0 erwin      (502) staff       (20)     4517 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_hyperg.h
--rw-r--r--   0 erwin      (502) staff       (20)     2000 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_laguerre.h
--rw-r--r--   0 erwin      (502) staff       (20)     1813 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_lambert.h
--rw-r--r--   0 erwin      (502) staff       (20)    11891 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_legendre.h
--rw-r--r--   0 erwin      (502) staff       (20)     2062 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_log.h
--rw-r--r--   0 erwin      (502) staff       (20)     4307 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_mathieu.h
--rw-r--r--   0 erwin      (502) staff       (20)     1390 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_pow_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     2683 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_psi.h
--rw-r--r--   0 erwin      (502) staff       (20)     1577 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_result.h
--rw-r--r--   0 erwin      (502) staff       (20)     1672 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_sincos_pi.h
--rw-r--r--   0 erwin      (502) staff       (20)     1723 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_synchrotron.h
--rw-r--r--   0 erwin      (502) staff       (20)     1978 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_transport.h
--rw-r--r--   0 erwin      (502) staff       (20)     3957 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_trig.h
--rw-r--r--   0 erwin      (502) staff       (20)     2894 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_zeta.h
--rw-r--r--   0 erwin      (502) staff       (20)     3018 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_siman.h
--rw-r--r--   0 erwin      (502) staff       (20)      435 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort.h
--rw-r--r--   0 erwin      (502) staff       (20)     1974 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     1967 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1995 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1953 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1974 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     2121 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1995 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     2075 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     2054 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     2075 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     2096 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)      533 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector.h
--rw-r--r--   0 erwin      (502) staff       (20)     1878 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     1817 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1900 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     1856 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     1878 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     2032 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     1900 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     1916 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     1894 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     1916 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     1938 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     1809 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_spblas.h
--rw-r--r--   0 erwin      (502) staff       (20)      173 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_specfunc.h
--rw-r--r--   0 erwin      (502) staff       (20)     2489 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_splinalg.h
--rw-r--r--   0 erwin      (502) staff       (20)     2781 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_spline.h
--rw-r--r--   0 erwin      (502) staff       (20)     4614 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_spline2d.h
--rw-r--r--   0 erwin      (502) staff       (20)     5672 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_spmatrix.h
--rw-r--r--   0 erwin      (502) staff       (20)      519 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics.h
--rw-r--r--   0 erwin      (502) staff       (20)     5845 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_char.h
--rw-r--r--   0 erwin      (502) staff       (20)     7950 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     8194 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     5742 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     5845 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     9082 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     5948 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     6412 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     6309 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     6412 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     6515 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)     5468 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sum.h
--rw-r--r--   0 erwin      (502) staff       (20)     1954 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_sys.h
--rw-r--r--   0 erwin      (502) staff       (20)     1850 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_test.h
--rw-r--r--   0 erwin      (502) staff       (20)     1149 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_types.h
--rw-r--r--   0 erwin      (502) staff       (20)      598 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector.h
--rw-r--r--   0 erwin      (502) staff       (20)     7346 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_char.h
--rw-r--r--   0 erwin      (502) staff       (20)      764 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex.h
--rw-r--r--   0 erwin      (502) staff       (20)     8268 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     9079 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     9967 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     6791 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     7492 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_float.h
--rw-r--r--   0 erwin      (502) staff       (20)     7200 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_int.h
--rw-r--r--   0 erwin      (502) staff       (20)     7346 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_long.h
--rw-r--r--   0 erwin      (502) staff       (20)     8368 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_long_double.h
--rw-r--r--   0 erwin      (502) staff       (20)     7492 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_short.h
--rw-r--r--   0 erwin      (502) staff       (20)     7652 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_uchar.h
--rw-r--r--   0 erwin      (502) staff       (20)     7506 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_uint.h
--rw-r--r--   0 erwin      (502) staff       (20)     7652 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_ulong.h
--rw-r--r--   0 erwin      (502) staff       (20)     7798 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_ushort.h
--rw-r--r--   0 erwin      (502) staff       (20)      458 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_version.h
--rw-r--r--   0 erwin      (502) staff       (20)     3043 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_wavelet.h
--rw-r--r--   0 erwin      (502) staff       (20)     4183 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/gsl/gsl_wavelet2d.h
--rw-r--r--   0 erwin      (502) staff       (20)    13959 2019-07-18 17:24:01.000000 pyimfit-0.8.8/extra_libs/include/nlopt.h
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/extra_libs/lib_linux64/
--rw-r--r--   0 erwin      (502) staff       (20)  5443050 2019-07-18 21:24:44.000000 pyimfit-0.8.8/extra_libs/lib_linux64/libfftw3.a
--rw-r--r--   0 erwin      (502) staff       (20)    51024 2019-07-18 21:24:49.000000 pyimfit-0.8.8/extra_libs/lib_linux64/libfftw3_threads.a
--rw-r--r--   0 erwin      (502) staff       (20) 25317418 2019-07-18 17:34:05.000000 pyimfit-0.8.8/extra_libs/lib_linux64/libgsl.a
--rw-r--r--   0 erwin      (502) staff       (20)  2240026 2019-07-18 17:34:05.000000 pyimfit-0.8.8/extra_libs/lib_linux64/libgslcblas.a
--rw-r--r--   0 erwin      (502) staff       (20)   569074 2019-07-18 17:34:05.000000 pyimfit-0.8.8/extra_libs/lib_linux64/libnlopt.a
--rw-r--r--   0 erwin      (502) staff       (20)      461 2019-07-18 17:45:37.000000 pyimfit-0.8.8/extra_libs/licenses.txt
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/libimfit/
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/libimfit/include/
--rw-r--r--   0 erwin      (502) staff       (20)     1512 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/add_functions.h
--rw-r--r--   0 erwin      (502) staff       (20)     1715 2019-08-09 10:56:22.000000 pyimfit-0.8.8/libimfit/include/bootstrap_errors.h
--rw-r--r--   0 erwin      (502) staff       (20)     4810 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/convolver.h
--rw-r--r--   0 erwin      (502) staff       (20)     3063 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/definitions.h
--rw-r--r--   0 erwin      (502) staff       (20)     3138 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/dispatch_solver.h
--rw-r--r--   0 erwin      (502) staff       (20)     4486 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/function_object.h
--rw-r--r--   0 erwin      (502) staff       (20)     9130 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/model_object.h
--rw-r--r--   0 erwin      (502) staff       (20)     5963 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/mpfit.h
--rw-r--r--   0 erwin      (502) staff       (20)     2143 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/oversampled_region.h
--rw-r--r--   0 erwin      (502) staff       (20)     2816 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/param_struct.h
--rw-r--r--   0 erwin      (502) staff       (20)     2071 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/psf_interpolators.h
--rw-r--r--   0 erwin      (502) staff       (20)     1361 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/psf_oversampling_info.h
--rw-r--r--   0 erwin      (502) staff       (20)     1473 2019-06-12 13:46:50.000000 pyimfit-0.8.8/libimfit/include/solver_results.h
--rw-r--r--   0 erwin      (502) staff       (20)      549 2019-08-09 10:53:18.000000 pyimfit-0.8.8/libimfit/include/statistics.h
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/prebuilt/
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/prebuilt/linux64/
--rw-r--r--   0 erwin      (502) staff       (20)  1125194 2019-08-09 11:38:04.000000 pyimfit-0.8.8/prebuilt/linux64/libimfit.a
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/prebuilt/macos/
--rw-r--r--   0 erwin      (502) staff       (20)   687072 2019-08-09 11:24:56.000000 pyimfit-0.8.8/prebuilt/macos/libimfit.a
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit/
--rw-r--r--   0 erwin      (502) staff       (20)      581 2019-08-25 19:31:49.000000 pyimfit-0.8.8/pyimfit/__init__.py
--rw-r--r--   0 erwin      (502) staff       (20)     8777 2019-08-07 16:29:09.000000 pyimfit-0.8.8/pyimfit/config.py
--rw-r--r--   0 erwin      (502) staff       (20)    33459 2019-08-20 12:00:43.000000 pyimfit-0.8.8/pyimfit/descriptions.py
--rw-r--r--   0 erwin      (502) staff       (20)    31032 2019-08-25 23:20:32.000000 pyimfit-0.8.8/pyimfit/fitting.py
--rw-r--r--   0 erwin      (502) staff       (20)    17275 2019-08-03 16:17:23.000000 pyimfit-0.8.8/pyimfit/imfit_funcs.py
--rw-r--r--   0 erwin      (502) staff       (20)     8672 2019-08-09 10:54:54.000000 pyimfit-0.8.8/pyimfit/imfit_lib.pxd
--rw-r--r--   0 erwin      (502) staff       (20)     3520 2019-08-02 11:08:21.000000 pyimfit-0.8.8/pyimfit/psf.py
--rw-r--r--   0 erwin      (502) staff       (20)  1447305 2019-08-21 13:12:18.000000 pyimfit-0.8.8/pyimfit/pyimfit_lib.cpp
--rw-r--r--   0 erwin      (502) staff       (20)    34080 2019-08-21 13:12:08.000000 pyimfit-0.8.8/pyimfit/pyimfit_lib.pyx
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit/tests/
--rw-r--r--   0 erwin      (502) staff       (20)        0 2019-02-11 14:50:51.000000 pyimfit-0.8.8/pyimfit/tests/__init__.py
--rw-r--r--   0 erwin      (502) staff       (20)     1230 2019-02-22 12:18:35.000000 pyimfit-0.8.8/pyimfit/tests/old_test_model.py
--rw-r--r--   0 erwin      (502) staff       (20)     2018 2019-08-21 13:01:03.000000 pyimfit-0.8.8/pyimfit/tests/test_bootstrap.py
--rw-r--r--   0 erwin      (502) staff       (20)    10383 2019-08-04 21:17:14.000000 pyimfit-0.8.8/pyimfit/tests/test_config.py
--rw-r--r--   0 erwin      (502) staff       (20)    25567 2019-08-20 12:21:43.000000 pyimfit-0.8.8/pyimfit/tests/test_descriptions.py
--rw-r--r--   0 erwin      (502) staff       (20)     9092 2019-08-25 23:19:50.000000 pyimfit-0.8.8/pyimfit/tests/test_fits_and_fitstatistics.py
--rw-r--r--   0 erwin      (502) staff       (20)    10071 2019-08-24 22:56:51.000000 pyimfit-0.8.8/pyimfit/tests/test_fitting.py
--rw-r--r--   0 erwin      (502) staff       (20)     4686 2019-08-21 12:58:54.000000 pyimfit-0.8.8/pyimfit/tests/test_imfit.py
--rw-r--r--   0 erwin      (502) staff       (20)     4163 2019-08-22 10:54:48.000000 pyimfit-0.8.8/pyimfit/tests/test_oversampled_psf.py
--rw-r--r--   0 erwin      (502) staff       (20)    13027 2019-08-20 11:44:36.000000 pyimfit-0.8.8/pyimfit/utils.py
-drwxr-xr-x   0 erwin      (502) staff       (20)        0 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/
--rw-r--r--   0 erwin      (502) staff       (20)     2578 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/PKG-INFO
--rw-r--r--   0 erwin      (502) staff       (20)    11889 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/SOURCES.txt
--rw-r--r--   0 erwin      (502) staff       (20)        1 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/dependency_links.txt
--rw-r--r--   0 erwin      (502) staff       (20)       12 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/requires.txt
--rw-r--r--   0 erwin      (502) staff       (20)        8 2019-08-26 08:51:32.000000 pyimfit-0.8.8/pyimfit.egg-info/top_level.txt
--rw-r--r--   0 erwin      (502) staff       (20)       38 2019-08-26 08:51:32.000000 pyimfit-0.8.8/setup.cfg
--rw-r--r--   0 erwin      (502) staff       (20)    13102 2019-08-13 16:02:30.000000 pyimfit-0.8.8/setup.py
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.150384 pyimfit-0.9.0/
+-rw-r--r--   0 erwin      (502) staff       (20)      357 2019-07-27 20:05:11.000000 pyimfit-0.9.0/MANIFEST.in
+-rw-r--r--   0 erwin      (502) staff       (20)     2552 2020-06-04 12:20:42.149930 pyimfit-0.9.0/PKG-INFO
+-rw-r--r--   0 erwin      (502) staff       (20)     6406 2019-09-27 12:20:11.000000 pyimfit-0.9.0/README.md
+-rw-r--r--   0 erwin      (502) staff       (20)     1506 2019-08-26 09:51:42.000000 pyimfit-0.9.0/README_pyimfit.md
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:41.687884 pyimfit-0.9.0/extra_libs/
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:41.689991 pyimfit-0.9.0/extra_libs/include/
+-rw-r--r--   0 erwin      (502) staff       (20)    17900 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/fftw3.h
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:41.927365 pyimfit-0.9.0/extra_libs/include/gsl/
+-rw-r--r--   0 erwin      (502) staff       (20)    21934 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_blas.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1579 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_blas_types.h
+-rw-r--r--   0 erwin      (502) staff       (20)      580 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2290 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2417 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2557 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2767 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2185 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2325 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2255 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2290 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2535 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2325 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2373 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2338 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2373 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2408 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3473 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_bspline.h
+-rw-r--r--   0 erwin      (502) staff       (20)    33677 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_cblas.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7373 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_cdf.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4509 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_chebyshev.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1579 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_check_range.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2866 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_combination.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3374 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_complex.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6048 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_complex_math.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1056 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6232 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_cgs.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6779 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_cgsm.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6929 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_mks.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7034 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_mksa.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1761 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_num.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1564 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_deriv.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1814 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_dft_complex.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1854 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_dft_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2629 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_dht.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1558 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_diff.h
+-rw-r--r--   0 erwin      (502) staff       (20)    13274 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_eigen.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5965 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_errno.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1402 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4830 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_complex.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5349 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3028 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_halfcomplex.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3234 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_halfcomplex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2232 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_real.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2382 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_real_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4147 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_filter.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2764 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_fit.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_heapsort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4140 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_histogram.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5642 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_histogram2d.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2715 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_ieee_utils.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2463 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_inline.h
+-rw-r--r--   0 erwin      (502) staff       (20)    13855 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_integration.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6961 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_interp.h
+-rw-r--r--   0 erwin      (502) staff       (20)     8795 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_interp2d.h
+-rw-r--r--   0 erwin      (502) staff       (20)    28560 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_linalg.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3805 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_machine.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4345 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_math.h
+-rw-r--r--   0 erwin      (502) staff       (20)      598 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12323 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12844 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)    14076 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)    15378 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)    11363 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12550 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12096 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12323 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)    13912 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12550 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12710 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12483 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12710 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12937 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2420 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_message.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4039 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_min.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2632 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_minmax.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2405 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_mode.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1601 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2662 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_miser.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1884 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_plain.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3234 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_vegas.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6083 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_movstat.h
+-rw-r--r--   0 erwin      (502) staff       (20)    14549 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit.h
+-rw-r--r--   0 erwin      (502) staff       (20)    11357 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit_nlin.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12064 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit_nlinear.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5411 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multilarge.h
+-rw-r--r--   0 erwin      (502) staff       (20)    12990 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multilarge_nlinear.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6795 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multimin.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6152 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multiroots.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2784 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_multiset.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1335 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_nan.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2149 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_ntuple.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7760 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_odeiv.h
+-rw-r--r--   0 erwin      (502) staff       (20)    13781 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_odeiv2.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3346 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permutation.h
+-rw-r--r--   0 erwin      (502) staff       (20)      614 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1430 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1509 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1515 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1563 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1432 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1438 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1422 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1430 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1486 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)      733 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1407 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1414 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1456 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1344 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1400 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1351 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1358 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1365 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1438 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1446 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1454 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1462 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)      733 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1527 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1546 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1600 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1455 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1456 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1528 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1465 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1474 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1483 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5408 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_poly.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2301 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_pow_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1780 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_precision.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2355 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_qrng.h
+-rw-r--r--   0 erwin      (502) staff       (20)    10347 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_randist.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6957 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_rng.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3728 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_roots.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2896 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_rstat.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1106 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3709 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_airy.h
+-rw-r--r--   0 erwin      (502) staff       (20)    14165 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_bessel.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1467 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_clausen.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4402 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_coulomb.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4165 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_coupling.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1402 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_dawson.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2303 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_debye.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4171 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_dilog.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1657 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_elementary.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4159 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_ellint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1364 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_elljac.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2295 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_erf.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3847 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_exp.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4397 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_expint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3413 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_fermi_dirac.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7750 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_gamma.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2154 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_gegenbauer.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4030 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_hermite.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4517 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_hyperg.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2000 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_laguerre.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1813 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_lambert.h
+-rw-r--r--   0 erwin      (502) staff       (20)    11891 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_legendre.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2062 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_log.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4307 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_mathieu.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1390 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_pow_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2683 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_psi.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1577 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_result.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1672 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_sincos_pi.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1723 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_synchrotron.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1978 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_transport.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3957 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_trig.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2894 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_zeta.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3018 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_siman.h
+-rw-r--r--   0 erwin      (502) staff       (20)      435 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1974 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1967 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1995 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1953 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1974 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2121 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1995 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2075 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2054 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2075 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2096 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)      533 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1878 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1817 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1900 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1856 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1878 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2032 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1900 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1916 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1894 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1916 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1938 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1809 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_spblas.h
+-rw-r--r--   0 erwin      (502) staff       (20)      173 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_specfunc.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2489 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_splinalg.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2781 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_spline.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4614 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_spline2d.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5672 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_spmatrix.h
+-rw-r--r--   0 erwin      (502) staff       (20)      519 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5845 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7950 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     8194 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5742 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5845 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     9082 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5948 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6412 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6309 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6412 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6515 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5468 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sum.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1954 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_sys.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1850 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_test.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1149 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_types.h
+-rw-r--r--   0 erwin      (502) staff       (20)      598 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7346 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_char.h
+-rw-r--r--   0 erwin      (502) staff       (20)      764 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex.h
+-rw-r--r--   0 erwin      (502) staff       (20)     8268 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     9079 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     9967 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     6791 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7492 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_float.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7200 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_int.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7346 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_long.h
+-rw-r--r--   0 erwin      (502) staff       (20)     8368 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_long_double.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7492 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_short.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7652 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_uchar.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7506 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_uint.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7652 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_ulong.h
+-rw-r--r--   0 erwin      (502) staff       (20)     7798 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_ushort.h
+-rw-r--r--   0 erwin      (502) staff       (20)      458 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_version.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3043 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_wavelet.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4183 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/gsl/gsl_wavelet2d.h
+-rw-r--r--   0 erwin      (502) staff       (20)    13959 2019-07-18 17:24:01.000000 pyimfit-0.9.0/extra_libs/include/nlopt.h
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.037961 pyimfit-0.9.0/extra_libs/lib_linux64/
+-rw-r--r--   0 erwin      (502) staff       (20)  5443050 2019-07-18 21:24:44.000000 pyimfit-0.9.0/extra_libs/lib_linux64/libfftw3.a
+-rw-r--r--   0 erwin      (502) staff       (20)    51024 2019-07-18 21:24:49.000000 pyimfit-0.9.0/extra_libs/lib_linux64/libfftw3_threads.a
+-rw-r--r--   0 erwin      (502) staff       (20) 25317418 2019-07-18 17:34:05.000000 pyimfit-0.9.0/extra_libs/lib_linux64/libgsl.a
+-rw-r--r--   0 erwin      (502) staff       (20)  2240026 2019-07-18 17:34:05.000000 pyimfit-0.9.0/extra_libs/lib_linux64/libgslcblas.a
+-rw-r--r--   0 erwin      (502) staff       (20)   569074 2019-07-18 17:34:05.000000 pyimfit-0.9.0/extra_libs/lib_linux64/libnlopt.a
+-rw-r--r--   0 erwin      (502) staff       (20)      461 2019-07-18 17:45:37.000000 pyimfit-0.9.0/extra_libs/licenses.txt
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:41.685064 pyimfit-0.9.0/libimfit/
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.051345 pyimfit-0.9.0/libimfit/include/
+-rw-r--r--   0 erwin      (502) staff       (20)     1512 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/add_functions.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1715 2019-08-09 10:56:22.000000 pyimfit-0.9.0/libimfit/include/bootstrap_errors.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4810 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/convolver.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3063 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/definitions.h
+-rw-r--r--   0 erwin      (502) staff       (20)     3138 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/dispatch_solver.h
+-rw-r--r--   0 erwin      (502) staff       (20)     4486 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/function_object.h
+-rw-r--r--   0 erwin      (502) staff       (20)     9130 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/model_object.h
+-rw-r--r--   0 erwin      (502) staff       (20)     5963 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/mpfit.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2143 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/oversampled_region.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2816 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/param_struct.h
+-rw-r--r--   0 erwin      (502) staff       (20)     2071 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/psf_interpolators.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1361 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/psf_oversampling_info.h
+-rw-r--r--   0 erwin      (502) staff       (20)     1473 2019-06-12 13:46:50.000000 pyimfit-0.9.0/libimfit/include/solver_results.h
+-rw-r--r--   0 erwin      (502) staff       (20)      549 2019-08-09 10:53:18.000000 pyimfit-0.9.0/libimfit/include/statistics.h
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:41.685389 pyimfit-0.9.0/prebuilt/
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.051846 pyimfit-0.9.0/prebuilt/linux64/
+-rw-r--r--   0 erwin      (502) staff       (20)  1125194 2019-08-09 11:38:04.000000 pyimfit-0.9.0/prebuilt/linux64/libimfit.a
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.062890 pyimfit-0.9.0/prebuilt/macos/
+-rw-r--r--   0 erwin      (502) staff       (20)   687072 2019-08-09 11:24:56.000000 pyimfit-0.9.0/prebuilt/macos/libimfit.a
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.141037 pyimfit-0.9.0/pyimfit/
+-rw-r--r--   0 erwin      (502) staff       (20)      581 2020-06-04 12:01:27.000000 pyimfit-0.9.0/pyimfit/__init__.py
+-rw-r--r--   0 erwin      (502) staff       (20)     8777 2019-08-07 16:29:09.000000 pyimfit-0.9.0/pyimfit/config.py
+-rw-r--r--   0 erwin      (502) staff       (20)    33776 2020-06-04 11:33:48.000000 pyimfit-0.9.0/pyimfit/descriptions.py
+-rw-r--r--   0 erwin      (502) staff       (20)    32251 2020-06-04 11:50:25.000000 pyimfit-0.9.0/pyimfit/fitting.py
+-rw-r--r--   0 erwin      (502) staff       (20)    17275 2019-08-03 16:17:23.000000 pyimfit-0.9.0/pyimfit/imfit_funcs.py
+-rw-r--r--   0 erwin      (502) staff       (20)     8569 2019-10-07 12:05:03.000000 pyimfit-0.9.0/pyimfit/imfit_lib.pxd
+-rw-r--r--   0 erwin      (502) staff       (20)     3520 2019-08-02 11:08:21.000000 pyimfit-0.9.0/pyimfit/psf.py
+-rw-r--r--   0 erwin      (502) staff       (20)  1447305 2020-06-04 11:21:11.000000 pyimfit-0.9.0/pyimfit/pyimfit_lib.cpp
+-rw-r--r--   0 erwin      (502) staff       (20)    34080 2019-08-21 13:12:08.000000 pyimfit-0.9.0/pyimfit/pyimfit_lib.pyx
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.149049 pyimfit-0.9.0/pyimfit/tests/
+-rw-r--r--   0 erwin      (502) staff       (20)        0 2019-02-11 14:50:51.000000 pyimfit-0.9.0/pyimfit/tests/__init__.py
+-rw-r--r--   0 erwin      (502) staff       (20)     1230 2019-02-22 12:18:35.000000 pyimfit-0.9.0/pyimfit/tests/old_test_model.py
+-rw-r--r--   0 erwin      (502) staff       (20)     2018 2019-08-21 13:01:03.000000 pyimfit-0.9.0/pyimfit/tests/test_bootstrap.py
+-rw-r--r--   0 erwin      (502) staff       (20)    10383 2019-08-04 21:17:14.000000 pyimfit-0.9.0/pyimfit/tests/test_config.py
+-rw-r--r--   0 erwin      (502) staff       (20)    25768 2020-06-04 11:31:57.000000 pyimfit-0.9.0/pyimfit/tests/test_descriptions.py
+-rw-r--r--   0 erwin      (502) staff       (20)     9092 2019-08-25 23:19:50.000000 pyimfit-0.9.0/pyimfit/tests/test_fits_and_fitstatistics.py
+-rw-r--r--   0 erwin      (502) staff       (20)    11054 2020-06-04 11:49:00.000000 pyimfit-0.9.0/pyimfit/tests/test_fitting.py
+-rw-r--r--   0 erwin      (502) staff       (20)     4686 2019-08-21 12:58:54.000000 pyimfit-0.9.0/pyimfit/tests/test_imfit.py
+-rw-r--r--   0 erwin      (502) staff       (20)     4163 2019-08-22 10:54:48.000000 pyimfit-0.9.0/pyimfit/tests/test_oversampled_psf.py
+-rw-r--r--   0 erwin      (502) staff       (20)    13027 2019-08-20 11:44:36.000000 pyimfit-0.9.0/pyimfit/utils.py
+drwxr-xr-x   0 erwin      (502) staff       (20)        0 2020-06-04 12:20:42.143214 pyimfit-0.9.0/pyimfit.egg-info/
+-rw-r--r--   0 erwin      (502) staff       (20)     2552 2020-06-04 12:20:41.000000 pyimfit-0.9.0/pyimfit.egg-info/PKG-INFO
+-rw-r--r--   0 erwin      (502) staff       (20)    11889 2020-06-04 12:20:41.000000 pyimfit-0.9.0/pyimfit.egg-info/SOURCES.txt
+-rw-r--r--   0 erwin      (502) staff       (20)        1 2020-06-04 12:20:41.000000 pyimfit-0.9.0/pyimfit.egg-info/dependency_links.txt
+-rw-r--r--   0 erwin      (502) staff       (20)       12 2020-06-04 12:20:41.000000 pyimfit-0.9.0/pyimfit.egg-info/requires.txt
+-rw-r--r--   0 erwin      (502) staff       (20)        8 2020-06-04 12:20:41.000000 pyimfit-0.9.0/pyimfit.egg-info/top_level.txt
+-rw-r--r--   0 erwin      (502) staff       (20)       38 2020-06-04 12:20:42.150566 pyimfit-0.9.0/setup.cfg
+-rw-r--r--   0 erwin      (502) staff       (20)    13102 2019-08-13 16:02:30.000000 pyimfit-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyimfit-0.8.8/PKG-INFO` & `pyimfit-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimfit
-Version: 0.8.8
+Version: 0.9.0
 Summary: Python wrapper for astronomical image-fitting program Imfit
 Home-page: https://github.com/perwin/pyimfit
 Author: Peter Erwin
 Author-email: erwin@sigmaxi.net
 License: UNKNOWN
 Project-URL: Documentation, https://pyimfit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/perwin/pyimfit
@@ -33,21 +33,21 @@
             model_desc = pyimfit.ModelDescription.load(configFile)
         
             # create an Imfit object, using the previously loaded model configuration
             imfit_fitter = pyimfit.Imfit(model_desc)
         
             # load the image data and image characteristics and do a standard fit
             # (using default chi^2 statistics and Levenberg-Marquardt solver)
-            imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
+            result = imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
             
             # check the fit and print the resulting best-fit parameter values
-            if imfit_fitter.fitConverged is True:
+            if result.fitConverged is True:
                 print("Fit converged: chi^2 = {0}, reduced chi^2 = {1}".format(imfit_fitter.fitStatistic,
-                    imfit_fitter.reducedFitStatistic))
-                bestfit_params = imfit_fitter.getRawParameters()
+                    result.reducedFitStat))
+                bestfit_params = result.params
                 print("Best-fit parameter values:", bestfit_params)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyimfit-0.8.8/README.md` & `pyimfit-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -142,12 +142,14 @@
 
 
 ## Credits
 
 PyImfit originated as [python-imfit](https://github.com/streeto/python-imfit), written by André Luiz de Amorim; 
 the current, updated version is by Peter Erwin.
 
+(See [the Imfit manual](http://www.mpe.mpg.de/~erwin/resources/imfit/imfit_howto.pdf) for additional credits.)
+
 
 ## License
 
 PyImfit is licensed under version 3 of the GNU Public License.
```

### Comparing `pyimfit-0.8.8/README_pyimfit.md` & `pyimfit-0.9.0/README_pyimfit.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     model_desc = pyimfit.ModelDescription.load(configFile)
 
     # create an Imfit object, using the previously loaded model configuration
     imfit_fitter = pyimfit.Imfit(model_desc)
 
     # load the image data and image characteristics and do a standard fit
     # (using default chi^2 statistics and Levenberg-Marquardt solver)
-    imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
+    result = imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
     
     # check the fit and print the resulting best-fit parameter values
-    if imfit_fitter.fitConverged is True:
+    if result.fitConverged is True:
         print("Fit converged: chi^2 = {0}, reduced chi^2 = {1}".format(imfit_fitter.fitStatistic,
-            imfit_fitter.reducedFitStatistic))
-        bestfit_params = imfit_fitter.getRawParameters()
+            result.reducedFitStat))
+        bestfit_params = result.params
         print("Best-fit parameter values:", bestfit_params)
```

### Comparing `pyimfit-0.8.8/extra_libs/include/fftw3.h` & `pyimfit-0.9.0/extra_libs/include/fftw3.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_blas.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_blas.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_blas_types.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_blas_types.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_block_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_block_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_bspline.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_bspline.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_cblas.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_cblas.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_cdf.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_cdf.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_chebyshev.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_chebyshev.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_check_range.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_check_range.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_combination.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_combination.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_complex.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_complex.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_complex_math.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_complex_math.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_cgs.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_cgs.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_cgsm.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_cgsm.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_mks.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_mks.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_mksa.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_mksa.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_const_num.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_const_num.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_deriv.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_deriv.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_dft_complex.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_dft_complex.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_dft_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_dft_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_dht.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_dht.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_diff.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_diff.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_eigen.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_eigen.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_errno.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_errno.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_complex.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_complex.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_halfcomplex.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_halfcomplex.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_halfcomplex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_halfcomplex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_real.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_real.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fft_real_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fft_real_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_filter.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_filter.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_fit.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_fit.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_heapsort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_heapsort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_histogram.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_histogram.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_histogram2d.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_histogram2d.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_ieee_utils.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_ieee_utils.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_inline.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_inline.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_integration.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_integration.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_interp.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_interp.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_interp2d.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_interp2d.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_linalg.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_linalg.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_machine.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_machine.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_math.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_math.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_matrix_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_matrix_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_message.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_message.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_min.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_min.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_minmax.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_minmax.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_mode.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_mode.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_miser.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_miser.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_plain.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_plain.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_monte_vegas.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_monte_vegas.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_movstat.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_movstat.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit_nlin.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit_nlin.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multifit_nlinear.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multifit_nlinear.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multilarge.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multilarge.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multilarge_nlinear.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multilarge_nlinear.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multimin.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multimin.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multiroots.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multiroots.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_multiset.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_multiset.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_nan.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_nan.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_ntuple.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_ntuple.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_odeiv.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_odeiv.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_odeiv2.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_odeiv2.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permutation.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permutation.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_matrix_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_matrix_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_permute_vector_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_permute_vector_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_poly.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_poly.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_pow_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_pow_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_precision.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_precision.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_qrng.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_qrng.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_randist.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_randist.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_rng.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_rng.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_roots.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_roots.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_rstat.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_rstat.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_airy.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_airy.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_bessel.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_bessel.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_clausen.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_clausen.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_coulomb.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_coulomb.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_coupling.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_coupling.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_dawson.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_dawson.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_debye.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_debye.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_dilog.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_dilog.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_elementary.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_elementary.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_ellint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_ellint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_elljac.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_elljac.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_erf.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_erf.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_exp.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_exp.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_expint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_expint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_fermi_dirac.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_fermi_dirac.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_gamma.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_gamma.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_gegenbauer.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_gegenbauer.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_hermite.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_hermite.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_hyperg.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_hyperg.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_laguerre.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_laguerre.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_lambert.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_lambert.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_legendre.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_legendre.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_log.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_log.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_mathieu.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_mathieu.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_pow_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_pow_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_psi.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_psi.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_result.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_result.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_sincos_pi.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_sincos_pi.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_synchrotron.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_synchrotron.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_transport.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_transport.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_trig.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_trig.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sf_zeta.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sf_zeta.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_siman.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_siman.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sort_vector_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sort_vector_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_spblas.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_spblas.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_splinalg.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_splinalg.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_spline.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_spline.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_spline2d.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_spline2d.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_spmatrix.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_spmatrix.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_statistics_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_statistics_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sum.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sum.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_sys.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_sys.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_test.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_test.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_types.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_types.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_char.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_char.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_complex_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_complex_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_float.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_float.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_int.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_int.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_long.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_long.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_long_double.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_long_double.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_short.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_short.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_uchar.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_uchar.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_uint.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_uint.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_ulong.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_ulong.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_vector_ushort.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_vector_ushort.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_wavelet.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_wavelet.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/gsl/gsl_wavelet2d.h` & `pyimfit-0.9.0/extra_libs/include/gsl/gsl_wavelet2d.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/include/nlopt.h` & `pyimfit-0.9.0/extra_libs/include/nlopt.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/lib_linux64/libfftw3.a` & `pyimfit-0.9.0/extra_libs/lib_linux64/libfftw3.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/lib_linux64/libfftw3_threads.a` & `pyimfit-0.9.0/extra_libs/lib_linux64/libfftw3_threads.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/lib_linux64/libgsl.a` & `pyimfit-0.9.0/extra_libs/lib_linux64/libgsl.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/lib_linux64/libgslcblas.a` & `pyimfit-0.9.0/extra_libs/lib_linux64/libgslcblas.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/extra_libs/lib_linux64/libnlopt.a` & `pyimfit-0.9.0/extra_libs/lib_linux64/libnlopt.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/add_functions.h` & `pyimfit-0.9.0/libimfit/include/add_functions.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/bootstrap_errors.h` & `pyimfit-0.9.0/libimfit/include/bootstrap_errors.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/convolver.h` & `pyimfit-0.9.0/libimfit/include/convolver.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/definitions.h` & `pyimfit-0.9.0/libimfit/include/definitions.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/dispatch_solver.h` & `pyimfit-0.9.0/libimfit/include/dispatch_solver.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/function_object.h` & `pyimfit-0.9.0/libimfit/include/function_object.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/model_object.h` & `pyimfit-0.9.0/libimfit/include/model_object.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/mpfit.h` & `pyimfit-0.9.0/libimfit/include/mpfit.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/oversampled_region.h` & `pyimfit-0.9.0/libimfit/include/oversampled_region.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/param_struct.h` & `pyimfit-0.9.0/libimfit/include/param_struct.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/psf_interpolators.h` & `pyimfit-0.9.0/libimfit/include/psf_interpolators.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/psf_oversampling_info.h` & `pyimfit-0.9.0/libimfit/include/psf_oversampling_info.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/solver_results.h` & `pyimfit-0.9.0/libimfit/include/solver_results.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/libimfit/include/statistics.h` & `pyimfit-0.9.0/libimfit/include/statistics.h`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/prebuilt/linux64/libimfit.a` & `pyimfit-0.9.0/prebuilt/linux64/libimfit.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/prebuilt/macos/libimfit.a` & `pyimfit-0.9.0/prebuilt/macos/libimfit.a`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/__init__.py` & `pyimfit-0.9.0/pyimfit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .psf import *
 from . import utils
 
 # useful package-level variables
 imageFunctionList = get_function_list()
 imageFunctionDict = get_function_dict()
 
-__version__ = "0.8.8"
+__version__ = "0.9.0"
```

### Comparing `pyimfit-0.8.8/pyimfit/config.py` & `pyimfit-0.9.0/pyimfit/config.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/descriptions.py` & `pyimfit-0.9.0/pyimfit/descriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,37 +391,39 @@
         f.nParameters = self.nParameters
         return f
 
 
 
 class FunctionSetDescription(object):
     """
-    Holds information describing an image-function block or set: one or more
+    Holds information describing an image-function block/set: one or more
     Imfit image functions sharing a common (X0,Y0) position on the image.
 
     This contains the X0 and Y0 coordinates, a list of FunctionDescription
     objects, and name or label for the function set (e.g., "fs0", "star 1",
     "galaxy 5", "offset nucleus", etc.)
 
     Attributes
     ----------
 
         name : str
-            name for the function block
+            name for the function set
 
         _name : str
-            name for the function block
+            name for the function set
         x0 : ParameterDescription
             x-coordinate of the function block/set's center
         y0 : ParameterDescription
             y-coordinate of the function block/set's center
         _functions : list of `FunctionDescription`
             the FunctionDescription objects, one for each image function
         nFunctions : int
-            number of functions in the function block
+            number of functions in the function set
+        nParameters : int
+            total number of parameters for this function set, including X0 and Y0
 
     Methods
     -------
         addFunction(f)
             Add a FunctionDescription instance
 
         functionList()
@@ -453,14 +455,15 @@
         else:
             if not isinstance(y0param, ParameterDescription):
                 msg = "y0param should be instance of ParameterDescription"
                 raise ValueError(msg)
             self.y0 = y0param
         self._functions = []  #type: List[FunctionDescription]
         self.nFunctions = 0
+        self.nParameters = 2   # X0,Y0
         if functionList is not None:
             for f in functionList:
                 self.addFunction(f)
             self.nFunctions = len(functionList)
 
 
     @property
@@ -486,14 +489,15 @@
             raise KeyError('Function with label \"%s\" already exists.' % f.label)
         self._functions.append(f)
         # add function labels as attributes, so we can do things like
         # function_set_instance.<func_name>
         if f._label is not None:
             setattr(self, f._label, f)
         self.nFunctions += 1
+        self.nParameters += f.nParameters
 
 
     def _contains(self, label: str):
         for f in self._functions:
             if f.label == label:
                 return True
         return False
@@ -552,15 +556,15 @@
 
         errors : sequence float, optional
             errors on parameter values (e.g., from Levenberg-Marquardt minimization)
 
         Returns
         -------
         outputStrings : list of string
-            list of newline-terminated strings describing the function block.
+            list of newline-terminated strings describing the function set.
             If errors is supplied, then parameter strings will contain "# +/- <error>" at end
         """
         # x0,y0
         if errors is not None:
             x0Line = self.x0.getStringDescription(error=errors[0])
             y0Line = self.y0.getStringDescription(error=errors[1])
         else:
@@ -622,14 +626,16 @@
         options : dict of {str: float}
             dict mapping image-description parameters (e.g., "GAIN") to
             their corresponding values [this is the internal name for the
             property optionsDict]
         _functionSets : list of `FunctionSetDescription`
             the individual image-function blocks/sets making up the model
         nFunctionSets : int
+        nParameters : int
+            total number of model parameters
 
     Class methods
     -------------
         load(fname)
             Returns a new instance of this class based on a standard Imfit
             configuration file (`fname`).
 
@@ -638,15 +644,15 @@
         addFunctionSet(fs)
             Add a function block/set to the model description
 
         addOptions(optionDict)
             Add image-description options via a dict
 
         functionSetIndices()
-            Returns a list of ``int`` specifying the function-block start
+            Returns a list of ``int`` specifying the function-set start
             indices
 
         functionList()
             Retuns a list of FunctionDescription instances for all the
             image functions in the model
 
         functionNameList()
@@ -662,14 +668,15 @@
     def __init__( self, functionSetsList: Optional[List[FunctionSetDescription]]=None,
                   options: Optional[Dict[str,float]]=None ):
         self.options = OrderedDict()  #type: Dict[str,float]
         if options is not None:
             self.options.update(options)
         self._functionSets = []  #type: List[FunctionSetDescription]
         self.nFunctionSets = 0
+        self.nParameters = 0
         if functionSetsList is not None:
             for fs in functionSetsList:
                 # note that addFunctionSet will increment nFunctionSets, so we don't need to
                 # do that here
                 self.addFunctionSet(fs)
 
 
@@ -745,14 +752,15 @@
         if not isinstance(fs, FunctionSetDescription):
             raise ValueError('fs is not a FunctionSet object.')
         if self._contains(fs.name):
             raise KeyError('FunctionSet named %s already exists.' % fs.name)
         self._functionSets.append(fs)
         setattr(self, fs.name, fs)
         self.nFunctionSets += 1
+        self.nParameters += fs.nParameters
 
 
     def updateOptions( self, optionsDict: Dict[str,float] ):
         """
         Updates the internal image-descriptions dict, replacing current values for keys
         already in the dict and added key-value pairs for keys not already present.
 
@@ -903,15 +911,15 @@
         outputLines = []
         # image-description parameters
         if saveOptions and len(self.options) > 0:
             for key,value in self.options.items():
                 newLine = "{0}\t\t{1}\n".format(key, value)
                 outputLines.append(newLine)
 
-        # function blocks
+        # function sets
         fblockIndices = self.functionSetIndices()
         for i in range(self.nFunctionSets):
             outputLines.extend("\n")
             fblock = self._functionSets[i]
             fblockStartIndex = fblockIndices[i]
             if errors is not None:
                 newLines = fblock.getStringDescription(noLimits=noLimits, errors=errors[fblockStartIndex:])
```

### Comparing `pyimfit-0.8.8/pyimfit/fitting.py` & `pyimfit-0.9.0/pyimfit/fitting.py`

 * *Files 12% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     regionString = "{0:d}:{1:d},{2:d}:{3:d}".format(regionSpec[0],regionSpec[1],regionSpec[2],regionSpec[3])
     return PsfOversampling(psfImage, oversampleScale, regionString, 0, 0, psfNormalization)
 
 
 
 class Imfit(object):
     """
-    A class for fitting models to images using Imfit.
+    The main class for fitting models to images using Imfit.
     Can also be used to create images based on models.
 
     Due to some library limitations, this object can only fit the model
     specified in the constructor. If you want to fit several models,
     you need to create one instance of :class:`Imfit` for each model.
     On the other hand, one instance can be used to fit the same model
     to any number of images, or to fit and then create the model image.
@@ -228,14 +228,15 @@
             model and component magnitudes) via getModelMagnitudes
         """
         if not isinstance(model_descr, ModelDescription ):
             raise ValueError('model_descr must be a ModelDescription object.')
         # copy the input ModelDescription (we don't want any links to the input object,
         # in case the latter gets updated later somewhere else)
         self._modelDescr = copy.deepcopy(model_descr)
+        self.nParameters = model_descr.nParameters
         if psf is not None:
             self._psf = FixImage(psf)
         else:
             self._psf = None
         self._normalizePSF = psfNormalization
         self._mask = None
         self._modelObjectWrapper = None
@@ -631,15 +632,18 @@
         ----------
         newParameters : ndarray of float
 
         Returns
         -------
         fitStatistic : float
         """
-        # FIXME: Check that length of newParameters is correct
+        if len(newParameters) != self.nParameters:
+            msg = "Number of input parameters (%d) " % len(newParameters)
+            msg += "does not equal number of model parameters (%d)!" % self.nParameters
+            raise ValueError(msg)
         if not isinstance(newParameters, np.ndarray):
             newParams = np.array(newParameters).astype(np.float64)
         else:
             newParams = newParameters.astype(np.float64)
         return self._modelObjectWrapper.computeFitStatistic(newParams)
 
 
@@ -800,34 +804,37 @@
         Parameters
         ----------
         newParameters : 1-D numpy array of float, optional
             vector of parameter values to use in computing model
             (default is to use current parameter values, e.g., from fit)
 
         shape : tuple, optional
-            Shape of the image in (Y, X) format.
+            Shape of the image in (Y, X) = (nRows, nColumns) format.
 
         includeMask : bool, optional
             Specifies whether output should be numpy masked array, if there
             is a mask image associated with the data image.
 
         Returns
         -------
         image : 2-D numpy array
-            Image computed from the current model. If a mask is associated
-            with the original data image, then the returned image is a
-            numpy masked array
+            Image computed from the current model. If a mask is associated with the
+            original data image, then the returned image is a numpy masked array
         """
         if self._modelObjectWrapper is None:
             self._setupModel()
         if shape is not None:
             if self._modelObjectWrapper.imageSizeSet:
                 msg = "Model image size has already been set!"
                 raise ValueError(msg)
             self._modelObjectWrapper.setupModelImage(shape)
+        if (newParameters is not None) and (len(newParameters) != self.nParameters):
+            msg = "Number of input parameters (%d) " % len(newParameters)
+            msg += "does not equal number of model parameters (%d)!" % self.nParameters
+            raise ValueError(msg)
 
         image = self._modelObjectWrapper.getModelImage(newParameters=newParameters)
         if self._mask is not None and includeMask:
             return np.ma.array(image, mask=self._mask)
         else:
             return image
 
@@ -837,56 +844,65 @@
         Computes and returns total and individual-function fluxes for the current model
         and current parameter values.
 
         Parameters
         ----------
         newParameters : 1-D numpy array of float, optional
             vector of parameter values to use in computing model
-            (default is to use current parameter values, e.g., from fit)
+            (default is to use current parameter values, e.g., from most rencent fit, instead)
 
         Returns
         -------
         (totalFlux, individualFluxes) : tuple of (float, ndarray of float)
             totalFlux = total flux (or magnitude) of model
             individualFluxes = numpy ndarray of fluxes/magnitudes for each image-function in the
             model
         """
+        if (newParameters is not None) and (len(newParameters) != self.nParameters):
+            msg = "Number of input parameters (%d) " % len(newParameters)
+            msg += "does not equal number of model parameters (%d)!" % self.nParameters
+            raise ValueError(msg)
         totalFlux, functionFluxes = self._modelObjectWrapper.getModelFluxes(newParameters=newParameters)
         return(totalFlux, functionFluxes)
 
 
     def getModelMagnitudes( self, newParameters=None, zeroPoint=None ):
         """
         Computes and returns total and individual-function magnitudes for the current model
         and current parameter values.
 
         Parameters
         ----------
         newParameters : 1-D numpy array of float, optional
             vector of parameter values to use in computing model
-            (default is to use current parameter values, e.g., from fit)
+            (default is to use current parameter values, e.g., from most rencent fit, instead)
 
         zeroPoint : float, optional
             If present, returned values are magnitudes, computed as
                 zeroPoint - 2.5*log10(flux)
             (default is to use value of object's zeroPoint property)
 
         Returns
         -------
         (totalMag, individualMags) : tuple of (float, ndarray of float)
             totalFlux = total flux (or magnitude) of model
             individualFluxes = numpy ndarray of fluxes/magnitudes for each image-function in the
             model
 
         """
+        if (newParameters is not None) and (len(newParameters) != self.nParameters):
+            msg = "Number of input parameters (%d) " % len(newParameters)
+            msg += "does not equal number of model parameters (%d)!" % self.nParameters
+            raise ValueError(msg)
         totalFlux, functionFluxes = self._modelObjectWrapper.getModelFluxes(newParameters=newParameters)
         if zeroPoint is not None:
             ZP = zeroPoint
         else:
             ZP = self.zeroPoint
+        #FIXME: Handle case of zeroPoint = None! (i.e., user forget to set it...)
         return (ZP - 2.5*np.log10(totalFlux), ZP - 2.5*np.log10(functionFluxes))
 
 
     def __del__(self):
         if self._modelObjectWrapper is not None:
             # FIXME: Find a better way to free Cython resources.
             self._modelObjectWrapper.close()
```

### Comparing `pyimfit-0.8.8/pyimfit/imfit_funcs.py` & `pyimfit-0.9.0/pyimfit/imfit_funcs.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/imfit_lib.pxd` & `pyimfit-0.9.0/pyimfit/imfit_lib.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     const int DIFF_EVOLN_SOLVER    =     2
     const int NMSIMPLEX_SOLVER     =     3
     const int ALT_SOLVER           =     4
     const int GENERIC_NLOPT_SOLVER =     5
 
 
 cdef extern from "statistics.h":
-    double Mean( double *vector, int nVals )
-    double StandardDeviation( double *vector, int nVals )
     double AIC_corrected( double logLikelihood, int nParams, long nData, int chiSquareUsed )
     double BIC( double logLikelihood, int nParams, long nData, int chiSquareUsed )
 
 
 cdef extern from "param_struct.h":
     ctypedef struct mp_par:
         bint fixed          # 1 = fixed; 0 = free
```

### Comparing `pyimfit-0.8.8/pyimfit/psf.py` & `pyimfit-0.9.0/pyimfit/psf.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/pyimfit_lib.cpp` & `pyimfit-0.9.0/pyimfit/pyimfit_lib.cpp`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/pyimfit_lib.pyx` & `pyimfit-0.9.0/pyimfit/pyimfit_lib.pyx`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/old_test_model.py` & `pyimfit-0.9.0/pyimfit/tests/old_test_model.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_bootstrap.py` & `pyimfit-0.9.0/pyimfit/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_config.py` & `pyimfit-0.9.0/pyimfit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_descriptions.py` & `pyimfit-0.9.0/pyimfit/tests/test_descriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,26 +243,28 @@
         self.p1 = ParameterDescription("PA", 0.0, fixed=True)
         self.p2 = ParameterDescription("ell", 0.5, [0.1,0.8])
         self.p3 = ParameterDescription("I_0", 100.0, [10.0, 1e3])
         self.p4 = ParameterDescription("sigma", 10.0, [5.0,20.0])
         self.paramDescList = [self.p1, self.p2, self.p3, self.p4]
         self.fdesc1 = FunctionDescription('Gaussian', "blob", self.paramDescList)
         self.functionList = [self.fdesc1]
+        self.N_PARAMS_CORRECT = 4 + 2
 
         self.x0_p = ParameterDescription("X0", 100.0, fixed=True)
         self.y0_p = ParameterDescription("Y0", 200.0, [180.0, 220.0])
 
 
     def test_FunctionSetDescription_simple( self ):
         fsetdesc1 = FunctionSetDescription('fs0', self.x0_p, self.y0_p, self.functionList)
         assert fsetdesc1.name == "fs0"
         assert fsetdesc1._contains("blob") is True
         assert fsetdesc1.blob == self.fdesc1
         assert fsetdesc1.x0 == self.x0_p
         assert fsetdesc1.y0 == self.y0_p
+        assert fsetdesc1.nParameters == self.N_PARAMS_CORRECT
 
     def test_FunctionSetDescription_parameterList( self ):
         fsetdesc1 = FunctionSetDescription('fs0', self.x0_p, self.y0_p, self.functionList)
         plist_correct = [self.x0_p, self.y0_p, self.p1, self.p2, self.p3, self.p4]
         assert fsetdesc1.parameterList() == plist_correct
 
     def test_FunctionSetDescription_parameterList_badInput( self ):
@@ -340,20 +342,22 @@
         self.p4 = ParameterDescription("sigma", 10.0, [5.0,20.0])
         self.paramDescList = [self.p1, self.p2, self.p3, self.p4]
         self.fullParamDescList = [self.x0_p, self.y0_p, self.p1, self.p2, self.p3, self.p4]
         self.fdesc1 = FunctionDescription('Gaussian', "blob", self.paramDescList)
         self.functionList = [self.fdesc1]
         self.fsetdesc1 = FunctionSetDescription('fs0', self.x0_p, self.y0_p, self.functionList)
         self.fsetList = [self.fsetdesc1]
+        self.N_PARAMS_CORRECT = 4 + 2
 
     def test_ModelDescription_simple( self ):
         modeldesc1 = ModelDescription(self.fsetList)
         assert modeldesc1.functionSetIndices() == [0]
         assert modeldesc1.functionNameList() == ['Gaussian']
         assert modeldesc1.parameterList() == self.fullParamDescList
+        assert modeldesc1.nParameters == self.N_PARAMS_CORRECT
 
     def test_ModelDescription_getParamLimits( self ):
         modeldesc1 = ModelDescription(self.fsetList)
         pLimits = modeldesc1.getParameterLimits()
         assert pLimits == [None,(180.0,220.0), None, (0.1,0.8), (10.0,1e3), (5.0,20.0)]
 
     def testModelDescription_get_and_set_options( self ):
```

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_fits_and_fitstatistics.py` & `pyimfit-0.9.0/pyimfit/tests/test_fits_and_fitstatistics.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_fitting.py` & `pyimfit-0.9.0/pyimfit/tests/test_fitting.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,14 +157,34 @@
         # get magnitudes -- now, use parameter zero point
         (totalMag, magsArray) = imfit_fitter.getModelMagnitudes(userParams, zeroPoint=20)
         totalMag_correct = 20 - 2.5*math.log10(94247.7796076937)
         magsArray_correct = np.array([totalMag_correct])
         assert totalMag == totalMag_correct
         assert magsArray == magsArray_correct
 
+    def test_Imfit_catch_bad_parameters(self):
+        """Check that we get ValueError exceptions when passing new-parameter-vector of wrong size
+        """
+        # Exponential model
+        imfit_fitter = Imfit(self.modelDesc)
+        imfit_fitter.loadData(image_ic3478, gain=4.725, read_noise=4.3, original_sky=130.14)
+
+        badParams = np.array([129.0,129.0, 20.0])   # not enough parameter values!
+        # computeFitStatistic
+        with pytest.raises(ValueError):
+            fitstat = imfit_fitter.computeFitStatistic(badParams)
+        # getModelImage
+        with pytest.raises(ValueError):
+            image = imfit_fitter.getModelImage(newParameters=badParams)
+        # getModelFluxes
+        with pytest.raises(ValueError):
+            (totalFlux, fluxArray) = imfit_fitter.getModelFluxes(badParams)
+        # getModelMagnitudes
+        with pytest.raises(ValueError):
+            (totalMag, magsArray) = imfit_fitter.getModelMagnitudes(badParams, zeroPoint=20)
 
 
 # result.fitConverged = self.fitConverged
 # result.nIter = self.nIter
 # result.fitStat = self.fitStatistic
 # result.fitStatReduced = self.reducedFitStatistic
 # result.aic = self.AIC
```

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_imfit.py` & `pyimfit-0.9.0/pyimfit/tests/test_imfit.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/tests/test_oversampled_psf.py` & `pyimfit-0.9.0/pyimfit/tests/test_oversampled_psf.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit/utils.py` & `pyimfit-0.9.0/pyimfit/utils.py`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/pyimfit.egg-info/PKG-INFO` & `pyimfit-0.9.0/pyimfit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimfit
-Version: 0.8.8
+Version: 0.9.0
 Summary: Python wrapper for astronomical image-fitting program Imfit
 Home-page: https://github.com/perwin/pyimfit
 Author: Peter Erwin
 Author-email: erwin@sigmaxi.net
 License: UNKNOWN
 Project-URL: Documentation, https://pyimfit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/perwin/pyimfit
@@ -33,21 +33,21 @@
             model_desc = pyimfit.ModelDescription.load(configFile)
         
             # create an Imfit object, using the previously loaded model configuration
             imfit_fitter = pyimfit.Imfit(model_desc)
         
             # load the image data and image characteristics and do a standard fit
             # (using default chi^2 statistics and Levenberg-Marquardt solver)
-            imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
+            result = imfit_fitter.fit(image_data, gain=4.725, read_noise=4.3, original_sky=130.14)
             
             # check the fit and print the resulting best-fit parameter values
-            if imfit_fitter.fitConverged is True:
+            if result.fitConverged is True:
                 print("Fit converged: chi^2 = {0}, reduced chi^2 = {1}".format(imfit_fitter.fitStatistic,
-                    imfit_fitter.reducedFitStatistic))
-                bestfit_params = imfit_fitter.getRawParameters()
+                    result.reducedFitStat))
+                bestfit_params = result.params
                 print("Best-fit parameter values:", bestfit_params)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyimfit-0.8.8/pyimfit.egg-info/SOURCES.txt` & `pyimfit-0.9.0/pyimfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyimfit-0.8.8/setup.py` & `pyimfit-0.9.0/setup.py`

 * *Files identical despite different names*

