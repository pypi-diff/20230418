# Comparing `tmp/repairwheel-0.2.0.tar.gz` & `tmp/repairwheel-0.2.1.tar.gz`

## Comparing `repairwheel-0.2.0.tar` & `repairwheel-0.2.1.tar`

### file list

```diff
@@ -1,121 +1,113 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.0/codecov.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/__main__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/compat.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/fileutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/py.typed
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/repair.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel.pyi
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel.pyi
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/vendor.txt
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/LICENSE
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/__main__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/condatools.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/elfutils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/error.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/hashfile.py
--rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/lddtree.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/libc.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_addtag.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_lddtree.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_repair.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_show.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/musllinux.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/patcher.py
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/repair.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/tmpdirs.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/tools.py
--rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/wheel_abi.py
--rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/__init__.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/external_references.py
--rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/LICENSE
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/_version.py
--rw-r--r--   0        0        0    33149 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/delocating.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/fuse.py
--rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/libsana.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/pkginfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/py.typed
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/tmpdirs.py
--rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/tools.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/__init__.py
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/__init__.py
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/__main__.py
--rw-r--r--   0        0        0   132622 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/_dll_list.py
--rw-r--r--   0        0        0    32249 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/_dll_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/_version.py
--rw-r--r--   0        0        0    40112 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/_wheel_repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/linux/__init__.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/linux/elffile.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/linux/monkeypatch.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/linux/patcher.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/linux/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/macos/__init__.py
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/macos/machosign.py
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/macos/machotools.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/macos/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/windows/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 repairwheel-0.2.0/src/repairwheel/windows/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/test_common.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/test_windows.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/gen_check/__init__.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/gen_check/test_check.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/gen_check/test_generate.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-native/README.md
--rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-native/build.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-native/testwheel.c
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-native/testdep/testdep.c
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-native/testdep/testdep.h
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-python/build.sh
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-python/pyproject.toml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-python/testwheel/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/build-python/testwheel/testwheel.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
--rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
--rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
--rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tools/vendoring/patches/auditwheel.patch
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.0/tools/vendoring/patches/delocate.patch
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.0/LICENSE
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repairwheel-0.2.0/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 repairwheel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 repairwheel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.1/CHANGELOG.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.1/codecov.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/__main__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/compat.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/fileutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/py.typed
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/repair.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel.pyi
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/vendor.txt
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/LICENSE
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/__main__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/condatools.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/elfutils.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/error.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/hashfile.py
+-rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/lddtree.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/libc.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_addtag.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_lddtree.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_repair.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_show.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/musllinux.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/patcher.py
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/repair.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/tmpdirs.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/tools.py
+-rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/wheel_abi.py
+-rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/__init__.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/external_references.py
+-rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/LICENSE
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/_version.py
+-rw-r--r--   0        0        0    33149 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/delocating.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/fuse.py
+-rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/libsana.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/pkginfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/py.typed
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/tmpdirs.py
+-rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/tools.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/__init__.py
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/linux/__init__.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/linux/elffile.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/linux/monkeypatch.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/linux/patcher.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/linux/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/macos/__init__.py
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/macos/machosign.py
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/macos/machotools.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/macos/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/windows/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 repairwheel-0.2.1/src/repairwheel/windows/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/test_common.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/test_windows.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/gen_check/__init__.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/gen_check/test_check.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/gen_check/test_generate.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-native/README.md
+-rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-native/build.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-native/testwheel.c
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-native/testdep/testdep.c
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-native/testdep/testdep.h
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-python/build.sh
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-python/pyproject.toml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-python/testwheel/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/build-python/testwheel/testwheel.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
+-rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
+-rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tools/vendoring/patches/auditwheel.patch
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.1/tools/vendoring/patches/delocate.patch
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 repairwheel-0.2.1/README.md
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 repairwheel-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 repairwheel-0.2.1/PKG-INFO
```

### Comparing `repairwheel-0.2.0/src/repairwheel/compat.py` & `repairwheel-0.2.1/src/repairwheel/compat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/fileutil.py` & `repairwheel-0.2.1/src/repairwheel/fileutil.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/repair.py` & `repairwheel-0.2.1/src/repairwheel/repair.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import argparse
+import datetime
+import os
 import shutil
 import sys
 import tempfile
 from pathlib import Path
 from typing import List, NoReturn, Set
 
 from packaging.utils import parse_wheel_filename
@@ -59,14 +61,23 @@
     shutil.copyfile(wheel, copied_location)
 
 
 def main():
     parser = make_parser()
     args = parser.parse_args()
 
