# Comparing `tmp/riyazi-0.16.tar.gz` & `tmp/riyazi-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riyazi-0.16.tar", last modified: Sun Apr  9 06:03:57 2023, max compression
+gzip compressed data, was "riyazi-0.17.tar", last modified: Tue Apr 18 06:45:11 2023, max compression
```

## Comparing `riyazi-0.16.tar` & `riyazi-0.17.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.948367 riyazi-0.16/
--rw-rw-rw-   0        0        0     1526 2023-02-02 12:38:49.000000 riyazi-0.16/LICENSE
--rw-rw-rw-   0        0        0      143 2023-04-09 06:03:57.945217 riyazi-0.16/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-04-03 11:13:54.000000 riyazi-0.16/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.585465 riyazi-0.16/riyazi/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.625294 riyazi-0.16/riyazi/Module/
--rw-rw-rw-   0        0        0      440 2022-11-13 07:09:57.000000 riyazi-0.16/riyazi/Module/__fornumerics.py
--rw-rw-rw-   0        0        0       27 2022-11-13 06:32:33.000000 riyazi-0.16/riyazi/Module/__init__.py
--rw-rw-rw-   0        0        0      980 2022-09-01 09:12:38.000000 riyazi-0.16/riyazi/Module/main.py
--rw-rw-rw-   0        0        0      219 2022-09-09 15:48:35.000000 riyazi-0.16/riyazi/Module/module.py
--rw-rw-rw-   0        0        0     2236 2022-09-28 02:56:20.000000 riyazi-0.16/riyazi/Module/mymodule.py
--rw-rw-rw-   0        0        0     1498 2022-09-27 13:10:35.000000 riyazi-0.16/riyazi/Module/numeric.py
--rw-rw-rw-   0        0        0      569 2023-03-31 04:49:26.000000 riyazi-0.16/riyazi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.634297 riyazi-0.16/riyazi/algebra/
--rw-rw-rw-   0        0        0       79 2023-04-01 05:03:00.000000 riyazi-0.16/riyazi/algebra/__init__.py
--rw-rw-rw-   0        0        0      535 2022-09-03 06:06:18.000000 riyazi-0.16/riyazi/algebra/_factor.py
--rw-rw-rw-   0        0        0      248 2023-03-30 05:44:16.000000 riyazi-0.16/riyazi/algebra/_law_exp.py
--rw-rw-rw-   0        0        0      717 2022-09-03 06:29:01.000000 riyazi-0.16/riyazi/algebra/_product.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.638302 riyazi-0.16/riyazi/constants/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.639299 riyazi-0.16/riyazi/constants/Strings/
--rw-rw-rw-   0        0        0      524 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/Strings/mmu.py
--rw-rw-rw-   0        0        0      615 2023-04-01 11:30:36.000000 riyazi-0.16/riyazi/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.644390 riyazi-0.16/riyazi/constants/calculation/
--rw-rw-rw-   0        0        0      129 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/calculation/Binary_prefixes.py
--rw-rw-rw-   0        0        0      285 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/calculation/SI_prefixes.py
--rw-rw-rw-   0        0        0       58 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/calculation/__init__.py
--rw-rw-rw-   0        0        0     5402 2023-02-02 13:02:16.000000 riyazi-0.16/riyazi/constants/codatamath.py
--rw-rw-rw-   0        0        0     1379 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/codatamath_function.py
--rw-rw-rw-   0        0        0      785 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/codataphy.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.651667 riyazi-0.16/riyazi/constants/testing/
--rw-rw-rw-   0        0        0    11715 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/testing/__init__.py
--rw-rw-rw-   0        0        0     3772 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/testing/codatamath.py
--rw-rw-rw-   0        0        0      217 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/testing/codataphy.py
--rw-rw-rw-   0        0        0     2017 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/testing/math.py
--rw-rw-rw-   0        0        0     5413 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/testing/physics.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.653667 riyazi-0.16/riyazi/constants/tests/
--rw-rw-rw-   0        0        0      321 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/tests/mm.py
--rw-rw-rw-   0        0        0      129 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/constants/tests/time.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.656674 riyazi-0.16/riyazi/crypto/
--rw-rw-rw-   0        0        0       19 2022-11-08 04:16:23.000000 riyazi-0.16/riyazi/crypto/__init__.py
--rw-rw-rw-   0        0        0     2910 2022-11-08 04:11:36.000000 riyazi-0.16/riyazi/crypto/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.438381 riyazi-0.16/riyazi/crypto/ciphers/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.659670 riyazi-0.16/riyazi/crypto/ciphers/testing/
--rw-rw-rw-   0        0        0      429 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/ciphers/testing/cryptomath_module.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.675095 riyazi-0.16/riyazi/crypto/hashes/
--rw-rw-rw-   0        0        0      786 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/adler32.py
--rw-rw-rw-   0        0        0     2423 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/chaos_machine.py
--rw-rw-rw-   0        0        0      871 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/djb2.py
--rw-rw-rw-   0        0        0     1704 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/enigma_machine.py
--rw-rw-rw-   0        0        0     9401 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/hamming_code.py
--rw-rw-rw-   0        0        0     1233 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/luhn.py
--rw-rw-rw-   0        0        0     4652 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/md5.py
--rw-rw-rw-   0        0        0     1342 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/sdbm.py
--rw-rw-rw-   0        0        0     6530 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/sha1.py
--rw-rw-rw-   0        0        0     7183 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/crypto/hashes/sha256.py
--rw-rw-rw-   0        0        0      629 2023-03-29 10:38:20.000000 riyazi-0.16/riyazi/crypto/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.676104 riyazi-0.16/riyazi/easymath/
--rw-rw-rw-   0        0        0       41 2022-11-26 12:49:26.000000 riyazi-0.16/riyazi/easymath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.681719 riyazi-0.16/riyazi/easymath/automata/
--rw-rw-rw-   0        0        0       19 2020-10-04 14:40:32.000000 riyazi-0.16/riyazi/easymath/automata/__init__.py
--rw-rw-rw-   0        0        0      371 2020-10-04 14:40:32.000000 riyazi-0.16/riyazi/easymath/automata/dfa.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.684719 riyazi-0.16/riyazi/fft/
--rw-rw-rw-   0        0        0      932 2018-06-19 23:16:08.000000 riyazi-0.16/riyazi/fft/Generaldistribution.py
--rw-rw-rw-   0        0        0      234 2023-01-10 05:14:55.000000 riyazi-0.16/riyazi/fft/__init__.py
--rw-rw-rw-   0        0        0      697 2023-03-30 06:05:36.000000 riyazi-0.16/riyazi/fft/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.445542 riyazi-0.16/riyazi/fft/testing/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.450546 riyazi-0.16/riyazi/fft/testing/scipy/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.686716 riyazi-0.16/riyazi/fft/testing/scipy/backendcontrol/
--rw-rw-rw-   0        0        0       30 2023-01-10 05:10:45.000000 riyazi-0.16/riyazi/fft/testing/scipy/backendcontrol/__init__.py
--rw-rw-rw-   0        0        0      231 2023-01-10 05:10:15.000000 riyazi-0.16/riyazi/fft/testing/scipy/backendcontrol/_backendcontrol.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.688716 riyazi-0.16/riyazi/fft/testing/scipy/discrete_sc/
--rw-rw-rw-   0        0        0       20 2023-01-10 04:31:18.000000 riyazi-0.16/riyazi/fft/testing/scipy/discrete_sc/__init__.py
--rw-rw-rw-   0        0        0     1769 2022-11-26 04:11:34.000000 riyazi-0.16/riyazi/fft/testing/scipy/discrete_sc/_dsct.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.691719 riyazi-0.16/riyazi/fft/testing/scipy/fast_fourier_transormation/
--rw-rw-rw-   0        0        0       20 2023-01-10 04:27:45.000000 riyazi-0.16/riyazi/fft/testing/scipy/fast_fourier_transormation/__init__.py
--rw-rw-rw-   0        0        0     1811 2023-01-10 04:27:00.000000 riyazi-0.16/riyazi/fft/testing/scipy/fast_fourier_transormation/_ffts.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.698269 riyazi-0.16/riyazi/fft/testing/scipy/fast_hankeltrans/
--rw-rw-rw-   0        0        0       19 2023-01-10 04:55:24.000000 riyazi-0.16/riyazi/fft/testing/scipy/fast_hankeltrans/__init__.py
--rw-rw-rw-   0        0        0       73 2023-01-10 04:54:52.000000 riyazi-0.16/riyazi/fft/testing/scipy/fast_hankeltrans/_fht.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.700267 riyazi-0.16/riyazi/fft/testing/scipy/helperfunction/
--rw-rw-rw-   0        0        0       25 2023-01-10 04:57:39.000000 riyazi-0.16/riyazi/fft/testing/scipy/helperfunction/__init__.py
--rw-rw-rw-   0        0        0      369 2023-01-10 05:02:22.000000 riyazi-0.16/riyazi/fft/testing/scipy/helperfunction/_helperfun.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.703639 riyazi-0.16/riyazi/geometry/
--rw-rw-rw-   0        0        0       44 2023-03-31 05:00:05.000000 riyazi-0.16/riyazi/geometry/__init__.py
--rw-rw-rw-   0        0        0      688 2023-03-29 10:39:06.000000 riyazi-0.16/riyazi/geometry/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.716401 riyazi-0.16/riyazi/geometry/three_dim/
--rw-rw-rw-   0        0        0      234 2023-03-31 05:06:31.000000 riyazi-0.16/riyazi/geometry/three_dim/__init__.py
--rw-rw-rw-   0        0        0      307 2022-09-28 15:11:48.000000 riyazi-0.16/riyazi/geometry/three_dim/acute.py
--rw-rw-rw-   0        0        0       66 2022-09-08 07:08:27.000000 riyazi-0.16/riyazi/geometry/three_dim/cone.py
--rw-rw-rw-   0        0        0       39 2023-03-31 05:03:57.000000 riyazi-0.16/riyazi/geometry/three_dim/cube.py
--rw-rw-rw-   0        0        0      103 2022-09-08 07:41:08.000000 riyazi-0.16/riyazi/geometry/three_dim/cylinder.py
--rw-rw-rw-   0        0        0       52 2023-03-31 05:04:07.000000 riyazi-0.16/riyazi/geometry/three_dim/pyramid.py
--rw-rw-rw-   0        0        0       66 2022-09-08 06:53:41.000000 riyazi-0.16/riyazi/geometry/three_dim/rectangle_prism.py
--rw-rw-rw-   0        0        0       97 2022-09-08 06:54:02.000000 riyazi-0.16/riyazi/geometry/three_dim/sphere.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.717400 riyazi-0.16/riyazi/geometry/three_dim/testing/
--rw-rw-rw-   0        0        0        0 2022-09-09 05:49:46.000000 riyazi-0.16/riyazi/geometry/three_dim/testing/hemisphere.py
--rw-rw-rw-   0        0        0        0 2022-09-09 05:49:31.000000 riyazi-0.16/riyazi/geometry/three_dim/testing/sphere.py
--rw-rw-rw-   0        0        0      186 2022-09-08 06:54:29.000000 riyazi-0.16/riyazi/geometry/three_dim/triangle_prism.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.720404 riyazi-0.16/riyazi/geometry/two_dim/
--rw-rw-rw-   0        0        0      910 2022-11-19 12:44:49.000000 riyazi-0.16/riyazi/geometry/two_dim/circle.py
--rw-rw-rw-   0        0        0      239 2022-09-08 05:14:29.000000 riyazi-0.16/riyazi/geometry/two_dim/rectangle.py
--rw-rw-rw-   0        0        0      863 2022-09-06 02:46:08.000000 riyazi-0.16/riyazi/geometry/two_dim/square.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.722406 riyazi-0.16/riyazi/geometry/two_dim/test/
--rw-rw-rw-   0        0        0      100 2022-11-19 12:43:50.000000 riyazi-0.16/riyazi/geometry/two_dim/test/__int__.py
--rw-rw-rw-   0        0        0     5576 2022-11-20 07:21:37.000000 riyazi-0.16/riyazi/geometry/two_dim/test/dim2.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.457538 riyazi-0.16/riyazi/integrate/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.459560 riyazi-0.16/riyazi/integrate/testing/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.723404 riyazi-0.16/riyazi/integrate/testing/scipy/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.724403 riyazi-0.16/riyazi/integrate/testing/scipy/_ivp/
--rw-rw-rw-   0        0        0      161 2023-01-11 04:58:32.000000 riyazi-0.16/riyazi/integrate/testing/scipy/_ivp/ivp.py
--rw-rw-rw-   0        0        0      172 2023-01-11 04:54:31.000000 riyazi-0.16/riyazi/integrate/testing/scipy/_quadture.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.726485 riyazi-0.16/riyazi/interpolate/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:42:10.000000 riyazi-0.16/riyazi/interpolate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.728490 riyazi-0.16/riyazi/interpolate/testing/
--rw-rw-rw-   0        0        0      776 2023-01-11 05:11:35.000000 riyazi-0.16/riyazi/interpolate/testing/_interpolate.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.733487 riyazi-0.16/riyazi/linalg/
--rw-rw-rw-   0        0        0     2287 2022-11-10 13:10:05.000000 riyazi-0.16/riyazi/linalg/Decompositions.py
--rw-rw-rw-   0        0        0       52 2022-11-11 06:13:20.000000 riyazi-0.16/riyazi/linalg/__init__.py
--rw-rw-rw-   0        0        0     5630 2023-03-31 05:10:51.000000 riyazi-0.16/riyazi/linalg/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.735489 riyazi-0.16/riyazi/linalg/testing/
--rw-rw-rw-   0        0        0        0 2022-09-21 05:14:22.000000 riyazi-0.16/riyazi/linalg/testing/inv.py
--rw-rw-rw-   0        0        0        0 2022-09-21 05:15:04.000000 riyazi-0.16/riyazi/linalg/testing/pinv.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.469268 riyazi-0.16/riyazi/linalg/testing/scipy/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.737486 riyazi-0.16/riyazi/linalg/testing/scipy/Basics/
--rw-rw-rw-   0        0        0      682 2022-11-13 05:58:59.000000 riyazi-0.16/riyazi/linalg/testing/scipy/Basics/__basics.py
--rw-rw-rw-   0        0        0       22 2022-11-13 05:39:49.000000 riyazi-0.16/riyazi/linalg/testing/scipy/Basics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.738486 riyazi-0.16/riyazi/linalg/testing/scipy/Decompositions/
--rw-rw-rw-   0        0        0      300 2023-01-11 05:20:14.000000 riyazi-0.16/riyazi/linalg/testing/scipy/Decompositions/_decom.py
--rw-rw-rw-   0        0        0        0 2022-09-21 05:15:23.000000 riyazi-0.16/riyazi/linalg/testing/solve.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.739488 riyazi-0.16/riyazi/math/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.744557 riyazi-0.16/riyazi/math/Research/
--rw-rw-rw-   0        0        0       27 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/Research/__init__.py
--rw-rw-rw-   0        0        0       86 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/Research/numbermath.py
--rw-rw-rw-   0        0        0      167 2023-03-30 05:30:43.000000 riyazi-0.16/riyazi/math/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.751332 riyazi-0.16/riyazi/math/_logarithms/
--rw-rw-rw-   0        0        0       43 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_logarithms/__init__.py
--rw-rw-rw-   0        0        0     2000 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_logarithms/_doc_log.py
--rw-rw-rw-   0        0        0      587 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_logarithms/_log.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.754334 riyazi-0.16/riyazi/math/_logic/
--rw-rw-rw-   0        0        0       22 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_logic/__init__.py
--rw-rw-rw-   0        0        0      404 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_logic/_bitwise.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.759343 riyazi-0.16/riyazi/math/_numeric/
--rw-rw-rw-   0        0        0       24 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_numeric/__init__.py
--rw-rw-rw-   0        0        0     4659 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_numeric/basic.py
--rw-rw-rw-   0        0        0    12641 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_numeric/doc_numerics.py
--rw-rw-rw-   0        0        0    14096 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_numeric/numerics.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.767332 riyazi-0.16/riyazi/math/_sets/
--rw-rw-rw-   0        0        0       18 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_sets/__init__.py
--rw-rw-rw-   0        0        0      526 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_sets/doc_set.py
--rw-rw-rw-   0        0        0     1054 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_sets/set.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.770331 riyazi-0.16/riyazi/math/_trigonometry/
--rw-rw-rw-   0        0        0       46 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_trigonometry/__init__.py
--rw-rw-rw-   0        0        0     3108 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_trigonometry/_trig.py
--rw-rw-rw-   0        0        0    10884 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_trigonometry/doc_trig.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.771332 riyazi-0.16/riyazi/math/_trigonometry/legacy/
--rw-rw-rw-   0        0        0       92 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_trigonometry/legacy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.772331 riyazi-0.16/riyazi/math/_trigonometry/tests/
--rw-rw-rw-   0        0        0      571 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/_trigonometry/tests/complex.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.778349 riyazi-0.16/riyazi/math/mpmath/
--rw-rw-rw-   0        0        0      235 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/mpmath/Exponential_integrals_and_error_functions.py
--rw-rw-rw-   0        0        0      310 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/mpmath/Hypergeometric_function.py
--rw-rw-rw-   0        0        0     2989 2023-02-02 12:38:49.000000 riyazi-0.16/riyazi/math/mpmath/power_and_logartihm.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.782332 riyazi-0.16/riyazi/matrix/
--rw-rw-rw-   0        0        0       22 2022-11-10 07:36:37.000000 riyazi-0.16/riyazi/matrix/__init__.py
--rw-rw-rw-   0        0        0     3674 2022-11-10 07:46:53.000000 riyazi-0.16/riyazi/matrix/matrices.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.783331 riyazi-0.16/riyazi/ndimage/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:44:01.000000 riyazi-0.16/riyazi/ndimage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.485457 riyazi-0.16/riyazi/numerical/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.485457 riyazi-0.16/riyazi/numerical/numerica/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.486467 riyazi-0.16/riyazi/numerical/numerica/differentiation/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.787333 riyazi-0.16/riyazi/numerical/numerica/differentiation/euler/
--rw-rw-rw-   0        0        0        0 2021-03-01 10:53:17.000000 riyazi-0.16/riyazi/numerical/numerica/differentiation/euler/__init__.py
--rw-rw-rw-   0        0        0      148 2021-03-01 10:53:17.000000 riyazi-0.16/riyazi/numerical/numerica/differentiation/euler/backward.py
--rw-rw-rw-   0        0        0      147 2021-03-01 10:53:17.000000 riyazi-0.16/riyazi/numerical/numerica/differentiation/euler/forward.py
--rw-rw-rw-   0        0        0      166 2021-03-01 10:53:17.000000 riyazi-0.16/riyazi/numerical/numerica/differentiation/euler/midpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.788333 riyazi-0.16/riyazi/odr/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:44:50.000000 riyazi-0.16/riyazi/odr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.790335 riyazi-0.16/riyazi/optimize/
--rw-rw-rw-   0        0        0       25 2022-11-16 02:49:45.000000 riyazi-0.16/riyazi/optimize/__init__.py
--rw-rw-rw-   0        0        0     1376 2022-11-16 02:49:28.000000 riyazi-0.16/riyazi/optimize/bisection.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.794572 riyazi-0.16/riyazi/physics/
--rw-rw-rw-   0        0        0       25 2022-11-14 10:34:35.000000 riyazi-0.16/riyazi/physics/__basics.py
--rw-rw-rw-   0        0        0       22 2022-11-14 08:48:15.000000 riyazi-0.16/riyazi/physics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.797565 riyazi-0.16/riyazi/physics/constants/
--rw-rw-rw-   0        0        0      127 2022-11-17 05:27:15.000000 riyazi-0.16/riyazi/physics/constants/codata.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.803548 riyazi-0.16/riyazi/physics/electronics/
--rw-rw-rw-   0        0        0      117 2022-11-14 10:34:09.000000 riyazi-0.16/riyazi/physics/electronics/__basics.py
--rw-rw-rw-   0        0        0     2887 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/electronics/carrier_concentration.py
--rw-rw-rw-   0        0        0     2713 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/electronics/coulombs_law.py
--rw-rw-rw-   0        0        0     1973 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/electronics/electric_power.py
--rw-rw-rw-   0        0        0     1459 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/electronics/ohms_law.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.815988 riyazi-0.16/riyazi/physics/quantum/
--rw-rw-rw-   0        0        0        0 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/__init__.py
--rw-rw-rw-   0        0        0     4428 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/deutsch_jozsa.py
--rw-rw-rw-   0        0        0     1547 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/half_adder.py
--rw-rw-rw-   0        0        0     1237 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/not_gate.py
--rw-rw-rw-   0        0        0     1960 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/quantum_entanglement.py
--rw-rw-rw-   0        0        0     3608 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/ripple_adder_classic.py
--rw-rw-rw-   0        0        0     1076 2022-09-24 17:04:00.000000 riyazi-0.16/riyazi/physics/quantum/single_qubit_measure.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.817988 riyazi-0.16/riyazi/polynomial/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.819987 riyazi-0.16/riyazi/polynomial/HermiteE/
--rw-rw-rw-   0        0        0       24 2023-04-05 06:59:31.000000 riyazi-0.16/riyazi/polynomial/HermiteE/__init__.py
--rw-rw-rw-   0        0        0    18508 2023-04-05 07:02:08.000000 riyazi-0.16/riyazi/polynomial/HermiteE/_hermite_e.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.821987 riyazi-0.16/riyazi/polynomial/Laguerre/
--rw-rw-rw-   0        0        0       23 2023-04-05 06:59:55.000000 riyazi-0.16/riyazi/polynomial/Laguerre/__init__.py
--rw-rw-rw-   0        0        0    18084 2023-04-05 07:01:37.000000 riyazi-0.16/riyazi/polynomial/Laguerre/_laguerre.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.823986 riyazi-0.16/riyazi/polynomial/Legendre/
--rw-rw-rw-   0        0        0       23 2023-04-05 07:04:28.000000 riyazi-0.16/riyazi/polynomial/Legendre/__init__.py
--rw-rw-rw-   0        0        0    18007 2023-04-05 07:01:21.000000 riyazi-0.16/riyazi/polynomial/Legendre/_legendre.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.828331 riyazi-0.16/riyazi/polynomial/Polynomial/
--rw-rw-rw-   0        0        0       26 2023-04-05 07:00:49.000000 riyazi-0.16/riyazi/polynomial/Polynomial/__init__.py
--rw-rw-rw-   0        0        0    18285 2023-04-05 07:08:24.000000 riyazi-0.16/riyazi/polynomial/Polynomial/_polynomial.py
--rw-rw-rw-   0        0        0      139 2023-04-05 07:03:32.000000 riyazi-0.16/riyazi/polynomial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.833322 riyazi-0.16/riyazi/polynomial/chebyshev/
--rw-rw-rw-   0        0        0       24 2023-04-04 06:19:41.000000 riyazi-0.16/riyazi/polynomial/chebyshev/__init__.py
--rw-rw-rw-   0        0        0    23012 2023-04-04 05:50:51.000000 riyazi-0.16/riyazi/polynomial/chebyshev/_chebyshev.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.836326 riyazi-0.16/riyazi/polynomial/hermite/
--rw-rw-rw-   0        0        0       21 2023-04-04 06:20:38.000000 riyazi-0.16/riyazi/polynomial/hermite/__init__.py
--rw-rw-rw-   0        0        0    18704 2023-04-03 14:38:24.000000 riyazi-0.16/riyazi/polynomial/hermite/hermite.py
--rw-rw-rw-   0        0        0    10226 2023-04-04 06:15:18.000000 riyazi-0.16/riyazi/polynomial/polyutils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.838362 riyazi-0.16/riyazi/polynomial/testing/
--rw-rw-rw-   0        0        0       25 2022-09-16 10:33:59.000000 riyazi-0.16/riyazi/polynomial/testing/__init__.py
--rw-rw-rw-   0        0        0      337 2022-11-26 12:55:29.000000 riyazi-0.16/riyazi/polynomial/testing/quadratic.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.502829 riyazi-0.16/riyazi/scimath/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.839361 riyazi-0.16/riyazi/scimath/random/
--rw-rw-rw-   0        0        0       22 2022-12-02 13:07:04.000000 riyazi-0.16/riyazi/scimath/random/random.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.840362 riyazi-0.16/riyazi/series/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:46:40.000000 riyazi-0.16/riyazi/series/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-03-31 04:55:10.000000 riyazi-0.16/riyazi/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.841363 riyazi-0.16/riyazi/signal/
--rw-rw-rw-   0        0        0       30 2023-01-19 03:31:55.000000 riyazi-0.16/riyazi/signal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.843380 riyazi-0.16/riyazi/signal/testing/
--rw-rw-rw-   0        0        0     1166 2023-03-31 05:12:04.000000 riyazi-0.16/riyazi/signal/testing/_signal.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.846388 riyazi-0.16/riyazi/sparse/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:47:34.000000 riyazi-0.16/riyazi/sparse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.848360 riyazi-0.16/riyazi/spatial/
--rw-rw-rw-   0        0        0        0 2023-03-31 04:48:22.000000 riyazi-0.16/riyazi/spatial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.849361 riyazi-0.16/riyazi/special/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.516914 riyazi-0.16/riyazi/special/__funtions_mpmath__/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.850361 riyazi-0.16/riyazi/special/__funtions_mpmath__/calculus/
--rw-rw-rw-   0        0        0       26 2023-02-03 09:30:06.000000 riyazi-0.16/riyazi/special/__funtions_mpmath__/calculus/_basic.py
--rw-rw-rw-   0        0        0      828 2023-01-10 04:06:13.000000 riyazi-0.16/riyazi/special/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.556467 riyazi-0.16/riyazi/special/testing/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.852362 riyazi-0.16/riyazi/special/testing/Other_special_functions/
--rw-rw-rw-   0        0        0       27 2023-01-09 06:25:53.000000 riyazi-0.16/riyazi/special/testing/Other_special_functions/__init__.py
--rw-rw-rw-   0        0        0     2503 2023-01-09 06:29:11.000000 riyazi-0.16/riyazi/special/testing/Other_special_functions/otherspsfunc.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.854364 riyazi-0.16/riyazi/special/testing/airy/
--rw-rw-rw-   0        0        0       19 2023-01-08 13:04:44.000000 riyazi-0.16/riyazi/special/testing/airy/__init__.py
--rw-rw-rw-   0        0        0     1003 2022-12-31 12:42:17.000000 riyazi-0.16/riyazi/special/testing/airy/airy.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.867542 riyazi-0.16/riyazi/special/testing/bessel/
--rw-rw-rw-   0        0        0      152 2023-01-08 11:27:09.000000 riyazi-0.16/riyazi/special/testing/bessel/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-01-08 04:21:05.000000 riyazi-0.16/riyazi/special/testing/bessel/bessel_function.py
--rw-rw-rw-   0        0        0      649 2023-01-08 11:17:22.000000 riyazi-0.16/riyazi/special/testing/bessel/common_bessel.py
--rw-rw-rw-   0        0        0      548 2023-01-08 11:26:39.000000 riyazi-0.16/riyazi/special/testing/bessel/drivative_bessel.py
--rw-rw-rw-   0        0        0      218 2023-01-08 12:50:25.000000 riyazi-0.16/riyazi/special/testing/bessel/integralbessel.py
--rw-rw-rw-   0        0        0      311 2023-01-08 05:27:01.000000 riyazi-0.16/riyazi/special/testing/bessel/riccati_bessel.py
--rw-rw-rw-   0        0        0      725 2023-01-08 05:54:46.000000 riyazi-0.16/riyazi/special/testing/bessel/sphe_bessel.py
--rw-rw-rw-   0        0        0      128 2023-01-01 07:34:08.000000 riyazi-0.16/riyazi/special/testing/bessel/zerosbessel.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.869543 riyazi-0.16/riyazi/special/testing/combinatorics/
--rw-rw-rw-   0        0        0       28 2023-01-09 12:22:25.000000 riyazi-0.16/riyazi/special/testing/combinatorics/__init__.py
--rw-rw-rw-   0        0        0       67 2023-01-09 12:21:41.000000 riyazi-0.16/riyazi/special/testing/combinatorics/combinatorics.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.873547 riyazi-0.16/riyazi/special/testing/convenience/
--rw-rw-rw-   0        0        0       56 2023-01-09 06:21:57.000000 riyazi-0.16/riyazi/special/testing/convenience/__init__.py
--rw-rw-rw-   0        0        0     1546 2022-12-30 16:02:54.000000 riyazi-0.16/riyazi/special/testing/convenience/convenience.py
--rw-rw-rw-   0        0        0     5427 2023-01-09 06:21:18.000000 riyazi-0.16/riyazi/special/testing/convenience/doc_convenience.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.875079 riyazi-0.16/riyazi/special/testing/ellipintegral/
--rw-rw-rw-   0        0        0      133 2023-01-01 07:27:39.000000 riyazi-0.16/riyazi/special/testing/ellipintegral/ellipintegral.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.549576 riyazi-0.16/riyazi/special/testing/errorintegral/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.882221 riyazi-0.16/riyazi/special/testing/errorintegral/testing/
--rw-rw-rw-   0        0        0       36 2023-01-09 05:47:32.000000 riyazi-0.16/riyazi/special/testing/errorintegral/testing/__init__.py
--rw-rw-rw-   0        0        0      866 2023-01-09 05:44:30.000000 riyazi-0.16/riyazi/special/testing/errorintegral/testing/error_frasnelintegral.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.884224 riyazi-0.16/riyazi/special/testing/gammarelt/
--rw-rw-rw-   0        0        0       27 2023-01-09 05:48:19.000000 riyazi-0.16/riyazi/special/testing/gammarelt/__init__.py
--rw-rw-rw-   0        0        0     1037 2023-01-09 05:36:53.000000 riyazi-0.16/riyazi/special/testing/gammarelt/gamma_related.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.886225 riyazi-0.16/riyazi/special/testing/hypergeometric/
--rw-rw-rw-   0        0        0       25 2023-01-10 03:32:13.000000 riyazi-0.16/riyazi/special/testing/hypergeometric/__init__.py
--rw-rw-rw-   0        0        0      167 2023-01-10 03:14:59.000000 riyazi-0.16/riyazi/special/testing/hypergeometric/_hypergeom.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.888220 riyazi-0.16/riyazi/special/testing/infotheory/
--rw-rw-rw-   0        0        0       23 2023-01-09 05:24:42.000000 riyazi-0.16/riyazi/special/testing/infotheory/__init__.py
--rw-rw-rw-   0        0        0      831 2023-01-09 05:33:16.000000 riyazi-0.16/riyazi/special/testing/infotheory/infothry.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.890232 riyazi-0.16/riyazi/special/testing/kelvin/
--rw-rw-rw-   0        0        0       21 2023-01-10 03:41:32.000000 riyazi-0.16/riyazi/special/testing/kelvin/__init__.py
--rw-rw-rw-   0        0        0      732 2023-01-10 03:48:16.000000 riyazi-0.16/riyazi/special/testing/kelvin/_kelvin.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.894372 riyazi-0.16/riyazi/special/testing/lambertwrelt/
--rw-rw-rw-   0        0        0       30 2023-01-09 12:56:54.000000 riyazi-0.16/riyazi/special/testing/lambertwrelt/__init__.py
--rw-rw-rw-   0        0        0      879 2023-01-09 12:56:23.000000 riyazi-0.16/riyazi/special/testing/lambertwrelt/lambert_related.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.899496 riyazi-0.16/riyazi/special/testing/legendre/
--rw-rw-rw-   0        0        0       23 2023-01-09 05:52:23.000000 riyazi-0.16/riyazi/special/testing/legendre/__init__.py
--rw-rw-rw-   0        0        0      693 2023-01-01 05:50:35.000000 riyazi-0.16/riyazi/special/testing/legendre/legendre.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.901494 riyazi-0.16/riyazi/special/testing/mathieu_related/
--rw-rw-rw-   0        0        0       23 2023-01-10 04:01:30.000000 riyazi-0.16/riyazi/special/testing/mathieu_related/__init__.py
--rw-rw-rw-   0        0        0      529 2023-01-10 04:00:30.000000 riyazi-0.16/riyazi/special/testing/mathieu_related/_mathieu.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.903495 riyazi-0.16/riyazi/special/testing/parabolic_cylinder/
--rw-rw-rw-   0        0        0       24 2023-01-10 03:19:15.000000 riyazi-0.16/riyazi/special/testing/parabolic_cylinder/__init__.py
--rw-rw-rw-   0        0        0      233 2023-01-10 03:27:48.000000 riyazi-0.16/riyazi/special/testing/parabolic_cylinder/pbcylinder.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.908147 riyazi-0.16/riyazi/special/testing/raw_statistical/
--rw-rw-rw-   0        0        0       22 2023-01-09 05:18:51.000000 riyazi-0.16/riyazi/special/testing/raw_statistical/__init__.py
--rw-rw-rw-   0        0        0     1526 2023-01-09 05:21:41.000000 riyazi-0.16/riyazi/special/testing/raw_statistical/rwstats.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.916214 riyazi-0.16/riyazi/special/testing/spheroidal_wave/
--rw-rw-rw-   0        0        0       27 2023-01-10 04:05:45.000000 riyazi-0.16/riyazi/special/testing/spheroidal_wave/__init__.py
--rw-rw-rw-   0        0        0      502 2023-01-10 04:04:44.000000 riyazi-0.16/riyazi/special/testing/spheroidal_wave/_spheroidwav.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.920990 riyazi-0.16/riyazi/special/testing/struve/
--rw-rw-rw-   0        0        0       30 2023-01-09 05:08:52.000000 riyazi-0.16/riyazi/special/testing/struve/__init__.py
--rw-rw-rw-   0        0        0      545 2023-01-09 05:08:14.000000 riyazi-0.16/riyazi/special/testing/struve/struve_function.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.926816 riyazi-0.16/riyazi/stats/
--rw-rw-rw-   0        0        0       21 2023-01-13 05:04:31.000000 riyazi-0.16/riyazi/stats/__init__.py
--rw-rw-rw-   0        0        0     6444 2022-11-08 13:11:13.000000 riyazi-0.16/riyazi/stats/_basics.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.559028 riyazi-0.16/riyazi/stats/probability/
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.932710 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/
--rw-rw-rw-   0        0        0        0 2023-01-13 04:43:14.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/__init__.py
--rw-rw-rw-   0        0        0       31 2023-01-13 04:44:55.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/ddf.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.939218 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/
--rw-rw-rw-   0        0        0        0 2022-11-12 01:45:27.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/Benfords_distribution.py
--rw-rw-rw-   0        0        0     1531 2022-11-11 13:34:44.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/Bernoulli_distributions.py
--rw-rw-rw-   0        0        0      508 2022-11-10 01:21:05.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/Binomial_distributions.py
--rw-rw-rw-   0        0        0        0 2022-11-12 01:45:53.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/Poisson_binomial.py
--rw-rw-rw-   0        0        0       76 2022-11-09 03:15:54.000000 riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.944218 riyazi-0.16/riyazi/stats/testing/
--rw-rw-rw-   0        0        0       55 2022-09-15 05:52:23.000000 riyazi-0.16/riyazi/stats/testing/__init__.py
--rw-rw-rw-   0        0        0      246 2022-09-15 06:00:04.000000 riyazi-0.16/riyazi/stats/testing/combination.py
--rw-rw-rw-   0        0        0     1183 2022-09-22 06:58:57.000000 riyazi-0.16/riyazi/stats/testing/percentile .py
--rw-rw-rw-   0        0        0      199 2022-09-15 05:57:50.000000 riyazi-0.16/riyazi/stats/testing/permutation.py
--rw-rw-rw-   0        0        0      193 2023-04-09 06:03:05.000000 riyazi-0.16/riyazi/version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:03:57.617499 riyazi-0.16/riyazi.egg-info/
--rw-rw-rw-   0        0        0      143 2023-04-09 06:03:56.000000 riyazi-0.16/riyazi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8762 2023-04-09 06:03:57.000000 riyazi-0.16/riyazi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:03:56.000000 riyazi-0.16/riyazi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 06:03:56.000000 riyazi-0.16/riyazi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:03:57.949358 riyazi-0.16/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-09 06:02:32.000000 riyazi-0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.812605 riyazi-0.17/
+-rw-rw-rw-   0        0        0     1526 2023-02-02 12:38:49.000000 riyazi-0.17/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-04-18 06:45:11.811604 riyazi-0.17/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-04-03 11:13:54.000000 riyazi-0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.448619 riyazi-0.17/riyazi/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.491273 riyazi-0.17/riyazi/Module/
+-rw-rw-rw-   0        0        0      440 2022-11-13 07:09:57.000000 riyazi-0.17/riyazi/Module/__fornumerics.py
+-rw-rw-rw-   0        0        0       27 2022-11-13 06:32:33.000000 riyazi-0.17/riyazi/Module/__init__.py
+-rw-rw-rw-   0        0        0      980 2022-09-01 09:12:38.000000 riyazi-0.17/riyazi/Module/main.py
+-rw-rw-rw-   0        0        0      219 2022-09-09 15:48:35.000000 riyazi-0.17/riyazi/Module/module.py
+-rw-rw-rw-   0        0        0     2236 2022-09-28 02:56:20.000000 riyazi-0.17/riyazi/Module/mymodule.py
+-rw-rw-rw-   0        0        0     1498 2022-09-27 13:10:35.000000 riyazi-0.17/riyazi/Module/numeric.py
+-rw-rw-rw-   0        0        0      569 2023-03-31 04:49:26.000000 riyazi-0.17/riyazi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.500320 riyazi-0.17/riyazi/algebra/
+-rw-rw-rw-   0        0        0       79 2023-04-01 05:03:00.000000 riyazi-0.17/riyazi/algebra/__init__.py
+-rw-rw-rw-   0        0        0      535 2022-09-03 06:06:18.000000 riyazi-0.17/riyazi/algebra/_factor.py
+-rw-rw-rw-   0        0        0      248 2023-03-30 05:44:16.000000 riyazi-0.17/riyazi/algebra/_law_exp.py
+-rw-rw-rw-   0        0        0      717 2022-09-03 06:29:01.000000 riyazi-0.17/riyazi/algebra/_product.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.506452 riyazi-0.17/riyazi/constants/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.508451 riyazi-0.17/riyazi/constants/Strings/
+-rw-rw-rw-   0        0        0      524 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/Strings/mmu.py
+-rw-rw-rw-   0        0        0      615 2023-04-01 11:30:36.000000 riyazi-0.17/riyazi/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.515382 riyazi-0.17/riyazi/constants/calculation/
+-rw-rw-rw-   0        0        0      129 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/calculation/Binary_prefixes.py
+-rw-rw-rw-   0        0        0      285 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/calculation/SI_prefixes.py
+-rw-rw-rw-   0        0        0       58 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/calculation/__init__.py
+-rw-rw-rw-   0        0        0     5402 2023-02-02 13:02:16.000000 riyazi-0.17/riyazi/constants/codatamath.py
+-rw-rw-rw-   0        0        0     1379 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/codatamath_function.py
+-rw-rw-rw-   0        0        0      785 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/codataphy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.520384 riyazi-0.17/riyazi/constants/testing/
+-rw-rw-rw-   0        0        0    11715 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/testing/__init__.py
+-rw-rw-rw-   0        0        0     3772 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/testing/codatamath.py
+-rw-rw-rw-   0        0        0      217 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/testing/codataphy.py
+-rw-rw-rw-   0        0        0     2017 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/testing/math.py
+-rw-rw-rw-   0        0        0     5413 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/testing/physics.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.522382 riyazi-0.17/riyazi/constants/tests/
+-rw-rw-rw-   0        0        0      321 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/tests/mm.py
+-rw-rw-rw-   0        0        0      129 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/constants/tests/time.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.526383 riyazi-0.17/riyazi/crypto/
+-rw-rw-rw-   0        0        0       19 2022-11-08 04:16:23.000000 riyazi-0.17/riyazi/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2910 2022-11-08 04:11:36.000000 riyazi-0.17/riyazi/crypto/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.335371 riyazi-0.17/riyazi/crypto/ciphers/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.530751 riyazi-0.17/riyazi/crypto/ciphers/testing/
+-rw-rw-rw-   0        0        0      429 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/ciphers/testing/cryptomath_module.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.546402 riyazi-0.17/riyazi/crypto/hashes/
+-rw-rw-rw-   0        0        0      786 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/adler32.py
+-rw-rw-rw-   0        0        0     2423 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/chaos_machine.py
+-rw-rw-rw-   0        0        0      871 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/djb2.py
+-rw-rw-rw-   0        0        0     1704 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/enigma_machine.py
+-rw-rw-rw-   0        0        0     9401 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/hamming_code.py
+-rw-rw-rw-   0        0        0     1233 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/luhn.py
+-rw-rw-rw-   0        0        0     4652 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/md5.py
+-rw-rw-rw-   0        0        0     1342 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/sdbm.py
+-rw-rw-rw-   0        0        0     6530 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/sha1.py
+-rw-rw-rw-   0        0        0     7183 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/crypto/hashes/sha256.py
+-rw-rw-rw-   0        0        0      629 2023-03-29 10:38:20.000000 riyazi-0.17/riyazi/crypto/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.546402 riyazi-0.17/riyazi/easymath/
+-rw-rw-rw-   0        0        0       41 2022-11-26 12:49:26.000000 riyazi-0.17/riyazi/easymath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.548402 riyazi-0.17/riyazi/easymath/automata/
+-rw-rw-rw-   0        0        0       19 2020-10-04 14:40:32.000000 riyazi-0.17/riyazi/easymath/automata/__init__.py
+-rw-rw-rw-   0        0        0      371 2020-10-04 14:40:32.000000 riyazi-0.17/riyazi/easymath/automata/dfa.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.551404 riyazi-0.17/riyazi/fft/
+-rw-rw-rw-   0        0        0      932 2018-06-19 23:16:08.000000 riyazi-0.17/riyazi/fft/Generaldistribution.py
+-rw-rw-rw-   0        0        0      234 2023-01-10 05:14:55.000000 riyazi-0.17/riyazi/fft/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-03-30 06:05:36.000000 riyazi-0.17/riyazi/fft/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.343181 riyazi-0.17/riyazi/fft/testing/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.349192 riyazi-0.17/riyazi/fft/testing/scipy/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.554403 riyazi-0.17/riyazi/fft/testing/scipy/backendcontrol/
+-rw-rw-rw-   0        0        0       30 2023-01-10 05:10:45.000000 riyazi-0.17/riyazi/fft/testing/scipy/backendcontrol/__init__.py
+-rw-rw-rw-   0        0        0      231 2023-01-10 05:10:15.000000 riyazi-0.17/riyazi/fft/testing/scipy/backendcontrol/_backendcontrol.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.556403 riyazi-0.17/riyazi/fft/testing/scipy/discrete_sc/
+-rw-rw-rw-   0        0        0       20 2023-01-10 04:31:18.000000 riyazi-0.17/riyazi/fft/testing/scipy/discrete_sc/__init__.py
+-rw-rw-rw-   0        0        0     1769 2022-11-26 04:11:34.000000 riyazi-0.17/riyazi/fft/testing/scipy/discrete_sc/_dsct.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.561833 riyazi-0.17/riyazi/fft/testing/scipy/fast_fourier_transormation/
+-rw-rw-rw-   0        0        0       20 2023-01-10 04:27:45.000000 riyazi-0.17/riyazi/fft/testing/scipy/fast_fourier_transormation/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-01-10 04:27:00.000000 riyazi-0.17/riyazi/fft/testing/scipy/fast_fourier_transormation/_ffts.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.563863 riyazi-0.17/riyazi/fft/testing/scipy/fast_hankeltrans/
+-rw-rw-rw-   0        0        0       19 2023-01-10 04:55:24.000000 riyazi-0.17/riyazi/fft/testing/scipy/fast_hankeltrans/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-01-10 04:54:52.000000 riyazi-0.17/riyazi/fft/testing/scipy/fast_hankeltrans/_fht.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.565864 riyazi-0.17/riyazi/fft/testing/scipy/helperfunction/
+-rw-rw-rw-   0        0        0       25 2023-01-10 04:57:39.000000 riyazi-0.17/riyazi/fft/testing/scipy/helperfunction/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-01-10 05:02:22.000000 riyazi-0.17/riyazi/fft/testing/scipy/helperfunction/_helperfun.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.567867 riyazi-0.17/riyazi/geometry/
+-rw-rw-rw-   0        0        0       44 2023-03-31 05:00:05.000000 riyazi-0.17/riyazi/geometry/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-03-29 10:39:06.000000 riyazi-0.17/riyazi/geometry/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.612003 riyazi-0.17/riyazi/geometry/three_dim/
+-rw-rw-rw-   0        0        0      234 2023-03-31 05:06:31.000000 riyazi-0.17/riyazi/geometry/three_dim/__init__.py
+-rw-rw-rw-   0        0        0      307 2022-09-28 15:11:48.000000 riyazi-0.17/riyazi/geometry/three_dim/acute.py
+-rw-rw-rw-   0        0        0       66 2022-09-08 07:08:27.000000 riyazi-0.17/riyazi/geometry/three_dim/cone.py
+-rw-rw-rw-   0        0        0       39 2023-03-31 05:03:57.000000 riyazi-0.17/riyazi/geometry/three_dim/cube.py
+-rw-rw-rw-   0        0        0      103 2022-09-08 07:41:08.000000 riyazi-0.17/riyazi/geometry/three_dim/cylinder.py
+-rw-rw-rw-   0        0        0       52 2023-03-31 05:04:07.000000 riyazi-0.17/riyazi/geometry/three_dim/pyramid.py
+-rw-rw-rw-   0        0        0       66 2022-09-08 06:53:41.000000 riyazi-0.17/riyazi/geometry/three_dim/rectangle_prism.py
+-rw-rw-rw-   0        0        0       97 2022-09-08 06:54:02.000000 riyazi-0.17/riyazi/geometry/three_dim/sphere.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.614004 riyazi-0.17/riyazi/geometry/three_dim/testing/
+-rw-rw-rw-   0        0        0        0 2022-09-09 05:49:46.000000 riyazi-0.17/riyazi/geometry/three_dim/testing/hemisphere.py
+-rw-rw-rw-   0        0        0        0 2022-09-09 05:49:31.000000 riyazi-0.17/riyazi/geometry/three_dim/testing/sphere.py
+-rw-rw-rw-   0        0        0      186 2022-09-08 06:54:29.000000 riyazi-0.17/riyazi/geometry/three_dim/triangle_prism.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.617000 riyazi-0.17/riyazi/geometry/two_dim/
+-rw-rw-rw-   0        0        0      910 2022-11-19 12:44:49.000000 riyazi-0.17/riyazi/geometry/two_dim/circle.py
+-rw-rw-rw-   0        0        0      239 2022-09-08 05:14:29.000000 riyazi-0.17/riyazi/geometry/two_dim/rectangle.py
+-rw-rw-rw-   0        0        0      863 2022-09-06 02:46:08.000000 riyazi-0.17/riyazi/geometry/two_dim/square.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.619002 riyazi-0.17/riyazi/geometry/two_dim/test/
+-rw-rw-rw-   0        0        0      100 2022-11-19 12:43:50.000000 riyazi-0.17/riyazi/geometry/two_dim/test/__int__.py
+-rw-rw-rw-   0        0        0     5576 2022-11-20 07:21:37.000000 riyazi-0.17/riyazi/geometry/two_dim/test/dim2.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.355918 riyazi-0.17/riyazi/integrate/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.355918 riyazi-0.17/riyazi/integrate/testing/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.622016 riyazi-0.17/riyazi/integrate/testing/scipy/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.625461 riyazi-0.17/riyazi/integrate/testing/scipy/_ivp/
+-rw-rw-rw-   0        0        0      161 2023-01-11 04:58:32.000000 riyazi-0.17/riyazi/integrate/testing/scipy/_ivp/ivp.py
+-rw-rw-rw-   0        0        0      172 2023-01-11 04:54:31.000000 riyazi-0.17/riyazi/integrate/testing/scipy/_quadture.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.628385 riyazi-0.17/riyazi/interpolate/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:42:10.000000 riyazi-0.17/riyazi/interpolate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.629871 riyazi-0.17/riyazi/interpolate/testing/
+-rw-rw-rw-   0        0        0      776 2023-01-11 05:11:35.000000 riyazi-0.17/riyazi/interpolate/testing/_interpolate.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.633067 riyazi-0.17/riyazi/linalg/
+-rw-rw-rw-   0        0        0     2287 2022-11-10 13:10:05.000000 riyazi-0.17/riyazi/linalg/Decompositions.py
+-rw-rw-rw-   0        0        0       52 2022-11-11 06:13:20.000000 riyazi-0.17/riyazi/linalg/__init__.py
+-rw-rw-rw-   0        0        0     5630 2023-03-31 05:10:51.000000 riyazi-0.17/riyazi/linalg/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.637565 riyazi-0.17/riyazi/linalg/testing/
+-rw-rw-rw-   0        0        0        0 2022-09-21 05:14:22.000000 riyazi-0.17/riyazi/linalg/testing/inv.py
+-rw-rw-rw-   0        0        0        0 2022-09-21 05:15:04.000000 riyazi-0.17/riyazi/linalg/testing/pinv.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.366037 riyazi-0.17/riyazi/linalg/testing/scipy/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.641248 riyazi-0.17/riyazi/linalg/testing/scipy/Basics/
+-rw-rw-rw-   0        0        0      682 2022-11-13 05:58:59.000000 riyazi-0.17/riyazi/linalg/testing/scipy/Basics/__basics.py
+-rw-rw-rw-   0        0        0       22 2022-11-13 05:39:49.000000 riyazi-0.17/riyazi/linalg/testing/scipy/Basics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.643268 riyazi-0.17/riyazi/linalg/testing/scipy/Decompositions/
+-rw-rw-rw-   0        0        0      300 2023-01-11 05:20:14.000000 riyazi-0.17/riyazi/linalg/testing/scipy/Decompositions/_decom.py
+-rw-rw-rw-   0        0        0        0 2022-09-21 05:15:23.000000 riyazi-0.17/riyazi/linalg/testing/solve.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.644248 riyazi-0.17/riyazi/math/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.646253 riyazi-0.17/riyazi/math/Research/
+-rw-rw-rw-   0        0        0       27 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/Research/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/Research/numbermath.py
+-rw-rw-rw-   0        0        0      167 2023-03-30 05:30:43.000000 riyazi-0.17/riyazi/math/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.649247 riyazi-0.17/riyazi/math/_logarithms/
+-rw-rw-rw-   0        0        0       43 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_logarithms/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_logarithms/_doc_log.py
+-rw-rw-rw-   0        0        0      587 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_logarithms/_log.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.650251 riyazi-0.17/riyazi/math/_logic/
+-rw-rw-rw-   0        0        0       22 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_logic/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_logic/_bitwise.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.657257 riyazi-0.17/riyazi/math/_numeric/
+-rw-rw-rw-   0        0        0       24 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_numeric/__init__.py
+-rw-rw-rw-   0        0        0     4659 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_numeric/basic.py
+-rw-rw-rw-   0        0        0    12641 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_numeric/doc_numerics.py
+-rw-rw-rw-   0        0        0    14096 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_numeric/numerics.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.661400 riyazi-0.17/riyazi/math/_sets/
+-rw-rw-rw-   0        0        0       18 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_sets/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_sets/doc_set.py
+-rw-rw-rw-   0        0        0     1054 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_sets/set.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.664401 riyazi-0.17/riyazi/math/_trigonometry/
+-rw-rw-rw-   0        0        0       46 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_trigonometry/__init__.py
+-rw-rw-rw-   0        0        0     3108 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_trigonometry/_trig.py
+-rw-rw-rw-   0        0        0    10884 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_trigonometry/doc_trig.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.665401 riyazi-0.17/riyazi/math/_trigonometry/legacy/
+-rw-rw-rw-   0        0        0       92 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_trigonometry/legacy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.666401 riyazi-0.17/riyazi/math/_trigonometry/tests/
+-rw-rw-rw-   0        0        0      571 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/_trigonometry/tests/complex.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.668400 riyazi-0.17/riyazi/math/mpmath/
+-rw-rw-rw-   0        0        0      235 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/mpmath/Exponential_integrals_and_error_functions.py
+-rw-rw-rw-   0        0        0      310 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/mpmath/Hypergeometric_function.py
+-rw-rw-rw-   0        0        0     2989 2023-02-02 12:38:49.000000 riyazi-0.17/riyazi/math/mpmath/power_and_logartihm.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.672620 riyazi-0.17/riyazi/matrix/
+-rw-rw-rw-   0        0        0       22 2022-11-10 07:36:37.000000 riyazi-0.17/riyazi/matrix/__init__.py
+-rw-rw-rw-   0        0        0     3674 2022-11-10 07:46:53.000000 riyazi-0.17/riyazi/matrix/matrices.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.675682 riyazi-0.17/riyazi/ndimage/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:44:01.000000 riyazi-0.17/riyazi/ndimage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.380943 riyazi-0.17/riyazi/numerical/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.381941 riyazi-0.17/riyazi/numerical/numerica/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.381941 riyazi-0.17/riyazi/numerical/numerica/differentiation/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.680680 riyazi-0.17/riyazi/numerical/numerica/differentiation/euler/
+-rw-rw-rw-   0        0        0        0 2021-03-01 10:53:17.000000 riyazi-0.17/riyazi/numerical/numerica/differentiation/euler/__init__.py
+-rw-rw-rw-   0        0        0      148 2021-03-01 10:53:17.000000 riyazi-0.17/riyazi/numerical/numerica/differentiation/euler/backward.py
+-rw-rw-rw-   0        0        0      147 2021-03-01 10:53:17.000000 riyazi-0.17/riyazi/numerical/numerica/differentiation/euler/forward.py
+-rw-rw-rw-   0        0        0      166 2021-03-01 10:53:17.000000 riyazi-0.17/riyazi/numerical/numerica/differentiation/euler/midpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.681679 riyazi-0.17/riyazi/odr/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:44:50.000000 riyazi-0.17/riyazi/odr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.682680 riyazi-0.17/riyazi/optimize/
+-rw-rw-rw-   0        0        0       25 2022-11-16 02:49:45.000000 riyazi-0.17/riyazi/optimize/__init__.py
+-rw-rw-rw-   0        0        0     1376 2022-11-16 02:49:28.000000 riyazi-0.17/riyazi/optimize/bisection.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.684682 riyazi-0.17/riyazi/physics/
+-rw-rw-rw-   0        0        0       25 2022-11-14 10:34:35.000000 riyazi-0.17/riyazi/physics/__basics.py
+-rw-rw-rw-   0        0        0       22 2022-11-14 08:48:15.000000 riyazi-0.17/riyazi/physics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.685681 riyazi-0.17/riyazi/physics/constants/
+-rw-rw-rw-   0        0        0      127 2022-11-17 05:27:15.000000 riyazi-0.17/riyazi/physics/constants/codata.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.695034 riyazi-0.17/riyazi/physics/electronics/
+-rw-rw-rw-   0        0        0      117 2022-11-14 10:34:09.000000 riyazi-0.17/riyazi/physics/electronics/__basics.py
+-rw-rw-rw-   0        0        0     2887 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/electronics/carrier_concentration.py
+-rw-rw-rw-   0        0        0     2713 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/electronics/coulombs_law.py
+-rw-rw-rw-   0        0        0     1973 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/electronics/electric_power.py
+-rw-rw-rw-   0        0        0     1459 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/electronics/ohms_law.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.701032 riyazi-0.17/riyazi/physics/quantum/
+-rw-rw-rw-   0        0        0        0 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/__init__.py
+-rw-rw-rw-   0        0        0     4428 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/deutsch_jozsa.py
+-rw-rw-rw-   0        0        0     1547 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/half_adder.py
+-rw-rw-rw-   0        0        0     1237 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/not_gate.py
+-rw-rw-rw-   0        0        0     1960 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/quantum_entanglement.py
+-rw-rw-rw-   0        0        0     3608 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/ripple_adder_classic.py
+-rw-rw-rw-   0        0        0     1076 2022-09-24 17:04:00.000000 riyazi-0.17/riyazi/physics/quantum/single_qubit_measure.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.704032 riyazi-0.17/riyazi/polynomial/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.709593 riyazi-0.17/riyazi/polynomial/HermiteE/
+-rw-rw-rw-   0        0        0       24 2023-04-05 06:59:31.000000 riyazi-0.17/riyazi/polynomial/HermiteE/__init__.py
+-rw-rw-rw-   0        0        0    18508 2023-04-05 07:02:08.000000 riyazi-0.17/riyazi/polynomial/HermiteE/_hermite_e.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.711590 riyazi-0.17/riyazi/polynomial/Laguerre/
+-rw-rw-rw-   0        0        0       23 2023-04-05 06:59:55.000000 riyazi-0.17/riyazi/polynomial/Laguerre/__init__.py
+-rw-rw-rw-   0        0        0    18084 2023-04-05 07:01:37.000000 riyazi-0.17/riyazi/polynomial/Laguerre/_laguerre.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.713589 riyazi-0.17/riyazi/polynomial/Legendre/
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:04:28.000000 riyazi-0.17/riyazi/polynomial/Legendre/__init__.py
+-rw-rw-rw-   0        0        0    18007 2023-04-05 07:01:21.000000 riyazi-0.17/riyazi/polynomial/Legendre/_legendre.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.715590 riyazi-0.17/riyazi/polynomial/Polynomial/
+-rw-rw-rw-   0        0        0       26 2023-04-05 07:00:49.000000 riyazi-0.17/riyazi/polynomial/Polynomial/__init__.py
+-rw-rw-rw-   0        0        0    18285 2023-04-05 07:08:24.000000 riyazi-0.17/riyazi/polynomial/Polynomial/_polynomial.py
+-rw-rw-rw-   0        0        0      139 2023-04-05 07:03:32.000000 riyazi-0.17/riyazi/polynomial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.717591 riyazi-0.17/riyazi/polynomial/chebyshev/
+-rw-rw-rw-   0        0        0       24 2023-04-04 06:19:41.000000 riyazi-0.17/riyazi/polynomial/chebyshev/__init__.py
+-rw-rw-rw-   0        0        0    23012 2023-04-04 05:50:51.000000 riyazi-0.17/riyazi/polynomial/chebyshev/_chebyshev.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.719590 riyazi-0.17/riyazi/polynomial/hermite/
+-rw-rw-rw-   0        0        0       21 2023-04-04 06:20:38.000000 riyazi-0.17/riyazi/polynomial/hermite/__init__.py
+-rw-rw-rw-   0        0        0    18704 2023-04-03 14:38:24.000000 riyazi-0.17/riyazi/polynomial/hermite/hermite.py
+-rw-rw-rw-   0        0        0    10226 2023-04-04 06:15:18.000000 riyazi-0.17/riyazi/polynomial/polyutils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.725616 riyazi-0.17/riyazi/polynomial/testing/
+-rw-rw-rw-   0        0        0       25 2022-09-16 10:33:59.000000 riyazi-0.17/riyazi/polynomial/testing/__init__.py
+-rw-rw-rw-   0        0        0      337 2022-11-26 12:55:29.000000 riyazi-0.17/riyazi/polynomial/testing/quadratic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.396943 riyazi-0.17/riyazi/scimath/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.727621 riyazi-0.17/riyazi/scimath/random/
+-rw-rw-rw-   0        0        0       22 2022-12-02 13:07:04.000000 riyazi-0.17/riyazi/scimath/random/random.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.728615 riyazi-0.17/riyazi/series/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:46:40.000000 riyazi-0.17/riyazi/series/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-03-31 04:55:10.000000 riyazi-0.17/riyazi/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.728615 riyazi-0.17/riyazi/signal/
+-rw-rw-rw-   0        0        0       30 2023-01-19 03:31:55.000000 riyazi-0.17/riyazi/signal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.729617 riyazi-0.17/riyazi/signal/testing/
+-rw-rw-rw-   0        0        0     1166 2023-03-31 05:12:04.000000 riyazi-0.17/riyazi/signal/testing/_signal.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.730616 riyazi-0.17/riyazi/sparse/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:47:34.000000 riyazi-0.17/riyazi/sparse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.731617 riyazi-0.17/riyazi/spatial/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:48:22.000000 riyazi-0.17/riyazi/spatial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.732615 riyazi-0.17/riyazi/special/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.401948 riyazi-0.17/riyazi/special/__funtions_mpmath__/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.733616 riyazi-0.17/riyazi/special/__funtions_mpmath__/calculus/
+-rw-rw-rw-   0        0        0       26 2023-02-03 09:30:06.000000 riyazi-0.17/riyazi/special/__funtions_mpmath__/calculus/_basic.py
+-rw-rw-rw-   0        0        0      828 2023-01-10 04:06:13.000000 riyazi-0.17/riyazi/special/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.417171 riyazi-0.17/riyazi/special/testing/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.735615 riyazi-0.17/riyazi/special/testing/Other_special_functions/
+-rw-rw-rw-   0        0        0       27 2023-01-09 06:25:53.000000 riyazi-0.17/riyazi/special/testing/Other_special_functions/__init__.py
+-rw-rw-rw-   0        0        0     2503 2023-01-09 06:29:11.000000 riyazi-0.17/riyazi/special/testing/Other_special_functions/otherspsfunc.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.738794 riyazi-0.17/riyazi/special/testing/airy/
+-rw-rw-rw-   0        0        0       19 2023-01-08 13:04:44.000000 riyazi-0.17/riyazi/special/testing/airy/__init__.py
+-rw-rw-rw-   0        0        0     1003 2022-12-31 12:42:17.000000 riyazi-0.17/riyazi/special/testing/airy/airy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.748780 riyazi-0.17/riyazi/special/testing/bessel/
+-rw-rw-rw-   0        0        0      152 2023-01-08 11:27:09.000000 riyazi-0.17/riyazi/special/testing/bessel/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-01-08 04:21:05.000000 riyazi-0.17/riyazi/special/testing/bessel/bessel_function.py
+-rw-rw-rw-   0        0        0      649 2023-01-08 11:17:22.000000 riyazi-0.17/riyazi/special/testing/bessel/common_bessel.py
+-rw-rw-rw-   0        0        0      548 2023-01-08 11:26:39.000000 riyazi-0.17/riyazi/special/testing/bessel/drivative_bessel.py
+-rw-rw-rw-   0        0        0      218 2023-01-08 12:50:25.000000 riyazi-0.17/riyazi/special/testing/bessel/integralbessel.py
+-rw-rw-rw-   0        0        0      311 2023-01-08 05:27:01.000000 riyazi-0.17/riyazi/special/testing/bessel/riccati_bessel.py
+-rw-rw-rw-   0        0        0      725 2023-01-08 05:54:46.000000 riyazi-0.17/riyazi/special/testing/bessel/sphe_bessel.py
+-rw-rw-rw-   0        0        0      128 2023-01-01 07:34:08.000000 riyazi-0.17/riyazi/special/testing/bessel/zerosbessel.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.750780 riyazi-0.17/riyazi/special/testing/combinatorics/
+-rw-rw-rw-   0        0        0       28 2023-01-09 12:22:25.000000 riyazi-0.17/riyazi/special/testing/combinatorics/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-01-09 12:21:41.000000 riyazi-0.17/riyazi/special/testing/combinatorics/combinatorics.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.755787 riyazi-0.17/riyazi/special/testing/convenience/
+-rw-rw-rw-   0        0        0       56 2023-01-09 06:21:57.000000 riyazi-0.17/riyazi/special/testing/convenience/__init__.py
+-rw-rw-rw-   0        0        0     1546 2022-12-30 16:02:54.000000 riyazi-0.17/riyazi/special/testing/convenience/convenience.py
+-rw-rw-rw-   0        0        0     5427 2023-01-09 06:21:18.000000 riyazi-0.17/riyazi/special/testing/convenience/doc_convenience.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.759050 riyazi-0.17/riyazi/special/testing/ellipintegral/
+-rw-rw-rw-   0        0        0      133 2023-01-01 07:27:39.000000 riyazi-0.17/riyazi/special/testing/ellipintegral/ellipintegral.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.407946 riyazi-0.17/riyazi/special/testing/errorintegral/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.762293 riyazi-0.17/riyazi/special/testing/errorintegral/testing/
+-rw-rw-rw-   0        0        0       36 2023-01-09 05:47:32.000000 riyazi-0.17/riyazi/special/testing/errorintegral/testing/__init__.py
+-rw-rw-rw-   0        0        0      866 2023-01-09 05:44:30.000000 riyazi-0.17/riyazi/special/testing/errorintegral/testing/error_frasnelintegral.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.764295 riyazi-0.17/riyazi/special/testing/gammarelt/
+-rw-rw-rw-   0        0        0       27 2023-01-09 05:48:19.000000 riyazi-0.17/riyazi/special/testing/gammarelt/__init__.py
+-rw-rw-rw-   0        0        0     1037 2023-01-09 05:36:53.000000 riyazi-0.17/riyazi/special/testing/gammarelt/gamma_related.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.766295 riyazi-0.17/riyazi/special/testing/hypergeometric/
+-rw-rw-rw-   0        0        0       25 2023-01-10 03:32:13.000000 riyazi-0.17/riyazi/special/testing/hypergeometric/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-01-10 03:14:59.000000 riyazi-0.17/riyazi/special/testing/hypergeometric/_hypergeom.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.768294 riyazi-0.17/riyazi/special/testing/infotheory/
+-rw-rw-rw-   0        0        0       23 2023-01-09 05:24:42.000000 riyazi-0.17/riyazi/special/testing/infotheory/__init__.py
+-rw-rw-rw-   0        0        0      831 2023-01-09 05:33:16.000000 riyazi-0.17/riyazi/special/testing/infotheory/infothry.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.772304 riyazi-0.17/riyazi/special/testing/kelvin/
+-rw-rw-rw-   0        0        0       21 2023-01-10 03:41:32.000000 riyazi-0.17/riyazi/special/testing/kelvin/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-01-10 03:48:16.000000 riyazi-0.17/riyazi/special/testing/kelvin/_kelvin.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.776677 riyazi-0.17/riyazi/special/testing/lambertwrelt/
+-rw-rw-rw-   0        0        0       30 2023-01-09 12:56:54.000000 riyazi-0.17/riyazi/special/testing/lambertwrelt/__init__.py
+-rw-rw-rw-   0        0        0      879 2023-01-09 12:56:23.000000 riyazi-0.17/riyazi/special/testing/lambertwrelt/lambert_related.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.779676 riyazi-0.17/riyazi/special/testing/legendre/
+-rw-rw-rw-   0        0        0       23 2023-01-09 05:52:23.000000 riyazi-0.17/riyazi/special/testing/legendre/__init__.py
+-rw-rw-rw-   0        0        0      693 2023-01-01 05:50:35.000000 riyazi-0.17/riyazi/special/testing/legendre/legendre.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.781676 riyazi-0.17/riyazi/special/testing/mathieu_related/
+-rw-rw-rw-   0        0        0       23 2023-01-10 04:01:30.000000 riyazi-0.17/riyazi/special/testing/mathieu_related/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-01-10 04:00:30.000000 riyazi-0.17/riyazi/special/testing/mathieu_related/_mathieu.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.783676 riyazi-0.17/riyazi/special/testing/parabolic_cylinder/
+-rw-rw-rw-   0        0        0       24 2023-01-10 03:19:15.000000 riyazi-0.17/riyazi/special/testing/parabolic_cylinder/__init__.py
+-rw-rw-rw-   0        0        0      233 2023-01-10 03:27:48.000000 riyazi-0.17/riyazi/special/testing/parabolic_cylinder/pbcylinder.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.785677 riyazi-0.17/riyazi/special/testing/raw_statistical/
+-rw-rw-rw-   0        0        0       22 2023-01-09 05:18:51.000000 riyazi-0.17/riyazi/special/testing/raw_statistical/__init__.py
+-rw-rw-rw-   0        0        0     1526 2023-01-09 05:21:41.000000 riyazi-0.17/riyazi/special/testing/raw_statistical/rwstats.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.789909 riyazi-0.17/riyazi/special/testing/spheroidal_wave/
+-rw-rw-rw-   0        0        0       27 2023-01-10 04:05:45.000000 riyazi-0.17/riyazi/special/testing/spheroidal_wave/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-01-10 04:04:44.000000 riyazi-0.17/riyazi/special/testing/spheroidal_wave/_spheroidwav.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.793278 riyazi-0.17/riyazi/special/testing/struve/
+-rw-rw-rw-   0        0        0       30 2023-01-09 05:08:52.000000 riyazi-0.17/riyazi/special/testing/struve/__init__.py
+-rw-rw-rw-   0        0        0      545 2023-01-09 05:08:14.000000 riyazi-0.17/riyazi/special/testing/struve/struve_function.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.796278 riyazi-0.17/riyazi/stats/
+-rw-rw-rw-   0        0        0       21 2023-01-13 05:04:31.000000 riyazi-0.17/riyazi/stats/__init__.py
+-rw-rw-rw-   0        0        0     6444 2022-11-08 13:11:13.000000 riyazi-0.17/riyazi/stats/_basics.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.419165 riyazi-0.17/riyazi/stats/probability/
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.797277 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/
+-rw-rw-rw-   0        0        0        0 2023-01-13 04:43:14.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-01-13 04:44:55.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/ddf.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.802301 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/
+-rw-rw-rw-   0        0        0        0 2022-11-12 01:45:27.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/Benfords_distribution.py
+-rw-rw-rw-   0        0        0     1531 2022-11-11 13:34:44.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/Bernoulli_distributions.py
+-rw-rw-rw-   0        0        0      508 2022-11-10 01:21:05.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/Binomial_distributions.py
+-rw-rw-rw-   0        0        0        0 2022-11-12 01:45:53.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/Poisson_binomial.py
+-rw-rw-rw-   0        0        0       76 2022-11-09 03:15:54.000000 riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.810606 riyazi-0.17/riyazi/stats/testing/
+-rw-rw-rw-   0        0        0       55 2022-09-15 05:52:23.000000 riyazi-0.17/riyazi/stats/testing/__init__.py
+-rw-rw-rw-   0        0        0      246 2022-09-15 06:00:04.000000 riyazi-0.17/riyazi/stats/testing/combination.py
+-rw-rw-rw-   0        0        0     1183 2022-09-22 06:58:57.000000 riyazi-0.17/riyazi/stats/testing/percentile .py
+-rw-rw-rw-   0        0        0      199 2022-09-15 05:57:50.000000 riyazi-0.17/riyazi/stats/testing/permutation.py
+-rw-rw-rw-   0        0        0      193 2023-04-18 06:44:16.000000 riyazi-0.17/riyazi/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:45:11.481959 riyazi-0.17/riyazi.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-04-18 06:45:10.000000 riyazi-0.17/riyazi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8762 2023-04-18 06:45:11.000000 riyazi-0.17/riyazi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:45:10.000000 riyazi-0.17/riyazi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 06:45:10.000000 riyazi-0.17/riyazi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:45:11.812605 riyazi-0.17/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-18 06:43:54.000000 riyazi-0.17/setup.py
```

### Comparing `riyazi-0.16/LICENSE` & `riyazi-0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/Module/main.py` & `riyazi-0.17/riyazi/Module/main.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/Module/mymodule.py` & `riyazi-0.17/riyazi/Module/mymodule.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/Module/numeric.py` & `riyazi-0.17/riyazi/Module/numeric.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/__init__.py` & `riyazi-0.17/riyazi/__init__.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/algebra/_factor.py` & `riyazi-0.17/riyazi/algebra/_factor.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/algebra/_product.py` & `riyazi-0.17/riyazi/algebra/_product.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/Strings/mmu.py` & `riyazi-0.17/riyazi/constants/Strings/mmu.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/__init__.py` & `riyazi-0.17/riyazi/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/codatamath.py` & `riyazi-0.17/riyazi/constants/codatamath.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/codatamath_function.py` & `riyazi-0.17/riyazi/constants/codatamath_function.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/codataphy.py` & `riyazi-0.17/riyazi/constants/codataphy.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/testing/__init__.py` & `riyazi-0.17/riyazi/constants/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/testing/codatamath.py` & `riyazi-0.17/riyazi/constants/testing/codatamath.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/testing/math.py` & `riyazi-0.17/riyazi/constants/testing/math.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/constants/testing/physics.py` & `riyazi-0.17/riyazi/constants/testing/physics.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/basic.py` & `riyazi-0.17/riyazi/crypto/basic.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/adler32.py` & `riyazi-0.17/riyazi/crypto/hashes/adler32.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/chaos_machine.py` & `riyazi-0.17/riyazi/crypto/hashes/chaos_machine.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/djb2.py` & `riyazi-0.17/riyazi/crypto/hashes/djb2.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/enigma_machine.py` & `riyazi-0.17/riyazi/crypto/hashes/enigma_machine.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/hamming_code.py` & `riyazi-0.17/riyazi/crypto/hashes/hamming_code.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/luhn.py` & `riyazi-0.17/riyazi/crypto/hashes/luhn.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/md5.py` & `riyazi-0.17/riyazi/crypto/hashes/md5.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/sdbm.py` & `riyazi-0.17/riyazi/crypto/hashes/sdbm.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/sha1.py` & `riyazi-0.17/riyazi/crypto/hashes/sha1.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/hashes/sha256.py` & `riyazi-0.17/riyazi/crypto/hashes/sha256.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/crypto/setup.py` & `riyazi-0.17/riyazi/crypto/setup.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/fft/Generaldistribution.py` & `riyazi-0.17/riyazi/fft/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/fft/setup.py` & `riyazi-0.17/riyazi/fft/setup.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/fft/testing/scipy/discrete_sc/_dsct.py` & `riyazi-0.17/riyazi/fft/testing/scipy/discrete_sc/_dsct.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/fft/testing/scipy/fast_fourier_transormation/_ffts.py` & `riyazi-0.17/riyazi/fft/testing/scipy/fast_fourier_transormation/_ffts.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/geometry/setup.py` & `riyazi-0.17/riyazi/geometry/setup.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/geometry/two_dim/circle.py` & `riyazi-0.17/riyazi/geometry/two_dim/circle.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/geometry/two_dim/square.py` & `riyazi-0.17/riyazi/geometry/two_dim/square.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/geometry/two_dim/test/dim2.py` & `riyazi-0.17/riyazi/geometry/two_dim/test/dim2.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/interpolate/testing/_interpolate.py` & `riyazi-0.17/riyazi/interpolate/testing/_interpolate.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/linalg/Decompositions.py` & `riyazi-0.17/riyazi/linalg/Decompositions.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/linalg/basic.py` & `riyazi-0.17/riyazi/linalg/basic.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/linalg/testing/scipy/Basics/__basics.py` & `riyazi-0.17/riyazi/linalg/testing/scipy/Basics/__basics.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_logarithms/_doc_log.py` & `riyazi-0.17/riyazi/math/_logarithms/_doc_log.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_logarithms/_log.py` & `riyazi-0.17/riyazi/math/_logarithms/_log.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_numeric/basic.py` & `riyazi-0.17/riyazi/math/_numeric/basic.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_numeric/doc_numerics.py` & `riyazi-0.17/riyazi/math/_numeric/doc_numerics.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_numeric/numerics.py` & `riyazi-0.17/riyazi/math/_numeric/numerics.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_sets/doc_set.py` & `riyazi-0.17/riyazi/math/_sets/doc_set.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_sets/set.py` & `riyazi-0.17/riyazi/math/_sets/set.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_trigonometry/_trig.py` & `riyazi-0.17/riyazi/math/_trigonometry/_trig.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_trigonometry/doc_trig.py` & `riyazi-0.17/riyazi/math/_trigonometry/doc_trig.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/_trigonometry/tests/complex.py` & `riyazi-0.17/riyazi/math/_trigonometry/tests/complex.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/math/mpmath/power_and_logartihm.py` & `riyazi-0.17/riyazi/math/mpmath/power_and_logartihm.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/matrix/matrices.py` & `riyazi-0.17/riyazi/matrix/matrices.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/optimize/bisection.py` & `riyazi-0.17/riyazi/optimize/bisection.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/electronics/carrier_concentration.py` & `riyazi-0.17/riyazi/physics/electronics/carrier_concentration.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/electronics/coulombs_law.py` & `riyazi-0.17/riyazi/physics/electronics/coulombs_law.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/electronics/electric_power.py` & `riyazi-0.17/riyazi/physics/electronics/electric_power.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/electronics/ohms_law.py` & `riyazi-0.17/riyazi/physics/electronics/ohms_law.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/deutsch_jozsa.py` & `riyazi-0.17/riyazi/physics/quantum/deutsch_jozsa.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/half_adder.py` & `riyazi-0.17/riyazi/physics/quantum/half_adder.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/not_gate.py` & `riyazi-0.17/riyazi/physics/quantum/not_gate.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/quantum_entanglement.py` & `riyazi-0.17/riyazi/physics/quantum/quantum_entanglement.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/ripple_adder_classic.py` & `riyazi-0.17/riyazi/physics/quantum/ripple_adder_classic.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/physics/quantum/single_qubit_measure.py` & `riyazi-0.17/riyazi/physics/quantum/single_qubit_measure.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/HermiteE/_hermite_e.py` & `riyazi-0.17/riyazi/polynomial/HermiteE/_hermite_e.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/Laguerre/_laguerre.py` & `riyazi-0.17/riyazi/polynomial/Laguerre/_laguerre.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/Legendre/_legendre.py` & `riyazi-0.17/riyazi/polynomial/Legendre/_legendre.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/Polynomial/_polynomial.py` & `riyazi-0.17/riyazi/polynomial/Polynomial/_polynomial.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/chebyshev/_chebyshev.py` & `riyazi-0.17/riyazi/polynomial/chebyshev/_chebyshev.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/hermite/hermite.py` & `riyazi-0.17/riyazi/polynomial/hermite/hermite.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/polynomial/polyutils.py` & `riyazi-0.17/riyazi/polynomial/polyutils.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/setup.py` & `riyazi-0.17/riyazi/setup.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/signal/testing/_signal.py` & `riyazi-0.17/riyazi/signal/testing/_signal.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/__init__.py` & `riyazi-0.17/riyazi/special/__init__.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/Other_special_functions/otherspsfunc.py` & `riyazi-0.17/riyazi/special/testing/Other_special_functions/otherspsfunc.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/airy/airy.py` & `riyazi-0.17/riyazi/special/testing/airy/airy.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/bessel/bessel_function.py` & `riyazi-0.17/riyazi/special/testing/bessel/bessel_function.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/bessel/common_bessel.py` & `riyazi-0.17/riyazi/special/testing/bessel/common_bessel.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/bessel/drivative_bessel.py` & `riyazi-0.17/riyazi/special/testing/bessel/drivative_bessel.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/bessel/sphe_bessel.py` & `riyazi-0.17/riyazi/special/testing/bessel/sphe_bessel.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/convenience/convenience.py` & `riyazi-0.17/riyazi/special/testing/convenience/convenience.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/convenience/doc_convenience.py` & `riyazi-0.17/riyazi/special/testing/convenience/doc_convenience.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/errorintegral/testing/error_frasnelintegral.py` & `riyazi-0.17/riyazi/special/testing/errorintegral/testing/error_frasnelintegral.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/gammarelt/gamma_related.py` & `riyazi-0.17/riyazi/special/testing/gammarelt/gamma_related.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/infotheory/infothry.py` & `riyazi-0.17/riyazi/special/testing/infotheory/infothry.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/kelvin/_kelvin.py` & `riyazi-0.17/riyazi/special/testing/kelvin/_kelvin.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/lambertwrelt/lambert_related.py` & `riyazi-0.17/riyazi/special/testing/lambertwrelt/lambert_related.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/legendre/legendre.py` & `riyazi-0.17/riyazi/special/testing/legendre/legendre.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/mathieu_related/_mathieu.py` & `riyazi-0.17/riyazi/special/testing/mathieu_related/_mathieu.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/raw_statistical/rwstats.py` & `riyazi-0.17/riyazi/special/testing/raw_statistical/rwstats.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/special/testing/struve/struve_function.py` & `riyazi-0.17/riyazi/special/testing/struve/struve_function.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/stats/_basics.py` & `riyazi-0.17/riyazi/stats/_basics.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/stats/probability/Discrete_distributions/finite/Bernoulli_distributions.py` & `riyazi-0.17/riyazi/stats/probability/Discrete_distributions/finite/Bernoulli_distributions.py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi/stats/testing/percentile .py` & `riyazi-0.17/riyazi/stats/testing/percentile .py`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/riyazi.egg-info/SOURCES.txt` & `riyazi-0.17/riyazi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riyazi-0.16/setup.py` & `riyazi-0.17/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
 
 name='riyazi',
 
-version = '0.16'
+version = '0.17'
 
 )
 
 
 with open('README.md', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
```

