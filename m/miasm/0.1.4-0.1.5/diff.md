# Comparing `tmp/miasm-0.1.4.tar.gz` & `tmp/miasm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miasm-0.1.4.tar", last modified: Wed Apr  5 21:33:44 2023, max compression
+gzip compressed data, was "miasm-0.1.5.tar", last modified: Tue Apr 18 21:27:11 2023, max compression
```

## Comparing `miasm-0.1.4.tar` & `miasm-0.1.5.tar`

### file list

```diff
@@ -1,221 +1,226 @@
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.163348 miasm-0.1.4/
--rw-r--r--   0 serpilliere  (1000) users      (985)    18092 2020-07-23 05:24:48.000000 miasm-0.1.4/LICENSE
--rw-r--r--   0 serpilliere  (1000) users      (985)    22076 2023-04-05 21:33:44.163348 miasm-0.1.4/PKG-INFO
--rw-r--r--   0 serpilliere  (1000) users      (985)    21508 2023-04-04 15:51:10.000000 miasm-0.1.4/README.md
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.060014 miasm-0.1.4/miasm/
--rw-r--r--   0 serpilliere  (1000) users      (985)        5 2023-04-05 21:33:43.000000 miasm-0.1.4/miasm/VERSION
--rw-r--r--   0 serpilliere  (1000) users      (985)     2732 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/__init__.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.066681 miasm-0.1.4/miasm/analysis/
--rw-r--r--   0 serpilliere  (1000) users      (985)       39 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/analysis/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     8209 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/analysis/apiset.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     7462 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/binary.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6170 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/cst_propag.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6829 2021-10-29 18:28:04.000000 miasm-0.1.4/miasm/analysis/data_analysis.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    79542 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/data_flow.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    16691 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/debugging.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    22278 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/depgraph.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3978 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/disasm_cb.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    29010 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/dse.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2653 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/analysis/expression_range.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    14342 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/gdbserver.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    10602 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/analysis/machine.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    19291 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/modularintervals.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    16079 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/outofssa.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    33866 2021-10-29 18:28:04.000000 miasm-0.1.4/miasm/analysis/sandbox.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     9574 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/simplifier.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    24132 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/analysis/ssa.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.066681 miasm-0.1.4/miasm/arch/
--rw-r--r--   0 serpilliere  (1000) users      (985)       31 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/__init__.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.066681 miasm-0.1.4/miasm/arch/aarch64/
--rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/aarch64/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    84898 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/aarch64/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      731 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/aarch64/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2536 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/aarch64/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1244 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/aarch64/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    10375 2021-10-29 18:28:04.000000 miasm-0.1.4/miasm/arch/aarch64/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    63189 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/aarch64/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.070014 miasm-0.1.4/miasm/arch/arm/
--rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/arm/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)   107077 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/arm/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1690 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/arm/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4583 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/arm/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3170 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/arch/arm/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5841 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/arm/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    57124 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/arm/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.073348 miasm-0.1.4/miasm/arch/mep/
--rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/mep/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    67308 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/mep/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      569 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/mep/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3297 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/mep/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1211 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/mep/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3528 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/mep/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    33760 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/mep/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.076681 miasm-0.1.4/miasm/arch/mips32/
--rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/mips32/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    27559 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/mips32/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      442 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/mips32/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5687 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/arch/mips32/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3275 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/mips32/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2726 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/mips32/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    18421 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/arch/mips32/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.076681 miasm-0.1.4/miasm/arch/msp430/
--rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/msp430/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    18343 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/msp430/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2600 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/msp430/ctype.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      240 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/msp430/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1205 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/msp430/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      958 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/msp430/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2914 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/msp430/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    12664 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/msp430/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.080014 miasm-0.1.4/miasm/arch/ppc/
--rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/ppc/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    27191 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/ppc/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      255 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/ppc/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2217 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/ppc/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2579 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/ppc/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3140 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/ppc/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    28791 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/ppc/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.083348 miasm-0.1.4/miasm/arch/sh4/
--rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/sh4/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    31603 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/sh4/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2158 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/sh4/regs.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.086681 miasm-0.1.4/miasm/arch/x86/
--rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/x86/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)   151299 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/x86/arch.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5080 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/arch/x86/ctype.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      581 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/x86/disasm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     9864 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/x86/jit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1998 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/arch/x86/lifter_model_call.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    12022 2023-04-05 15:00:32.000000 miasm-0.1.4/miasm/arch/x86/regs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)   177294 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/arch/x86/sem.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.093348 miasm-0.1.4/miasm/core/
--rw-r--r--   0 serpilliere  (1000) users      (985)       18 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/core/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1998 2021-10-04 17:15:41.000000 miasm-0.1.4/miasm/core/asm_ast.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    51507 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/asmblock.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     9610 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/bin_stream.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1368 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/core/bin_stream_ida.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    48186 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/cpu.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    23630 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/core/ctypesmngr.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    38246 2022-04-15 11:00:24.000000 miasm-0.1.4/miasm/core/graph.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     8511 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/core/interval.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    18765 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/locationdb.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6711 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/core/modint.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    55183 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/objc.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     9290 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/parse_asm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    13186 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/core/sembuilder.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    57205 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/core/types.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     7874 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/core/utils.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.096681 miasm-0.1.4/miasm/expression/
--rw-r--r--   0 serpilliere  (1000) users      (985)      828 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/expression/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    61236 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/expression/expression.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    20658 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/expression/expression_helper.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     8640 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/expression/expression_reduce.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3404 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/expression/parser.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     7270 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/expression/simplifications.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    57956 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/expression/simplifications_common.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4736 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/expression/simplifications_cond.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4228 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/expression/simplifications_explicit.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5822 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/expression/smt2_helper.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.100014 miasm-0.1.4/miasm/ir/
--rw-r--r--   0 serpilliere  (1000) users      (985)       38 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/ir/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3689 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/ir/analysis.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    35042 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/ir/ir.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    37454 2022-03-24 07:17:16.000000 miasm-0.1.4/miasm/ir/symbexec.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     7210 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/ir/symbexec_top.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3922 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/ir/symbexec_types.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4632 2021-01-07 10:40:57.000000 miasm-0.1.4/miasm/ir/test_ir.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.106681 miasm-0.1.4/miasm/ir/translators/
--rw-r--r--   0 serpilliere  (1000) users      (985)    19866 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/ir/translators/C.py
--rw-r--r--   0 serpilliere  (1000) users      (985)      347 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/ir/translators/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     1507 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/ir/translators/miasm_ir.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3338 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/ir/translators/python.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    11987 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/ir/translators/smt2.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4001 2022-05-04 11:09:58.000000 miasm-0.1.4/miasm/ir/translators/translator.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    10482 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/ir/translators/z3_ir.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.123348 miasm-0.1.4/miasm/jitter/
--rw-r--r--   0 serpilliere  (1000) users      (985)     4886 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/JitCore.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     6741 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/JitCore.h
--rw-r--r--   0 serpilliere  (1000) users      (985)     1860 2021-06-18 12:39:16.000000 miasm-0.1.4/miasm/jitter/Jitgcc.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     1915 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/Jitllvm.c
--rw-r--r--   0 serpilliere  (1000) users      (985)       33 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/jitter/__init__.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.136681 miasm-0.1.4/miasm/jitter/arch/
--rw-r--r--   0 serpilliere  (1000) users      (985)    16182 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_aarch64.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     1044 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_aarch64.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    13257 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_arm.c
--rw-r--r--   0 serpilliere  (1000) users      (985)      878 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_arm.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    13150 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_m68k.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     1004 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_m68k.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    18880 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_mep.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     1452 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_mep.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    15038 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_mips32.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     6390 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_mips32.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    12335 2021-08-30 05:58:06.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_msp430.c
--rw-r--r--   0 serpilliere  (1000) users      (985)      848 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_msp430.h
--rw-r--r--   0 serpilliere  (1000) users      (985)     7688 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32.c
--rw-r--r--   0 serpilliere  (1000) users      (985)      713 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32.h
--rw-r--r--   0 serpilliere  (1000) users      (985)     6172 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32_regs.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    28554 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_x86.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     2225 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/arch/JitCore_x86.h
--rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/jitter/arch/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    17860 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/bn.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     6440 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/bn.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    22931 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/codegen.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6412 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/compat_py23.h
--rw-r--r--   0 serpilliere  (1000) users      (985)     1404 2021-10-29 18:28:04.000000 miasm-0.1.4/miasm/jitter/csts.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5328 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/emulatedsymbexec.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    10866 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/jitcore.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3849 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/jitcore_cc_base.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     5329 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/jitcore_gcc.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4710 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/jitcore_llvm.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     8421 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/jitcore_python.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    19180 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/jitload.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    69203 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/llvmconvert.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.140014 miasm-0.1.4/miasm/jitter/loader/
--rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/jitter/loader/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    49506 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/jitter/loader/apiset_win10.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    12741 2023-04-04 15:51:10.000000 miasm-0.1.4/miasm/jitter/loader/elf.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    24479 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/jitter/loader/pe.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     3409 2021-07-31 11:12:12.000000 miasm-0.1.4/miasm/jitter/loader/utils.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    16167 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/op_semantics.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     6090 2021-08-30 05:58:06.000000 miasm-0.1.4/miasm/jitter/op_semantics.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    17719 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/queue.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    25228 2022-04-28 09:01:57.000000 miasm-0.1.4/miasm/jitter/vm_mngr.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     9962 2023-04-05 15:00:32.000000 miasm-0.1.4/miasm/jitter/vm_mngr.h
--rw-r--r--   0 serpilliere  (1000) users      (985)    29709 2022-04-28 09:01:57.000000 miasm-0.1.4/miasm/jitter/vm_mngr_py.c
--rw-r--r--   0 serpilliere  (1000) users      (985)      259 2020-07-23 05:24:48.000000 miasm-0.1.4/miasm/jitter/vm_mngr_py.h
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.150014 miasm-0.1.4/miasm/loader/
--rw-r--r--   0 serpilliere  (1000) users      (985)       73 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4090 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/cstruct.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    74531 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/elf.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    24756 2021-10-29 18:28:04.000000 miasm-0.1.4/miasm/loader/elf_init.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    19467 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/minidump.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6797 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/minidump_init.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     8816 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/loader/new_cstruct.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    63449 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/loader/pe.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    21896 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/loader/pe_init.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     2791 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/loader/strpatchwork.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.156681 miasm-0.1.4/miasm/os_dep/
--rw-r--r--   0 serpilliere  (1000) users      (985)       36 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/os_dep/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     4757 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/os_dep/common.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.160014 miasm-0.1.4/miasm/os_dep/linux/
--rw-r--r--   0 serpilliere  (1000) users      (985)       18 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/os_dep/linux/__init__.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    30916 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/os_dep/linux/environment.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    33578 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/os_dep/linux/syscall.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6366 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/os_dep/linux_stdlib.py
--rw-r--r--   0 serpilliere  (1000) users      (985)     6555 2020-12-07 17:06:02.000000 miasm-0.1.4/miasm/os_dep/win_32_structs.py
--rw-r--r--   0 serpilliere  (1000) users      (985)   119905 2022-03-24 07:22:49.000000 miasm-0.1.4/miasm/os_dep/win_api_x86_32.py
--rw-r--r--   0 serpilliere  (1000) users      (985)    21475 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/os_dep/win_api_x86_32_seh.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.160014 miasm-0.1.4/miasm/runtime/
--rw-r--r--   0 serpilliere  (1000) users      (985)     1219 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/runtime/divti3.c
--rw-r--r--   0 serpilliere  (1000) users      (985)     5461 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/runtime/udivmodti4.c
--rw-r--r--   0 serpilliere  (1000) users      (985)      717 2021-10-29 18:27:09.000000 miasm-0.1.4/miasm/runtime/udivti3.c
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.060014 miasm-0.1.4/miasm.egg-info/
--rw-r--r--   0 serpilliere  (1000) users      (985)    22076 2023-04-05 21:33:43.000000 miasm-0.1.4/miasm.egg-info/PKG-INFO
--rw-r--r--   0 serpilliere  (1000) users      (985)     5247 2023-04-05 21:33:44.000000 miasm-0.1.4/miasm.egg-info/SOURCES.txt
--rw-r--r--   0 serpilliere  (1000) users      (985)        1 2023-04-05 21:33:43.000000 miasm-0.1.4/miasm.egg-info/dependency_links.txt
--rw-r--r--   0 serpilliere  (1000) users      (985)       22 2023-04-05 21:33:43.000000 miasm-0.1.4/miasm.egg-info/requires.txt
--rw-r--r--   0 serpilliere  (1000) users      (985)      316 2023-04-05 21:33:43.000000 miasm-0.1.4/miasm.egg-info/top_level.txt
--rw-r--r--   0 serpilliere  (1000) users      (985)       38 2023-04-05 21:33:44.163348 miasm-0.1.4/setup.cfg
--rw-r--r--   0 serpilliere  (1000) users      (985)    15830 2023-04-05 15:00:32.000000 miasm-0.1.4/setup.py
-drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-05 21:33:44.163348 miasm-0.1.4/test/
--rwxr-xr-x   0 serpilliere  (1000) users      (985)    39034 2023-04-04 15:51:10.000000 miasm-0.1.4/test/test_all.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.159966 miasm-0.1.5/
+-rw-r--r--   0 serpilliere  (1000) users      (985)    18092 2020-07-23 05:24:48.000000 miasm-0.1.5/LICENSE
+-rw-r--r--   0 serpilliere  (1000) users      (985)    22076 2023-04-18 21:27:11.159966 miasm-0.1.5/PKG-INFO
+-rw-r--r--   0 serpilliere  (1000) users      (985)    21508 2023-04-04 15:51:10.000000 miasm-0.1.5/README.md
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.133299 miasm-0.1.5/miasm/
+-rw-r--r--   0 serpilliere  (1000) users      (985)        5 2023-04-18 21:27:10.000000 miasm-0.1.5/miasm/VERSION
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2732 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/__init__.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.136633 miasm-0.1.5/miasm/analysis/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       39 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/analysis/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     8209 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/analysis/apiset.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     7462 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/binary.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6170 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/cst_propag.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6829 2021-10-29 18:28:04.000000 miasm-0.1.5/miasm/analysis/data_analysis.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    79542 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/data_flow.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    16691 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/debugging.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    22278 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/depgraph.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3978 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/disasm_cb.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    29010 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/dse.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2653 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/analysis/expression_range.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    14342 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/gdbserver.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    10602 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/analysis/machine.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    19291 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/modularintervals.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    16079 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/outofssa.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    33866 2021-10-29 18:28:04.000000 miasm-0.1.5/miasm/analysis/sandbox.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     9574 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/simplifier.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    24132 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/analysis/ssa.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.136633 miasm-0.1.5/miasm/arch/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       31 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/__init__.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.136633 miasm-0.1.5/miasm/arch/aarch64/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/aarch64/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    84898 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/aarch64/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      731 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/aarch64/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2536 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/aarch64/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1244 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/aarch64/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    10375 2021-10-29 18:28:04.000000 miasm-0.1.5/miasm/arch/aarch64/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    63189 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/aarch64/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.139966 miasm-0.1.5/miasm/arch/arm/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/arm/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)   107077 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/arm/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1690 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/arm/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4583 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/arm/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3170 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/arch/arm/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5841 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/arm/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    57124 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/arm/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.139966 miasm-0.1.5/miasm/arch/mep/
+-rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/mep/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    67308 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/mep/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      569 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/mep/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3297 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/mep/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1211 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/mep/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3528 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/mep/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    33760 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/mep/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.139966 miasm-0.1.5/miasm/arch/mips32/
+-rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/mips32/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    27559 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/mips32/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      442 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/mips32/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5687 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/arch/mips32/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3275 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/mips32/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2726 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/mips32/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    18421 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/arch/mips32/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.139966 miasm-0.1.5/miasm/arch/msp430/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/msp430/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    18343 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/msp430/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2600 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/msp430/ctype.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      240 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/msp430/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1205 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/msp430/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      958 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/msp430/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2914 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/msp430/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    12664 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/msp430/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.143299 miasm-0.1.5/miasm/arch/ppc/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/ppc/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    27191 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/ppc/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      255 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/ppc/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2217 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/ppc/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2579 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/ppc/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3140 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/ppc/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    28791 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/ppc/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.143299 miasm-0.1.5/miasm/arch/sh4/
+-rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/sh4/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    31603 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/sh4/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2158 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/sh4/regs.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.143299 miasm-0.1.5/miasm/arch/x86/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       44 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/x86/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)   151299 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/x86/arch.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5080 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/arch/x86/ctype.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      581 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/x86/disasm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     9864 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/x86/jit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1998 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/arch/x86/lifter_model_call.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    12022 2023-04-05 15:00:32.000000 miasm-0.1.5/miasm/arch/x86/regs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)   177294 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/arch/x86/sem.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.146633 miasm-0.1.5/miasm/core/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       18 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/core/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1998 2021-10-04 17:15:41.000000 miasm-0.1.5/miasm/core/asm_ast.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    51507 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/asmblock.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     9610 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/bin_stream.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1368 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/core/bin_stream_ida.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    48186 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/cpu.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    23630 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/core/ctypesmngr.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    38246 2022-04-15 11:00:24.000000 miasm-0.1.5/miasm/core/graph.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     8511 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/core/interval.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    18765 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/locationdb.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6711 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/core/modint.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    55183 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/objc.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     9290 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/parse_asm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    13186 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/core/sembuilder.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    57205 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/core/types.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     7874 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/core/utils.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.146633 miasm-0.1.5/miasm/expression/
+-rw-r--r--   0 serpilliere  (1000) users      (985)      828 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/expression/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    61236 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/expression/expression.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    20658 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/expression/expression_helper.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     8640 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/expression/expression_reduce.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3404 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/expression/parser.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     7270 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/expression/simplifications.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    57956 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/expression/simplifications_common.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4736 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/expression/simplifications_cond.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4228 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/expression/simplifications_explicit.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5822 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/expression/smt2_helper.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.146633 miasm-0.1.5/miasm/ir/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       38 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/ir/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3689 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/ir/analysis.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    35042 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/ir/ir.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    37454 2022-03-24 07:17:16.000000 miasm-0.1.5/miasm/ir/symbexec.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     7210 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/ir/symbexec_top.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3922 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/ir/symbexec_types.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4632 2021-01-07 10:40:57.000000 miasm-0.1.5/miasm/ir/test_ir.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.153299 miasm-0.1.5/miasm/ir/translators/
+-rw-r--r--   0 serpilliere  (1000) users      (985)    19866 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/ir/translators/C.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)      347 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/ir/translators/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1507 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/ir/translators/miasm_ir.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3338 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/ir/translators/python.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    11987 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/ir/translators/smt2.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4001 2022-05-04 11:09:58.000000 miasm-0.1.5/miasm/ir/translators/translator.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    10482 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/ir/translators/z3_ir.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.153299 miasm-0.1.5/miasm/jitter/
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4886 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/JitCore.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6741 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/JitCore.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1860 2021-06-18 12:39:16.000000 miasm-0.1.5/miasm/jitter/Jitgcc.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1915 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/Jitllvm.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)       33 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/jitter/__init__.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.153299 miasm-0.1.5/miasm/jitter/arch/
+-rw-r--r--   0 serpilliere  (1000) users      (985)    16182 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_aarch64.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1044 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_aarch64.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    13257 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_arm.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      878 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_arm.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    13150 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_m68k.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1004 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_m68k.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    18880 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_mep.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1452 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_mep.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    15038 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_mips32.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6390 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_mips32.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    12335 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_msp430.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      848 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_msp430.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     7688 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      713 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6172 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32_regs.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    28554 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_x86.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2225 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/arch/JitCore_x86.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/jitter/arch/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    17860 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/bn.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6440 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/bn.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    22931 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/codegen.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6412 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/compat_py23.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1404 2021-10-29 18:28:04.000000 miasm-0.1.5/miasm/jitter/csts.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5328 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/emulatedsymbexec.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    10866 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/jitcore.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3849 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/jitcore_cc_base.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5329 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/jitcore_gcc.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4710 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/jitcore_llvm.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     8421 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/jitcore_python.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    19180 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/jitload.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    69203 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/llvmconvert.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.153299 miasm-0.1.5/miasm/jitter/loader/
+-rw-r--r--   0 serpilliere  (1000) users      (985)        0 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/jitter/loader/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    49506 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/jitter/loader/apiset_win10.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    12741 2023-04-04 15:51:10.000000 miasm-0.1.5/miasm/jitter/loader/elf.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    24479 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/jitter/loader/pe.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3409 2021-07-31 11:12:12.000000 miasm-0.1.5/miasm/jitter/loader/utils.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    16167 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/op_semantics.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6090 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/jitter/op_semantics.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    17719 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/queue.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    25228 2022-04-28 09:01:57.000000 miasm-0.1.5/miasm/jitter/vm_mngr.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)     9962 2023-04-05 15:00:32.000000 miasm-0.1.5/miasm/jitter/vm_mngr.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)    29709 2022-04-28 09:01:57.000000 miasm-0.1.5/miasm/jitter/vm_mngr_py.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      259 2020-07-23 05:24:48.000000 miasm-0.1.5/miasm/jitter/vm_mngr_py.h
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.156633 miasm-0.1.5/miasm/loader/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       73 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4090 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/cstruct.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    74531 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/elf.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    24756 2021-10-29 18:28:04.000000 miasm-0.1.5/miasm/loader/elf_init.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    19467 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/minidump.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6797 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/minidump_init.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     8816 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/loader/new_cstruct.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    63449 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/loader/pe.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    21896 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/loader/pe_init.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2791 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/loader/strpatchwork.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.156633 miasm-0.1.5/miasm/os_dep/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       36 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/os_dep/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4757 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/os_dep/common.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.156633 miasm-0.1.5/miasm/os_dep/linux/
+-rw-r--r--   0 serpilliere  (1000) users      (985)       18 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/os_dep/linux/__init__.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    30916 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/os_dep/linux/environment.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    33578 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/os_dep/linux/syscall.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6366 2023-04-18 21:18:43.000000 miasm-0.1.5/miasm/os_dep/linux_stdlib.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)     6555 2020-12-07 17:06:02.000000 miasm-0.1.5/miasm/os_dep/win_32_structs.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)   119905 2022-03-24 07:22:49.000000 miasm-0.1.5/miasm/os_dep/win_api_x86_32.py
+-rw-r--r--   0 serpilliere  (1000) users      (985)    21475 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/os_dep/win_api_x86_32_seh.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.156633 miasm-0.1.5/miasm/runtime/
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1219 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/runtime/divti3.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      193 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/runtime/export.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     2818 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/runtime/int_endianness.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     4426 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/runtime/int_lib.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     3782 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/runtime/int_types.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     1355 2021-08-30 05:58:06.000000 miasm-0.1.5/miasm/runtime/int_util.h
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5461 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/runtime/udivmodti4.c
+-rw-r--r--   0 serpilliere  (1000) users      (985)      717 2021-10-29 18:27:09.000000 miasm-0.1.5/miasm/runtime/udivti3.c
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.133299 miasm-0.1.5/miasm.egg-info/
+-rw-r--r--   0 serpilliere  (1000) users      (985)    22076 2023-04-18 21:27:10.000000 miasm-0.1.5/miasm.egg-info/PKG-INFO
+-rw-r--r--   0 serpilliere  (1000) users      (985)     5376 2023-04-18 21:27:11.000000 miasm-0.1.5/miasm.egg-info/SOURCES.txt
+-rw-r--r--   0 serpilliere  (1000) users      (985)        1 2023-04-18 21:27:10.000000 miasm-0.1.5/miasm.egg-info/dependency_links.txt
+-rw-r--r--   0 serpilliere  (1000) users      (985)       22 2023-04-18 21:27:10.000000 miasm-0.1.5/miasm.egg-info/requires.txt
+-rw-r--r--   0 serpilliere  (1000) users      (985)      316 2023-04-18 21:27:10.000000 miasm-0.1.5/miasm.egg-info/top_level.txt
+-rw-r--r--   0 serpilliere  (1000) users      (985)       38 2023-04-18 21:27:11.159966 miasm-0.1.5/setup.cfg
+-rw-r--r--   0 serpilliere  (1000) users      (985)    16145 2023-04-18 21:21:45.000000 miasm-0.1.5/setup.py
+drwxr-xr-x   0 serpilliere  (1000) users      (985)        0 2023-04-18 21:27:11.156633 miasm-0.1.5/test/
+-rwxr-xr-x   0 serpilliere  (1000) users      (985)    39034 2023-04-04 15:51:10.000000 miasm-0.1.5/test/test_all.py
```

### Comparing `miasm-0.1.4/LICENSE` & `miasm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/PKG-INFO` & `miasm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miasm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Machine code manipulation library
 Home-page: http://miasm.re
 Author: Fabrice Desclaux
 Author-email: serpilliere@droid-corp.org
 License: GPLv2
 Keywords: reverse engineering,disassembler,emulator,symbolic execution,intermediate representation,assembler
 Classifier: Programming Language :: Python :: 2