+    if "SOURCE_DATE_EPOCH" in os.environ:
+        try:
+            epoch = int(os.environ["SOURCE_DATE_EPOCH"])
+            mtime = datetime.datetime.utcfromtimestamp(epoch)
+        except ValueError:
+            fatal(f"SOURCE_DATE_EPOCH value cannot be parsed as a number: {os.environ['SOURCE_DATE_EPOCH']}")
+    else:
+        mtime = None
+
     original_wheel: Path = args.wheel.resolve()
     out_dir: Path = args.output_dir.resolve()
     lib_path: List[Path] = [lp.resolve() for lp in (args.lib_dir or [])]
 
     if not original_wheel.is_file():
         fatal(f"File does not exist: {original_wheel}")
 
@@ -88,14 +99,14 @@
 
     with tempfile.TemporaryDirectory(prefix="repairwheel") as temp_wheel_dir:
         temp_wheel_dir = Path(temp_wheel_dir)
         fn(original_wheel, temp_wheel_dir, lib_path)
         patched_wheel = find_written_wheel(temp_wheel_dir)
 
         out_dir.mkdir(parents=True, exist_ok=True)
-        out_wheel = write_canonical_wheel(original_wheel, patched_wheel, out_dir)
+        out_wheel = write_canonical_wheel(original_wheel, patched_wheel, out_dir, mtime=mtime)
 
     print("Wrote", out_wheel)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `repairwheel-0.2.0/src/repairwheel/wheel.py` & `repairwheel-0.2.1/src/repairwheel/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import hashlib
 import operator
 import os
 import zipfile
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
-from typing import BinaryIO, List, Tuple
+from typing import BinaryIO, List, Optional, Tuple
 from zipfile import ZipFile, ZipInfo
 
 from packaging.utils import parse_wheel_filename
 
 
 DEFAULT_MTIME = datetime.fromisoformat("1980-01-01T00:00:00")
 # Taken from shutil in 3.8+
@@ -23,15 +23,14 @@
     # Filters out the RECORD and DELVEWHEEL files.
     wheel_name = Path(file.filename).name
     dist_name, dist_version, _, _ = parse_wheel_filename(wheel_name)
     dist_info_prefix = f"{dist_name}-{dist_version}.dist-info/"
 
     skip_files = {
         f"{dist_info_prefix}RECORD",  # Skip the record file; we'll write our own.
-        f"{dist_info_prefix}DELVEWHEEL",  # This file contains non-reproducible text.
     }
 
     dist_info_infos = []
     other_infos = []
     for info in file.infolist():
         if info.filename in skip_files:
             continue
@@ -65,26 +64,29 @@
 
 def write_canonical_wheel(
     original_wheel: Path,
     patched_wheel: Path,
     out_dir: Path,
     default_file_mode: int = 0o664,
     default_dir_mode: int = 0o775,
-    mtime: datetime = DEFAULT_MTIME,
+    mtime: Optional[datetime] = None,
     compression: int = zipfile.ZIP_DEFLATED,
 ) -> Path:
     """This function rewrites a wheel in a canonical form.
 
     * File and directory entries are lexicographically ordered
     * File data is written in the same order as corresponding names
     * All timestamps are set to a constant value
 
     Because Windows doesn't support posix file modes, we use corresponding modes in the original file if they exist.
     Else we use the default mode.
     """
+    if mtime is None:
+        mtime = DEFAULT_MTIME
+
     out_wheel = out_dir / patched_wheel.name
     dist_name, dist_version, _, _ = parse_wheel_filename(patched_wheel.name)
 
     with ZipFile(original_wheel) as original_wheel_zip:
         original_modes = {zi.filename: (zi.external_attr >> 16) & 0xFFFF for zi in original_wheel_zip.infolist()}
 
     mtime_args = mtime.timetuple()[:6]
```

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/LICENSE` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/LICENSE.txt` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/condatools.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/condatools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/elfutils.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/elfutils.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/genericpkgctx.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/genericpkgctx.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/lddtree.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/lddtree.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_addtag.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_addtag.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_repair.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/main_show.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/main_show.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/musllinux.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/musllinux.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/patcher.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/patcher.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/repair.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/tmpdirs.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/tools.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/tools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/wheel_abi.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/wheel_abi.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/wheeltools.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/wheeltools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/__init__.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/external_references.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/external_references.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/LICENSE` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/delocating.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/delocating.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/fuse.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/libsana.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/libsana.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/pkginfo.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/tmpdirs.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/tools.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/tools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/wheeltools.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/wheeltools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_path.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_path.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py` & `repairwheel-0.2.1/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/_vendor/delvewheel/LICENSE` & `repairwheel-0.2.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Copyright (c) 2020 Aohan Dang
+Copyright © 2023 Jeremy Volkman
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice (including the next
+paragraph) shall be included in all copies or substantial portions of the
+Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `repairwheel-0.2.0/src/repairwheel/linux/elffile.py` & `repairwheel-0.2.1/src/repairwheel/linux/elffile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/linux/monkeypatch.py` & `repairwheel-0.2.1/src/repairwheel/linux/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/linux/patcher.py` & `repairwheel-0.2.1/src/repairwheel/linux/patcher.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/linux/repair.py` & `repairwheel-0.2.1/src/repairwheel/linux/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/macos/machosign.py` & `repairwheel-0.2.1/src/repairwheel/macos/machosign.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/macos/machotools.py` & `repairwheel-0.2.1/src/repairwheel/macos/machotools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/src/repairwheel/macos/repair.py` & `repairwheel-0.2.1/src/repairwheel/macos/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/test_windows.py` & `repairwheel-0.2.1/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/gen_check/test_check.py` & `repairwheel-0.2.1/tests/gen_check/test_check.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/build-native/build.py` & `repairwheel-0.2.1/tests/testwheel/build-native/build.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/build-native/testwheel.c` & `repairwheel-0.2.1/tests/testwheel/build-native/testwheel.c`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll` & `repairwheel-0.2.1/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl` & `repairwheel-0.2.1/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tools/vendoring/patches/auditwheel.patch` & `repairwheel-0.2.1/tools/vendoring/patches/auditwheel.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/tools/vendoring/patches/delocate.patch` & `repairwheel-0.2.1/tools/vendoring/patches/delocate.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.0/pyproject.toml` & `repairwheel-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repairwheel"
-version = "0.2.0"
+version = "0.2.1"
 description = "Repair any wheel, anywhere"
 readme = "README.md"
 requires-python = ">= 3.7"
 license.file = "LICENSE"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
@@ -20,14 +20,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 urls.homepage = "https://github.com/jvolkman/repairwheel"
 
 dependencies = [
+  "delvewheel >= 1.3.6",
   "importlib_metadata; python_version < \"3.8\"",
   "macholib >= 1.16",
   "packaging >= 20.9",
   "pyelftools >= 0.24",
   "pefile >= 2023.2.7",  # for delvewheel
 ]
```

