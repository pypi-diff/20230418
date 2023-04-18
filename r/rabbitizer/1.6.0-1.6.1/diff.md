# Comparing `tmp/rabbitizer-1.6.0.tar.gz` & `tmp/rabbitizer-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.6.0.tar", last modified: Mon Apr 17 20:19:35 2023, max compression
+gzip compressed data, was "rabbitizer-1.6.1.tar", last modified: Tue Apr 18 04:16:42 2023, max compression
```

## Comparing `rabbitizer-1.6.0.tar` & `rabbitizer-1.6.1.tar`

### file list

```diff
@@ -1,197 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.806258 rabbitizer-1.6.0/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrId_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/Registers_enums.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/Registers_enums.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.806258 rabbitizer-1.6.0/include/instructions/instr_id/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.810258 rabbitizer-1.6.0/include/instructions/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/operands/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.822258 rabbitizer-1.6.0/include/instructions/registers/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspVector.inc
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.830258 rabbitizer-1.6.0/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.830258 rabbitizer-1.6.0/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.794258 rabbitizer-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrCategory_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)   108158 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerRegisterDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.501833 rabbitizer-1.6.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.501833 rabbitizer-1.6.1/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.501833 rabbitizer-1.6.1/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/Abi_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.505833 rabbitizer-1.6.1/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/AccessType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrCategory_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrId_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrSuffix_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/OperandType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/OperandType_function_declarations.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/Registers_enums.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/Registers_enums.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.505833 rabbitizer-1.6.1/include/instructions/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.505833 rabbitizer-1.6.1/include/instructions/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.509832 rabbitizer-1.6.1/include/instructions/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.513833 rabbitizer-1.6.1/include/instructions/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.513833 rabbitizer-1.6.1/include/instructions/operands/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.513833 rabbitizer-1.6.1/include/instructions/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspVector.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.517833 rabbitizer-1.6.1/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegCop1N32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegCop1N64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegCop1O32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.521833 rabbitizer-1.6.1/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.521833 rabbitizer-1.6.1/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.517833 rabbitizer-1.6.1/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-18 04:16:42.000000 rabbitizer-1.6.1/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-18 04:16:42.000000 rabbitizer-1.6.1/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:16:42.000000 rabbitizer-1.6.1/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 04:16:42.000000 rabbitizer-1.6.1/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.501833 rabbitizer-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.521833 rabbitizer-1.6.1/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.521833 rabbitizer-1.6.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrCategory_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)   108158 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrDescriptor_Descriptors_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrId_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:16:42.525833 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RabbitizerRegisterDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/Registers_Names_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-18 04:16:34.000000 rabbitizer-1.6.1/src/instructions/Registers_Names_arrays.table.template
```

### Comparing `rabbitizer-1.6.0/LICENSE` & `rabbitizer-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/PKG-INFO` & `rabbitizer-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.6.0
+Version: 1.6.1
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.6.0/README.md` & `rabbitizer-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.6.1/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.6.1/include/analysis/RabbitizerRegistersTracker.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.6.1/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/common/RabbitizerConfig.h` & `rabbitizer-1.6.1/include/common/RabbitizerConfig.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/common/RabbitizerVersion.h` & `rabbitizer-1.6.1/include/common/RabbitizerVersion.h`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
 #define RAB_VERSION_MINOR 6
-#define RAB_VERSION_PATCH 0
+#define RAB_VERSION_PATCH 1
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 // Compiled library version
 extern const int RabVersion_Major;
 extern const int RabVersion_Minor;
 extern const int RabVersion_Patch;
```

### Comparing `rabbitizer-1.6.0/include/common/Utils.h` & `rabbitizer-1.6.1/include/common/Utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/InstrId_enum.table.h` & `rabbitizer-1.6.1/include/instructions/InstrId_enum.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/InstrId_enum.table.template` & `rabbitizer-1.6.1/include/instructions/InstrId_enum.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/OperandType_enum.table.h` & `rabbitizer-1.6.1/include/instructions/OperandType_enum.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.h` & `rabbitizer-1.6.1/include/instructions/OperandType_function_declarations.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstrId.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstrSuffix.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstruction.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstructionR5900.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerInstructionRsp.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerOperandType.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerRegister.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.6.1/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/Registers_enums.table.h` & `rabbitizer-1.6.1/include/instructions/Registers_enums.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/Registers_enums.table.template` & `rabbitizer-1.6.1/include/instructions/Registers_enums.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/cpu/cpu_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_special1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_3.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/r5900/r5900_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_swc2.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.6.1/include/instructions/instr_id/rsp/rsp_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_r5900.inc` & `rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.6.1/include/instructions/operands/RabbitizerOperandType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_Cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_GprN32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_GprO32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.6.1/include/instructions/registers/RabbitizerRegister_RspVector.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/include/rabbitizer.h` & `rabbitizer-1.6.1/include/rabbitizer.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/pyproject.toml` & `rabbitizer-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.6.0"
+version = "1.6.1"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.6.0/rabbitizer/Config.pyi` & `rabbitizer-1.6.1/rabbitizer/Config.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/Enum.pyi` & `rabbitizer-1.6.1/rabbitizer/Enum.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/InstrId.pyi` & `rabbitizer-1.6.1/rabbitizer/InstrId.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/OperandType.pyi` & `rabbitizer-1.6.1/rabbitizer/OperandType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.6.1/rabbitizer/RegGprN32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.6.1/rabbitizer/RegGprO32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.6.1/rabbitizer/RegistersTracker.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.6.1/rabbitizer/enums/enums_utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.6.1/rabbitizer/enums/enums_utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrId.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_OperandType.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_enum_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.6.1/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.6.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_global_config.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_module.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 #include <stdbool.h>
 
 #include "common/Utils.h"