```

### Comparing `miasm-0.1.4/README.md` & `miasm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/__init__.py` & `miasm-0.1.5/miasm/__init__.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/apiset.py` & `miasm-0.1.5/miasm/analysis/apiset.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/binary.py` & `miasm-0.1.5/miasm/analysis/binary.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/cst_propag.py` & `miasm-0.1.5/miasm/analysis/cst_propag.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/data_analysis.py` & `miasm-0.1.5/miasm/analysis/data_analysis.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/data_flow.py` & `miasm-0.1.5/miasm/analysis/data_flow.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/debugging.py` & `miasm-0.1.5/miasm/analysis/debugging.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/depgraph.py` & `miasm-0.1.5/miasm/analysis/depgraph.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/disasm_cb.py` & `miasm-0.1.5/miasm/analysis/disasm_cb.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/dse.py` & `miasm-0.1.5/miasm/analysis/dse.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/expression_range.py` & `miasm-0.1.5/miasm/analysis/expression_range.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/gdbserver.py` & `miasm-0.1.5/miasm/analysis/gdbserver.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/machine.py` & `miasm-0.1.5/miasm/analysis/machine.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/modularintervals.py` & `miasm-0.1.5/miasm/analysis/modularintervals.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/outofssa.py` & `miasm-0.1.5/miasm/analysis/outofssa.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/sandbox.py` & `miasm-0.1.5/miasm/analysis/sandbox.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/simplifier.py` & `miasm-0.1.5/miasm/analysis/simplifier.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/analysis/ssa.py` & `miasm-0.1.5/miasm/analysis/ssa.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/arch.py` & `miasm-0.1.5/miasm/arch/aarch64/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/disasm.py` & `miasm-0.1.5/miasm/arch/aarch64/disasm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/jit.py` & `miasm-0.1.5/miasm/arch/aarch64/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/aarch64/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/regs.py` & `miasm-0.1.5/miasm/arch/aarch64/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/aarch64/sem.py` & `miasm-0.1.5/miasm/arch/aarch64/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/arch.py` & `miasm-0.1.5/miasm/arch/arm/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/disasm.py` & `miasm-0.1.5/miasm/arch/arm/disasm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/jit.py` & `miasm-0.1.5/miasm/arch/arm/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/arm/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/regs.py` & `miasm-0.1.5/miasm/arch/arm/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/arm/sem.py` & `miasm-0.1.5/miasm/arch/arm/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/arch.py` & `miasm-0.1.5/miasm/arch/mep/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/disasm.py` & `miasm-0.1.5/miasm/arch/mep/disasm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/jit.py` & `miasm-0.1.5/miasm/arch/mep/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/mep/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/regs.py` & `miasm-0.1.5/miasm/arch/mep/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mep/sem.py` & `miasm-0.1.5/miasm/arch/mep/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mips32/arch.py` & `miasm-0.1.5/miasm/arch/mips32/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mips32/jit.py` & `miasm-0.1.5/miasm/arch/mips32/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mips32/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/mips32/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mips32/regs.py` & `miasm-0.1.5/miasm/arch/mips32/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/mips32/sem.py` & `miasm-0.1.5/miasm/arch/mips32/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/arch.py` & `miasm-0.1.5/miasm/arch/msp430/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/ctype.py` & `miasm-0.1.5/miasm/arch/msp430/ctype.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/jit.py` & `miasm-0.1.5/miasm/arch/msp430/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/msp430/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/regs.py` & `miasm-0.1.5/miasm/arch/msp430/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/msp430/sem.py` & `miasm-0.1.5/miasm/arch/msp430/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/ppc/arch.py` & `miasm-0.1.5/miasm/arch/ppc/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/ppc/jit.py` & `miasm-0.1.5/miasm/arch/ppc/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/ppc/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/ppc/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/ppc/regs.py` & `miasm-0.1.5/miasm/arch/ppc/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/ppc/sem.py` & `miasm-0.1.5/miasm/arch/ppc/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/sh4/arch.py` & `miasm-0.1.5/miasm/arch/sh4/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/sh4/regs.py` & `miasm-0.1.5/miasm/arch/sh4/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/arch.py` & `miasm-0.1.5/miasm/arch/x86/arch.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/ctype.py` & `miasm-0.1.5/miasm/arch/x86/ctype.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/disasm.py` & `miasm-0.1.5/miasm/arch/x86/disasm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/jit.py` & `miasm-0.1.5/miasm/arch/x86/jit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/lifter_model_call.py` & `miasm-0.1.5/miasm/arch/x86/lifter_model_call.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/regs.py` & `miasm-0.1.5/miasm/arch/x86/regs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/arch/x86/sem.py` & `miasm-0.1.5/miasm/arch/x86/sem.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/asm_ast.py` & `miasm-0.1.5/miasm/core/asm_ast.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/asmblock.py` & `miasm-0.1.5/miasm/core/asmblock.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/bin_stream.py` & `miasm-0.1.5/miasm/core/bin_stream.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/bin_stream_ida.py` & `miasm-0.1.5/miasm/core/bin_stream_ida.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/cpu.py` & `miasm-0.1.5/miasm/core/cpu.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/ctypesmngr.py` & `miasm-0.1.5/miasm/core/ctypesmngr.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/graph.py` & `miasm-0.1.5/miasm/core/graph.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/interval.py` & `miasm-0.1.5/miasm/core/interval.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/locationdb.py` & `miasm-0.1.5/miasm/core/locationdb.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/modint.py` & `miasm-0.1.5/miasm/core/modint.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/objc.py` & `miasm-0.1.5/miasm/core/objc.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/parse_asm.py` & `miasm-0.1.5/miasm/core/parse_asm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/sembuilder.py` & `miasm-0.1.5/miasm/core/sembuilder.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/types.py` & `miasm-0.1.5/miasm/core/types.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/core/utils.py` & `miasm-0.1.5/miasm/core/utils.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/__init__.py` & `miasm-0.1.5/miasm/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/expression.py` & `miasm-0.1.5/miasm/expression/expression.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/expression_helper.py` & `miasm-0.1.5/miasm/expression/expression_helper.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/expression_reduce.py` & `miasm-0.1.5/miasm/expression/expression_reduce.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/parser.py` & `miasm-0.1.5/miasm/expression/parser.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/simplifications.py` & `miasm-0.1.5/miasm/expression/simplifications.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/simplifications_common.py` & `miasm-0.1.5/miasm/expression/simplifications_common.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/simplifications_cond.py` & `miasm-0.1.5/miasm/expression/simplifications_cond.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/simplifications_explicit.py` & `miasm-0.1.5/miasm/expression/simplifications_explicit.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/expression/smt2_helper.py` & `miasm-0.1.5/miasm/expression/smt2_helper.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/analysis.py` & `miasm-0.1.5/miasm/ir/analysis.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/ir.py` & `miasm-0.1.5/miasm/ir/ir.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/symbexec.py` & `miasm-0.1.5/miasm/ir/symbexec.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/symbexec_top.py` & `miasm-0.1.5/miasm/ir/symbexec_top.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/symbexec_types.py` & `miasm-0.1.5/miasm/ir/symbexec_types.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/test_ir.py` & `miasm-0.1.5/miasm/ir/test_ir.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/C.py` & `miasm-0.1.5/miasm/ir/translators/C.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/miasm_ir.py` & `miasm-0.1.5/miasm/ir/translators/miasm_ir.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/python.py` & `miasm-0.1.5/miasm/ir/translators/python.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/smt2.py` & `miasm-0.1.5/miasm/ir/translators/smt2.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/translator.py` & `miasm-0.1.5/miasm/ir/translators/translator.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/ir/translators/z3_ir.py` & `miasm-0.1.5/miasm/ir/translators/z3_ir.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/JitCore.c` & `miasm-0.1.5/miasm/jitter/JitCore.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/JitCore.h` & `miasm-0.1.5/miasm/jitter/JitCore.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/Jitgcc.c` & `miasm-0.1.5/miasm/jitter/Jitgcc.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/Jitllvm.c` & `miasm-0.1.5/miasm/jitter/Jitllvm.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_aarch64.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_aarch64.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_aarch64.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_aarch64.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_arm.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_arm.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_arm.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_arm.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_m68k.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_m68k.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_m68k.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_m68k.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_mep.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_mep.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_mep.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_mep.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_mips32.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_mips32.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_mips32.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_mips32.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_msp430.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_msp430.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_msp430.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_msp430.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_ppc32_regs.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_ppc32_regs.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_x86.c` & `miasm-0.1.5/miasm/jitter/arch/JitCore_x86.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/arch/JitCore_x86.h` & `miasm-0.1.5/miasm/jitter/arch/JitCore_x86.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/bn.c` & `miasm-0.1.5/miasm/jitter/bn.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/bn.h` & `miasm-0.1.5/miasm/jitter/bn.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/codegen.py` & `miasm-0.1.5/miasm/jitter/codegen.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/compat_py23.h` & `miasm-0.1.5/miasm/jitter/compat_py23.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/csts.py` & `miasm-0.1.5/miasm/jitter/csts.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/emulatedsymbexec.py` & `miasm-0.1.5/miasm/jitter/emulatedsymbexec.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitcore.py` & `miasm-0.1.5/miasm/jitter/jitcore.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitcore_cc_base.py` & `miasm-0.1.5/miasm/jitter/jitcore_cc_base.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitcore_gcc.py` & `miasm-0.1.5/miasm/jitter/jitcore_gcc.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitcore_llvm.py` & `miasm-0.1.5/miasm/jitter/jitcore_llvm.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitcore_python.py` & `miasm-0.1.5/miasm/jitter/jitcore_python.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/jitload.py` & `miasm-0.1.5/miasm/jitter/jitload.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/llvmconvert.py` & `miasm-0.1.5/miasm/jitter/llvmconvert.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/loader/apiset_win10.py` & `miasm-0.1.5/miasm/jitter/loader/apiset_win10.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/loader/elf.py` & `miasm-0.1.5/miasm/jitter/loader/elf.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/loader/pe.py` & `miasm-0.1.5/miasm/jitter/loader/pe.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/loader/utils.py` & `miasm-0.1.5/miasm/jitter/loader/utils.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/op_semantics.c` & `miasm-0.1.5/miasm/jitter/op_semantics.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/op_semantics.h` & `miasm-0.1.5/miasm/jitter/op_semantics.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/queue.h` & `miasm-0.1.5/miasm/jitter/queue.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/vm_mngr.c` & `miasm-0.1.5/miasm/jitter/vm_mngr.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/vm_mngr.h` & `miasm-0.1.5/miasm/jitter/vm_mngr.h`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/jitter/vm_mngr_py.c` & `miasm-0.1.5/miasm/jitter/vm_mngr_py.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/cstruct.py` & `miasm-0.1.5/miasm/loader/cstruct.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/elf.py` & `miasm-0.1.5/miasm/loader/elf.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/elf_init.py` & `miasm-0.1.5/miasm/loader/elf_init.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/minidump.py` & `miasm-0.1.5/miasm/loader/minidump.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/minidump_init.py` & `miasm-0.1.5/miasm/loader/minidump_init.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/new_cstruct.py` & `miasm-0.1.5/miasm/loader/new_cstruct.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/pe.py` & `miasm-0.1.5/miasm/loader/pe.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/pe_init.py` & `miasm-0.1.5/miasm/loader/pe_init.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/loader/strpatchwork.py` & `miasm-0.1.5/miasm/loader/strpatchwork.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/common.py` & `miasm-0.1.5/miasm/os_dep/common.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/linux/environment.py` & `miasm-0.1.5/miasm/os_dep/linux/environment.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/linux/syscall.py` & `miasm-0.1.5/miasm/os_dep/linux/syscall.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/linux_stdlib.py` & `miasm-0.1.5/miasm/os_dep/linux_stdlib.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/win_32_structs.py` & `miasm-0.1.5/miasm/os_dep/win_32_structs.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/win_api_x86_32.py` & `miasm-0.1.5/miasm/os_dep/win_api_x86_32.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/os_dep/win_api_x86_32_seh.py` & `miasm-0.1.5/miasm/os_dep/win_api_x86_32_seh.py`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/runtime/divti3.c` & `miasm-0.1.5/miasm/runtime/divti3.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/runtime/udivmodti4.c` & `miasm-0.1.5/miasm/runtime/udivmodti4.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm/runtime/udivti3.c` & `miasm-0.1.5/miasm/runtime/udivti3.c`

 * *Files identical despite different names*

### Comparing `miasm-0.1.4/miasm.egg-info/PKG-INFO` & `miasm-0.1.5/miasm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miasm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Machine code manipulation library
 Home-page: http://miasm.re
 Author: Fabrice Desclaux
 Author-email: serpilliere@droid-corp.org
 License: GPLv2
 Keywords: reverse engineering,disassembler,emulator,symbolic execution,intermediate representation,assembler
 Classifier: Programming Language :: Python :: 2