### Comparing `repairwheel-0.2.0/PKG-INFO` & `repairwheel-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repairwheel
-Version: 0.2.0
+Version: 0.2.1
 Summary: Repair any wheel, anywhere
 Project-URL: homepage, https://github.com/jvolkman/repairwheel
 License: Copyright © 2023 Jeremy Volkman
         
         Permission is hereby granted, free of charge, to any person obtaining a
         copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
@@ -31,29 +31,43 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: delvewheel>=1.3.6
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: macholib>=1.16
 Requires-Dist: packaging>=20.9
 Requires-Dist: pefile>=2023.2.7
 Requires-Dist: pyelftools>=0.24
 Description-Content-Type: text/markdown
 
 # repairwheel
 
 [![CI - Test](https://github.com/jvolkman/repairwheel/actions/workflows/test.yml/badge.svg)](https://github.com/jvolkman/repairwheel/actions/workflows/test.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/repairwheel.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/repairwheel/)
 
-</div>
+## Overview
 
-This project aims to be a combination of `auditwheel`, `delocate`, and `delvewheel` written in pure Python and able to run cross-platform.
+- `repairwheel` combines the "repair" steps from [`auditwheel`](https://github.com/pypa/auditwheel), [`delocate`](https://github.com/matthew-brett/delocate),
+  and [`delvewheel`](https://github.com/adang1345/delvewheel) into a single tool, enabling cross-platform wheel repair.
+- It includes pure-python replacements for external tools like `patchelf`, `otool`, `install_name_tool`, and `codesign`, so no non-python dependencies are required.
+
+## What's it do?
+
+1. When invoked, `repairwheel` first looks at the platform tag on the input wheel.
+2. Based on the tag, `repairwheel` selects a repair step from `auditwheel`, `delocate`, or `delvewheel` (or nothing, if it's a pure-Python wheel)
+3. Finally, `repairwheel` rewrites the result in a canonical form ensuring that:
+   1. File timestamps are set to a constant value;
+   2. Files in the archive are ordered lexicographically; and
+   3. Files in `RECORD` are ordered lexicographically
+
+The final result _should_ be bitwise-identitcal regardless of the system used to perform the repair.
 
 ## Usage
 
 ```
 usage: repairwheel [-h] -o OUTPUT_DIR [-l LIB_DIR] wheel
 
 positional arguments:
```