@@ -42,14 +42,17 @@
     MODULE_ATTRIBUTE_ENUM(InstrCategory),
     MODULE_ATTRIBUTE_ENUM(InstrId),
     MODULE_ATTRIBUTE_ENUM(OperandType),
     MODULE_ATTRIBUTE_ENUM(AccessType),
 
     MODULE_ATTRIBUTE_ENUM(RegGprO32),
     MODULE_ATTRIBUTE_ENUM(RegGprN32),
+    MODULE_ATTRIBUTE_ENUM(RegCop1O32),
+    MODULE_ATTRIBUTE_ENUM(RegCop1N32),
+    MODULE_ATTRIBUTE_ENUM(RegCop1N64),
 
     MODULE_ATTRIBUTE_TYPE(Instruction),
     MODULE_ATTRIBUTE_TYPE(LoPairingInfo),
     MODULE_ATTRIBUTE_TYPE(TrackedRegisterState),
     MODULE_ATTRIBUTE_TYPE(RegistersTracker),
 };
```

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_module.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_MODULE_H
 #define RABBITIZER_MODULE_H
 #pragma once
 
 #define PY_SSIZE_T_CLEAN
@@ -49,8 +49,12 @@
 DECL_ENUM(InstrId)
 DECL_ENUM(OperandType)
 DECL_ENUM(AccessType)
 
 DECL_ENUM(RegGprO32)
 DECL_ENUM(RegGprN32)
 
+DECL_ENUM(RegCop1O32)
+DECL_ENUM(RegCop1N32)
+DECL_ENUM(RegCop1N64)
+
 #endif
```

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 #include "instructions/RabbitizerInstructionRsp.h"
 #include "instructions/RabbitizerInstructionR5900.h"
 #include "common/RabbitizerConfig.h"
@@ -12,15 +12,15 @@
     RabbitizerInstruction_destroy(&self->instr);
     Py_TYPE(self)->tp_free((PyObject *) self);
 }
 
 static int rabbitizer_type_Instruction_init(PyRabbitizerInstruction *self, PyObject *args, PyObject *kwds) {
     static char *kwlist[] = { "word", "vram", "category", NULL };
     uint32_t word;
-    uint32_t vram;
+    uint32_t vram = 0;
     PyObject *category = NULL;
     int enumCheck;
     RabbitizerInstrCategory instrCategory = RABBITIZER_INSTRCAT_CPU;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwds, "I|IO!", kwlist, &word, &vram, &rabbitizer_type_Enum_TypeObject, &category)) {
         return -1;
     }
@@ -129,14 +129,52 @@
 
 DEF_MEMBER_GET_REGGPR(rs)
 DEF_MEMBER_GET_REGGPR(rt)
 DEF_MEMBER_GET_REGGPR(rd)
 
 DEF_MEMBER_GET_UINT(sa)
 