```

### Comparing `miasm-0.1.4/miasm.egg-info/SOURCES.txt` & `miasm-0.1.5/miasm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -185,10 +185,15 @@
 miasm/os_dep/win_32_structs.py
 miasm/os_dep/win_api_x86_32.py
 miasm/os_dep/win_api_x86_32_seh.py
 miasm/os_dep/linux/__init__.py
 miasm/os_dep/linux/environment.py
 miasm/os_dep/linux/syscall.py
 miasm/runtime/divti3.c
+miasm/runtime/export.h
+miasm/runtime/int_endianness.h
+miasm/runtime/int_lib.h
+miasm/runtime/int_types.h
+miasm/runtime/int_util.h
 miasm/runtime/udivmodti4.c
 miasm/runtime/udivti3.c
 test/test_all.py
```

### Comparing `miasm-0.1.4/setup.py` & `miasm-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,21 +250,31 @@
                 "miasm/jitter/vm_mngr.c",
                 "miasm/jitter/vm_mngr_py.c",
                 "miasm/jitter/op_semantics.c",
                 "miasm/jitter/bn.c",
                 "miasm/jitter/arch/JitCore_m68k.c"
             ]
         ),
-        Extension("miasm.jitter.Jitllvm",
-                  ["miasm/jitter/Jitllvm.c",
-                   "miasm/jitter/bn.c",
-                   "miasm/runtime/udivmodti4.c",
-                   "miasm/runtime/divti3.c",
-                   "miasm/runtime/udivti3.c"
-                  ]),
+        Extension(
+            "miasm.jitter.Jitllvm",
+            [
+                "miasm/jitter/Jitllvm.c",
+                "miasm/jitter/bn.c",
+                "miasm/runtime/udivmodti4.c",
+                "miasm/runtime/divti3.c",
+                "miasm/runtime/udivti3.c"
+            ],
+            depends=[
+                "miasm/runtime/export.h",
+                "miasm/runtime/int_endianness.h",
+                "miasm/runtime/int_lib.h",
+                "miasm/runtime/int_types.h",
+                "miasm/runtime/int_util.h",
+            ]
+        ),
         Extension("miasm.jitter.Jitgcc",
                   ["miasm/jitter/Jitgcc.c",
                    "miasm/jitter/bn.c",
                   ]),
         ]
 
     if is_win:
@@ -307,14 +317,15 @@
                 version = __import__("miasm").VERSION,
                 packages = packages,
                 data_files=[("", ["README.md"])],
                 package_data = {
                     "miasm": [
                         "jitter/*.h",
                         "jitter/arch/*.h",
+                        "runtime/*.h",
                         "VERSION"
                     ]
                 },
                 install_requires=["future", "pyparsing~=2.0"],
                 cmdclass={"install_data": smart_install_data},
                 ext_modules = ext_modules,
                 # Metadata
```

### Comparing `miasm-0.1.4/test/test_all.py` & `miasm-0.1.5/test/test_all.py`

 * *Files identical despite different names*