+#define DEF_MEMBER_GET_REGCOP1(name) \
+    static PyObject *rabbitizer_type_Instruction_member_get_##name(PyRabbitizerInstruction *self, UNUSED PyObject *closure) { \
+        uint32_t reg; \
+        PyObject *enumInstance = NULL; \
+        \
+        if (!RabbitizerInstruction_hasOperandAlias(&self->instr, RAB_OPERAND_cpu_##name)) { \
+            PyErr_Format(PyExc_RuntimeError, "'%s' instruction does not reference register '" #name "'", RabbitizerInstrId_getOpcodeName(self->instr.uniqueId)); \
+            return NULL; \
+        } \
+        \
+        reg = RAB_INSTR_GET_##name(&self->instr); \
+        switch (RabbitizerConfig_Cfg.regNames.fprAbiNames) { \
+            case RABBITIZER_ABI_N32: \
+                enumInstance = rabbitizer_enum_RegCop1N32_enumvalues[reg].instance; \
+                break; \
+        \
+            case RABBITIZER_ABI_N64: \
+                enumInstance = rabbitizer_enum_RegCop1N64_enumvalues[reg].instance; \
+                break; \
+        \
+            default: \
+                enumInstance = rabbitizer_enum_RegCop1O32_enumvalues[reg].instance; \
+                break; \
+        } \
+        \
+        if (enumInstance == NULL) { \
+            PyErr_SetString(PyExc_RuntimeError, "Internal error: invalid RegCop1 enum value"); \
+            return NULL; \
+        } \
+        \
+        Py_INCREF(enumInstance); \
+        return enumInstance; \
+    }
+
+DEF_MEMBER_GET_REGCOP1(fs)
+DEF_MEMBER_GET_REGCOP1(ft)
+DEF_MEMBER_GET_REGCOP1(fd)
+
 static PyObject *rabbitizer_type_Instruction_member_get_uniqueId(PyRabbitizerInstruction *self, UNUSED PyObject *closure) {
     PyObject *enumInstance = rabbitizer_enum_InstrId_enumvalues[self->instr.uniqueId].instance;
 
     if (enumInstance == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "Internal error: invalid uniqueId enum value");
         return NULL;
     }
@@ -151,14 +189,17 @@
 
 
 static PyGetSetDef rabbitizer_type_Instruction_getsetters[] = {
     MEMBER_GET(rs, "", NULL),
     MEMBER_GET(rt, "", NULL),
     MEMBER_GET(rd, "", NULL),
     MEMBER_GET(sa, "", NULL),
+    MEMBER_GET(fs, "", NULL),
+    MEMBER_GET(ft, "", NULL),
+    MEMBER_GET(fd, "", NULL),
     MEMBER_GET(uniqueId, "", NULL),
 
     { 0 }
 };
 
 
 #define DEF_METHOD_GET_UINT(name) \
```

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.6.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.6.1/rabbitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.6.0
+Version: 1.6.1
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.6.0/rabbitizer.egg-info/SOURCES.txt` & `rabbitizer-1.6.1/rabbitizer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 rabbitizer/AccessType.pyi
 rabbitizer/Config.pyi
 rabbitizer/Enum.pyi
 rabbitizer/InstrCategory.pyi
 rabbitizer/InstrId.pyi
 rabbitizer/LoPairingInfo.pyi
 rabbitizer/OperandType.pyi
+rabbitizer/RegCop1N32.pyi
+rabbitizer/RegCop1N64.pyi
+rabbitizer/RegCop1O32.pyi
 rabbitizer/RegGprN32.pyi
 rabbitizer/RegGprO32.pyi
 rabbitizer/RegistersTracker.pyi
 rabbitizer/TrackedRegisterState.pyi
 rabbitizer/Utils.pyi
 rabbitizer/__init__.pyi
 rabbitizer/py.typed
@@ -128,14 +131,17 @@
 rabbitizer/enums/enums_utils.h
 rabbitizer/enums/rabbitizer_enum_Abi.c
 rabbitizer/enums/rabbitizer_enum_AccessType.c
 rabbitizer/enums/rabbitizer_enum_InstrCategory.c
 rabbitizer/enums/rabbitizer_enum_InstrId.c
 rabbitizer/enums/rabbitizer_enum_OperandType.c
 rabbitizer/enums/rabbitizer_type_Enum.c
+rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
 rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
 rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
 src/analysis/RabbitizerLoPairingInfo.c
 src/analysis/RabbitizerRegistersTracker.c
 src/analysis/RabbitizerTrackedRegisterState.c
 src/common/RabbitizerConfig.c
 src/common/RabbitizerVersion.c
```

### Comparing `rabbitizer-1.6.0/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.6.1/src/analysis/RabbitizerRegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.6.1/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/common/RabbitizerConfig.c` & `rabbitizer-1.6.1/src/common/RabbitizerConfig.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/common/Utils.c` & `rabbitizer-1.6.1/src/common/Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.h` & `rabbitizer-1.6.1/src/instructions/InstrDescriptor_Descriptors_array.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.template` & `rabbitizer-1.6.1/src/instructions/InstrDescriptor_Descriptors_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.h` & `rabbitizer-1.6.1/src/instructions/InstrId_Names_array.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.template` & `rabbitizer-1.6.1/src/instructions/InstrId_Names_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstrSuffix.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerRegister.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.6.1/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h` & `rabbitizer-1.6.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.6.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.h` & `rabbitizer-1.6.1/src/instructions/Registers_Names_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.template` & `rabbitizer-1.6.1/src/instructions/Registers_Names_arrays.table.template`

 * *Files identical despite different names*

