# Comparing `tmp/amaranth-0.4.4.tar.gz` & `tmp/amaranth-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaranth-0.4.4.tar", last modified: Fri Mar 15 12:12:42 2024, max compression
+gzip compressed data, was "amaranth-0.4.5.tar", last modified: Wed Apr  3 15:35:26 2024, max compression
```

## Comparing `amaranth-0.4.4.tar` & `amaranth-0.4.5.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1333 2024-03-15 12:12:34.690499 amaranth-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0     3280 2024-03-15 12:12:34.690499 amaranth-0.4.4/README.md
--rw-r--r--   0        0        0      908 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/__init__.py
--rw-r--r--   0        0        0     1053 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/_toolchain/__init__.py
--rw-r--r--   0        0        0     8475 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/_toolchain/yosys.py
--rw-r--r--   0        0        0     1459 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/_unused.py
--rw-r--r--   0        0        0     2942 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/_utils.py
--rw-r--r--   0        0        0      116 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/asserts.py
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/back/__init__.py
--rw-r--r--   0        0        0     1595 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/back/cxxrtl.py
--rw-r--r--   0        0        0    39258 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/back/rtlil.py
--rw-r--r--   0        0        0     2552 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/back/verilog.py
--rw-r--r--   0        0        0       70 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/build/__init__.py
--rw-r--r--   0        0        0    10006 2024-03-15 12:12:34.690499 amaranth-0.4.4/amaranth/build/dsl.py
--rw-r--r--   0        0        0    20626 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/build/plat.py
--rw-r--r--   0        0        0    12396 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/build/res.py
--rw-r--r--   0        0        0    11176 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/build/run.py
--rw-r--r--   0        0        0     3365 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/cli.py
--rw-r--r--   0        0        0      257 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/__init__.py
--rw-r--r--   0        0        0      569 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/bitcontainer.py
--rw-r--r--   0        0        0     1070 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/conv_output.py
--rw-r--r--   0        0        0     2122 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/decorators.py
--rw-r--r--   0        0        0     5206 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/module.py
--rw-r--r--   0        0        0     5152 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/specials.py
--rw-r--r--   0        0        0     6169 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/structure.py
--rw-r--r--   0        0        0     1066 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/fhdl/verilog.py
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/__init__.py
--rw-r--r--   0        0        0     2536 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/cdc.py
--rw-r--r--   0        0        0      101 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/coding.py
--rw-r--r--   0        0        0     3691 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/fifo.py
--rw-r--r--   0        0        0     7024 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/fsm.py
--rw-r--r--   0        0        0     5953 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/record.py
--rw-r--r--   0        0        0      589 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/resetsync.py
--rw-r--r--   0        0        0     2066 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/genlib/roundrobin.py
--rw-r--r--   0        0        0     1605 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/compat/sim/__init__.py
--rw-r--r--   0        0        0      780 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/__init__.py
--rw-r--r--   0        0        0    11262 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/_rec.py
--rw-r--r--   0        0        0     1113 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/_repr.py
--rw-r--r--   0        0        0    75978 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/ast.py
--rw-r--r--   0        0        0     2911 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/cd.py
--rw-r--r--   0        0        0    22716 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/dsl.py
--rw-r--r--   0        0        0    27124 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/ir.py
--rw-r--r--   0        0        0    14757 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/mem.py
--rw-r--r--   0        0        0      701 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/rec.py
--rw-r--r--   0        0        0    24647 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/hdl/xfrm.py
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/__init__.py
--rw-r--r--   0        0        0    10699 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/cdc.py
--rw-r--r--   0        0        0     4227 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/coding.py
--rw-r--r--   0        0        0    17783 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/crc/__init__.py
--rw-r--r--   0        0        0    20518 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/crc/catalog.py
--rw-r--r--   0        0        0    36040 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/data.py
--rw-r--r--   0        0        0    15883 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/enum.py
--rw-r--r--   0        0        0    23879 2024-03-15 12:12:34.694499 amaranth-0.4.4/amaranth/lib/fifo.py
--rw-r--r--   0        0        0     5708 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/lib/io.py
--rw-r--r--   0        0        0     2090 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/lib/scheduler.py
--rw-r--r--   0        0        0    73107 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/lib/wiring.py
--rw-r--r--   0        0        0     4521 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/rpc.py
--rw-r--r--   0        0        0       94 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/__init__.py
--rw-r--r--   0        0        0     1405 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/_base.py
--rw-r--r--   0        0        0      794 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/_pyclock.py
--rw-r--r--   0        0        0     4792 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/_pycoro.py
--rw-r--r--   0        0        0    18624 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/_pyrtl.py
--rw-r--r--   0        0        0     8192 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/core.py
--rw-r--r--   0        0        0    12336 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/sim/pysim.py
--rw-r--r--   0        0        0     2446 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/tracer.py
--rw-r--r--   0        0        0     1105 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/utils.py
--rw-r--r--   0        0        0     1402 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/__init__.py
--rw-r--r--   0        0        0    21759 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_gowin.py
--rw-r--r--   0        0        0    21256 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_intel.py
--rw-r--r--   0        0        0    26395 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_lattice_ecp5.py
--rw-r--r--   0        0        0    26282 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_lattice_ice40.py
--rw-r--r--   0        0        0    18659 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_lattice_machxo_2_3l.py
--rw-r--r--   0        0        0     6764 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_quicklogic.py
--rw-r--r--   0        0        0    48928 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/_xilinx.py
--rw-r--r--   0        0        0      425 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/gowin.py
--rw-r--r--   0        0        0      425 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/intel.py
--rw-r--r--   0        0        0      431 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/lattice_ecp5.py
--rw-r--r--   0        0        0      432 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/lattice_ice40.py
--rw-r--r--   0        0        0      461 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/lattice_machxo_2_3l.py
--rw-r--r--   0        0        0      430 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/quicklogic.py
--rw-r--r--   0        0        0      426 2024-03-15 12:12:34.698499 amaranth-0.4.4/amaranth/vendor/xilinx.py
--rw-r--r--   0        0        0      608 2024-03-15 12:12:34.702499 amaranth-0.4.4/pdm_build.py
--rw-r--r--   0        0        0     1916 2024-03-15 12:12:42.722461 amaranth-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/__init__.py
--rw-r--r--   0        0        0      445 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/support.py
--rw-r--r--   0        0        0     3656 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_coding.py
--rw-r--r--   0        0        0      961 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_constant.py
--rw-r--r--   0        0        0     1284 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_fifo.py
--rw-r--r--   0        0        0     2770 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_fsm.py
--rw-r--r--   0        0        0      477 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_passive.py
--rw-r--r--   0        0        0      683 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_run_simulation.py
--rw-r--r--   0        0        0     1448 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_signed.py
--rw-r--r--   0        0        0      532 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/compat/test_size.py
--rw-r--r--   0        0        0    12934 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_build_dsl.py
--rw-r--r--   0        0        0     2189 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_build_plat.py
--rw-r--r--   0        0        0    12833 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_build_res.py
--rw-r--r--   0        0        0      224 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_compat.py
--rw-r--r--   0        0        0     1276 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_examples.py
--rw-r--r--   0        0        0    55037 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_ast.py
--rw-r--r--   0        0        0     2784 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_cd.py
--rw-r--r--   0        0        0    27561 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_dsl.py
--rw-r--r--   0        0        0    27423 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_ir.py
--rw-r--r--   0        0        0     5520 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_mem.py
--rw-r--r--   0        0        0    18317 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_rec.py
--rw-r--r--   0        0        0    15982 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_hdl_xfrm.py
--rw-r--r--   0        0        0     8426 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_lib_cdc.py
--rw-r--r--   0        0        0     3654 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_lib_coding.py
--rw-r--r--   0        0        0    13992 2024-03-15 12:12:34.702499 amaranth-0.4.4/tests/test_lib_crc.py
--rw-r--r--   0        0        0    35430 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_data.py
--rw-r--r--   0        0        0    10199 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_enum.py
--rw-r--r--   0        0        0    16077 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_fifo.py
--rw-r--r--   0        0        0     7082 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_io.py
--rw-r--r--   0        0        0     3311 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_scheduler.py
--rw-r--r--   0        0        0    40338 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_lib_wiring.py
--rw-r--r--   0        0        0    42708 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_sim.py
--rw-r--r--   0        0        0     1994 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_tracer.py
--rw-r--r--   0        0        0     2741 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/test_utils.py
--rw-r--r--   0        0        0     2633 2024-03-15 12:12:34.706499 amaranth-0.4.4/tests/utils.py
--rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 amaranth-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1333 2024-04-03 15:35:20.985160 amaranth-0.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     3280 2024-04-03 15:35:20.985160 amaranth-0.4.5/README.md
+-rw-r--r--   0        0        0      908 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/_toolchain/__init__.py
+-rw-r--r--   0        0        0     8475 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/_toolchain/yosys.py
+-rw-r--r--   0        0        0     1459 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/_unused.py
+-rw-r--r--   0        0        0     2942 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/_utils.py
+-rw-r--r--   0        0        0      116 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/asserts.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/back/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/back/cxxrtl.py
+-rw-r--r--   0        0        0    39258 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/back/rtlil.py
+-rw-r--r--   0        0        0     2552 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/back/verilog.py
+-rw-r--r--   0        0        0       70 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/build/__init__.py
+-rw-r--r--   0        0        0    10006 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/build/dsl.py
+-rw-r--r--   0        0        0    20626 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/build/plat.py
+-rw-r--r--   0        0        0    12396 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/build/res.py
+-rw-r--r--   0        0        0    11176 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/build/run.py
+-rw-r--r--   0        0        0     3365 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/cli.py
+-rw-r--r--   0        0        0      257 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/__init__.py
+-rw-r--r--   0        0        0      569 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/bitcontainer.py
+-rw-r--r--   0        0        0     1070 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/conv_output.py
+-rw-r--r--   0        0        0     2122 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/decorators.py
+-rw-r--r--   0        0        0     5206 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/module.py
+-rw-r--r--   0        0        0     5152 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/specials.py
+-rw-r--r--   0        0        0     6169 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/structure.py
+-rw-r--r--   0        0        0     1066 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/fhdl/verilog.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/genlib/__init__.py
+-rw-r--r--   0        0        0     2536 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/genlib/cdc.py
+-rw-r--r--   0        0        0      101 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/genlib/coding.py
+-rw-r--r--   0        0        0     3691 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/genlib/fifo.py
+-rw-r--r--   0        0        0     7024 2024-04-03 15:35:20.985160 amaranth-0.4.5/amaranth/compat/genlib/fsm.py
+-rw-r--r--   0        0        0     5953 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/compat/genlib/record.py
+-rw-r--r--   0        0        0      589 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/compat/genlib/resetsync.py
+-rw-r--r--   0        0        0     2066 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/compat/genlib/roundrobin.py
+-rw-r--r--   0        0        0     1605 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/compat/sim/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/__init__.py
+-rw-r--r--   0        0        0    11262 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/_rec.py
+-rw-r--r--   0        0        0     1113 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/_repr.py
+-rw-r--r--   0        0        0    75978 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/ast.py
+-rw-r--r--   0        0        0     2911 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/cd.py
+-rw-r--r--   0        0        0    22716 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/dsl.py
+-rw-r--r--   0        0        0    27124 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/ir.py
+-rw-r--r--   0        0        0    15059 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/mem.py
+-rw-r--r--   0        0        0      701 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/rec.py
+-rw-r--r--   0        0        0    24647 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/hdl/xfrm.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/__init__.py
+-rw-r--r--   0        0        0    10699 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/cdc.py
+-rw-r--r--   0        0        0     4227 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/coding.py
+-rw-r--r--   0        0        0    17783 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/crc/__init__.py
+-rw-r--r--   0        0        0    20518 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/crc/catalog.py
+-rw-r--r--   0        0        0    36082 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/data.py
+-rw-r--r--   0        0        0    15883 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/enum.py
+-rw-r--r--   0        0        0    23879 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/fifo.py
+-rw-r--r--   0        0        0     5708 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/io.py
+-rw-r--r--   0        0        0     2090 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/scheduler.py
+-rw-r--r--   0        0        0    73107 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/lib/wiring.py
+-rw-r--r--   0        0        0     4521 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/rpc.py
+-rw-r--r--   0        0        0       94 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/__init__.py
+-rw-r--r--   0        0        0     1405 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/_base.py
+-rw-r--r--   0        0        0      794 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/_pyclock.py
+-rw-r--r--   0        0        0     4792 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/_pycoro.py
+-rw-r--r--   0        0        0    18624 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/_pyrtl.py
+-rw-r--r--   0        0        0     8192 2024-04-03 15:35:20.989160 amaranth-0.4.5/amaranth/sim/core.py
+-rw-r--r--   0        0        0    12336 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/sim/pysim.py
+-rw-r--r--   0        0        0     2464 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/tracer.py
+-rw-r--r--   0        0        0     1105 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/utils.py
+-rw-r--r--   0        0        0     1402 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/__init__.py
+-rw-r--r--   0        0        0    21759 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_gowin.py
+-rw-r--r--   0        0        0    21256 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_intel.py
+-rw-r--r--   0        0        0    26395 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_lattice_ecp5.py
+-rw-r--r--   0        0        0    26282 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_lattice_ice40.py
+-rw-r--r--   0        0        0    18659 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_lattice_machxo_2_3l.py
+-rw-r--r--   0        0        0     6764 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_quicklogic.py
+-rw-r--r--   0        0        0    48928 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/_xilinx.py
+-rw-r--r--   0        0        0      425 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/gowin.py
+-rw-r--r--   0        0        0      425 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/intel.py
+-rw-r--r--   0        0        0      431 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/lattice_ecp5.py
+-rw-r--r--   0        0        0      432 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/lattice_ice40.py
+-rw-r--r--   0        0        0      461 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/lattice_machxo_2_3l.py
+-rw-r--r--   0        0        0      430 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/quicklogic.py
+-rw-r--r--   0        0        0      426 2024-04-03 15:35:20.993161 amaranth-0.4.5/amaranth/vendor/xilinx.py
+-rw-r--r--   0        0        0      608 2024-04-03 15:35:20.997161 amaranth-0.4.5/pdm_build.py
+-rw-r--r--   0        0        0     1916 2024-04-03 15:35:26.693141 amaranth-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/__init__.py
+-rw-r--r--   0        0        0      445 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/support.py
+-rw-r--r--   0        0        0     3656 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_coding.py
+-rw-r--r--   0        0        0      961 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_constant.py
+-rw-r--r--   0        0        0     1284 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_fifo.py
+-rw-r--r--   0        0        0     2770 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_fsm.py
+-rw-r--r--   0        0        0      477 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_passive.py
+-rw-r--r--   0        0        0      683 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_run_simulation.py
+-rw-r--r--   0        0        0     1448 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_signed.py
+-rw-r--r--   0        0        0      532 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/compat/test_size.py
+-rw-r--r--   0        0        0    12934 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_build_dsl.py
+-rw-r--r--   0        0        0     2189 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_build_plat.py
+-rw-r--r--   0        0        0    12833 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_build_res.py
+-rw-r--r--   0        0        0      224 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_compat.py
+-rw-r--r--   0        0        0     1276 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_examples.py
+-rw-r--r--   0        0        0    55037 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_ast.py
+-rw-r--r--   0        0        0     2784 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_cd.py
+-rw-r--r--   0        0        0    27561 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_dsl.py
+-rw-r--r--   0        0        0    27423 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_ir.py
+-rw-r--r--   0        0        0     5520 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_mem.py
+-rw-r--r--   0        0        0    18317 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_rec.py
+-rw-r--r--   0        0        0    15982 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_hdl_xfrm.py
+-rw-r--r--   0        0        0     8426 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_cdc.py
+-rw-r--r--   0        0        0     3654 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_coding.py
+-rw-r--r--   0        0        0    13992 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_crc.py
+-rw-r--r--   0        0        0    35430 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_data.py
+-rw-r--r--   0        0        0    10199 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_enum.py
+-rw-r--r--   0        0        0    16077 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_fifo.py
+-rw-r--r--   0        0        0     7082 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_io.py
+-rw-r--r--   0        0        0     3311 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_scheduler.py
+-rw-r--r--   0        0        0    40338 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_lib_wiring.py
+-rw-r--r--   0        0        0    42708 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_sim.py
+-rw-r--r--   0        0        0     2524 2024-04-03 15:35:20.997161 amaranth-0.4.5/tests/test_tracer.py
+-rw-r--r--   0        0        0     2741 2024-04-03 15:35:21.001160 amaranth-0.4.5/tests/test_utils.py
+-rw-r--r--   0        0        0     2633 2024-04-03 15:35:21.001160 amaranth-0.4.5/tests/utils.py
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 amaranth-0.4.5/PKG-INFO
```

### Comparing `amaranth-0.4.4/LICENSE.txt` & `amaranth-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/README.md` & `amaranth-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/__init__.py` & `amaranth-0.4.5/amaranth/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/_toolchain/__init__.py` & `amaranth-0.4.5/amaranth/_toolchain/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/_toolchain/yosys.py` & `amaranth-0.4.5/amaranth/_toolchain/yosys.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/_unused.py` & `amaranth-0.4.5/amaranth/_unused.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/_utils.py` & `amaranth-0.4.5/amaranth/_utils.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/back/cxxrtl.py` & `amaranth-0.4.5/amaranth/back/cxxrtl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/back/rtlil.py` & `amaranth-0.4.5/amaranth/back/rtlil.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/back/verilog.py` & `amaranth-0.4.5/amaranth/back/verilog.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/build/dsl.py` & `amaranth-0.4.5/amaranth/build/dsl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/build/plat.py` & `amaranth-0.4.5/amaranth/build/plat.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/build/res.py` & `amaranth-0.4.5/amaranth/build/res.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/build/run.py` & `amaranth-0.4.5/amaranth/build/run.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/cli.py` & `amaranth-0.4.5/amaranth/cli.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/bitcontainer.py` & `amaranth-0.4.5/amaranth/compat/fhdl/bitcontainer.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/conv_output.py` & `amaranth-0.4.5/amaranth/compat/fhdl/conv_output.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/decorators.py` & `amaranth-0.4.5/amaranth/compat/fhdl/decorators.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/module.py` & `amaranth-0.4.5/amaranth/compat/fhdl/module.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/specials.py` & `amaranth-0.4.5/amaranth/compat/fhdl/specials.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/structure.py` & `amaranth-0.4.5/amaranth/compat/fhdl/structure.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/fhdl/verilog.py` & `amaranth-0.4.5/amaranth/compat/fhdl/verilog.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/cdc.py` & `amaranth-0.4.5/amaranth/compat/genlib/cdc.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/fifo.py` & `amaranth-0.4.5/amaranth/compat/genlib/fifo.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/fsm.py` & `amaranth-0.4.5/amaranth/compat/genlib/fsm.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/record.py` & `amaranth-0.4.5/amaranth/compat/genlib/record.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/resetsync.py` & `amaranth-0.4.5/amaranth/compat/genlib/resetsync.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/genlib/roundrobin.py` & `amaranth-0.4.5/amaranth/compat/genlib/roundrobin.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/compat/sim/__init__.py` & `amaranth-0.4.5/amaranth/compat/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/__init__.py` & `amaranth-0.4.5/amaranth/hdl/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/_rec.py` & `amaranth-0.4.5/amaranth/hdl/_rec.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/_repr.py` & `amaranth-0.4.5/amaranth/hdl/_repr.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/ast.py` & `amaranth-0.4.5/amaranth/hdl/ast.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/cd.py` & `amaranth-0.4.5/amaranth/hdl/cd.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/dsl.py` & `amaranth-0.4.5/amaranth/hdl/dsl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/ir.py` & `amaranth-0.4.5/amaranth/hdl/ir.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/mem.py` & `amaranth-0.4.5/amaranth/hdl/mem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import operator
+import warnings
 from collections import OrderedDict
 
 from .. import tracer
 from .ast import *
 from .ir import Elaboratable, Instance, Fragment
 
 
@@ -112,14 +113,18 @@
         -------
         An instance of :class:`WritePort` associated with this memory.
         """
         return WritePort(self, src_loc_at=1 + src_loc_at, **kwargs)
 
     def __getitem__(self, index):
         """Simulation only."""
+        if not isinstance(index, int):
+            warnings.warn(f"Memory index is {index!r} instead of an 'int'; indexing a memory with "
+                          f"values is deprecated and will be removed in Amaranth 0.5",
+                          DeprecationWarning, stacklevel=2)
         return self._array[index]
 
     def elaborate(self, platform):
         init = "".join(format(Const(elem, unsigned(self.width)).value, f"0{self.width}b") for elem in reversed(self.init))
         init = Const(int(init or "0", 2), self.depth * self.width)
         rd_clk = []
         rd_clk_enable = 0
```

### Comparing `amaranth-0.4.4/amaranth/hdl/rec.py` & `amaranth-0.4.5/amaranth/hdl/rec.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/hdl/xfrm.py` & `amaranth-0.4.5/amaranth/hdl/xfrm.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/cdc.py` & `amaranth-0.4.5/amaranth/lib/cdc.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/coding.py` & `amaranth-0.4.5/amaranth/lib/coding.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/crc/__init__.py` & `amaranth-0.4.5/amaranth/lib/crc/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/crc/catalog.py` & `amaranth-0.4.5/amaranth/lib/crc/catalog.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/data.py` & `amaranth-0.4.5/amaranth/lib/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,23 +797,23 @@
             # be instantiated. It can be used to share behavior.
             return type.__new__(metacls, name, bases, namespace)
         elif all(not hasattr(base, "_AggregateMeta__layout") for base in bases):
             # This is a leaf class with its own layout. It is shape-castable and can
             # be instantiated. It can also be subclassed, and used to share layout and behavior.
             layout  = dict()
             default = dict()
-            for name in {**namespace["__annotations__"]}:
+            for field_name in {**namespace["__annotations__"]}:
                 try:
-                    Shape.cast(namespace["__annotations__"][name])
+                    Shape.cast(namespace["__annotations__"][field_name])
                 except TypeError:
                     # Not a shape-castable annotation; leave as-is.
                     continue
-                layout[name] = namespace["__annotations__"].pop(name)
-                if name in namespace:
-                    default[name] = namespace.pop(name)
+                layout[field_name] = namespace["__annotations__"].pop(field_name)
+                if field_name in namespace:
+                    default[field_name] = namespace.pop(field_name)
             cls = type.__new__(metacls, name, bases, namespace)
             if cls.__layout_cls is UnionLayout:
                 if len(default) > 1:
                     raise ValueError("Reset value for at most one field can be provided for "
                                      "a union class (specified: {})"
                                      .format(", ".join(default.keys())))
             cls.__layout  = cls.__layout_cls(layout)
```

### Comparing `amaranth-0.4.4/amaranth/lib/enum.py` & `amaranth-0.4.5/amaranth/lib/enum.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/fifo.py` & `amaranth-0.4.5/amaranth/lib/fifo.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/io.py` & `amaranth-0.4.5/amaranth/lib/io.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/scheduler.py` & `amaranth-0.4.5/amaranth/lib/scheduler.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/lib/wiring.py` & `amaranth-0.4.5/amaranth/lib/wiring.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/rpc.py` & `amaranth-0.4.5/amaranth/rpc.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/_base.py` & `amaranth-0.4.5/amaranth/sim/_base.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/_pyclock.py` & `amaranth-0.4.5/amaranth/sim/_pyclock.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/_pycoro.py` & `amaranth-0.4.5/amaranth/sim/_pycoro.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/_pyrtl.py` & `amaranth-0.4.5/amaranth/sim/_pyrtl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/core.py` & `amaranth-0.4.5/amaranth/sim/core.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/sim/pysim.py` & `amaranth-0.4.5/amaranth/sim/pysim.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/tracer.py` & `amaranth-0.4.5/amaranth/tracer.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     while True:
         call_opc = opname[code.co_code[call_index]]
         if call_opc in ("EXTENDED_ARG",):
             call_index += 2
         else:
             break
     if call_opc not in ("CALL_FUNCTION", "CALL_FUNCTION_KW", "CALL_FUNCTION_EX",
-                        "CALL_METHOD", "CALL", "CALL_KW"):
+                        "CALL_METHOD", "CALL_METHOD_KW", "CALL", "CALL_KW"):
         if default is _raise_exception:
             raise NameNotFound
         else:
             return default
 
     index = call_index + 2
     imm = 0
```

### Comparing `amaranth-0.4.4/amaranth/utils.py` & `amaranth-0.4.5/amaranth/utils.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/__init__.py` & `amaranth-0.4.5/amaranth/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_gowin.py` & `amaranth-0.4.5/amaranth/vendor/_gowin.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_intel.py` & `amaranth-0.4.5/amaranth/vendor/_intel.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_lattice_ecp5.py` & `amaranth-0.4.5/amaranth/vendor/_lattice_ecp5.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_lattice_ice40.py` & `amaranth-0.4.5/amaranth/vendor/_lattice_ice40.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_lattice_machxo_2_3l.py` & `amaranth-0.4.5/amaranth/vendor/_lattice_machxo_2_3l.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_quicklogic.py` & `amaranth-0.4.5/amaranth/vendor/_quicklogic.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/amaranth/vendor/_xilinx.py` & `amaranth-0.4.5/amaranth/vendor/_xilinx.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/pdm_build.py` & `amaranth-0.4.5/pdm_build.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/pyproject.toml` & `amaranth-0.4.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 requires-python = "~=3.8"
 dependencies = [
     "importlib_resources; python_version<'3.9'",
     "pyvcd>=0.2.2,<0.5",
     "Jinja2~=3.0",
 ]
-version = "0.4.4"
+version = "0.4.5"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 builtin-yosys = [
     "amaranth-yosys>=0.38",
@@ -79,15 +79,15 @@
 ]
 
 [project.scripts]
 amaranth-rpc = "amaranth.rpc:main"
 
 [project.urls]
 Homepage = "https://amaranth-lang.org/"
-Documentation = "https://amaranth-lang.org/docs/amaranth/v0.4.4"
+Documentation = "https://amaranth-lang.org/docs/amaranth/v0.4.5"
 "Source Code" = "https://github.com/amaranth-lang/amaranth"
 "Bug Tracker" = "https://github.com/amaranth-lang/amaranth/issues"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `amaranth-0.4.4/tests/compat/test_coding.py` & `amaranth-0.4.5/tests/compat/test_coding.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_constant.py` & `amaranth-0.4.5/tests/compat/test_constant.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_fifo.py` & `amaranth-0.4.5/tests/compat/test_fifo.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_fsm.py` & `amaranth-0.4.5/tests/compat/test_fsm.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_run_simulation.py` & `amaranth-0.4.5/tests/compat/test_run_simulation.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_signed.py` & `amaranth-0.4.5/tests/compat/test_signed.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/compat/test_size.py` & `amaranth-0.4.5/tests/compat/test_size.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_build_dsl.py` & `amaranth-0.4.5/tests/test_build_dsl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_build_plat.py` & `amaranth-0.4.5/tests/test_build_plat.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_build_res.py` & `amaranth-0.4.5/tests/test_build_res.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_examples.py` & `amaranth-0.4.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_ast.py` & `amaranth-0.4.5/tests/test_hdl_ast.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_cd.py` & `amaranth-0.4.5/tests/test_hdl_cd.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_dsl.py` & `amaranth-0.4.5/tests/test_hdl_dsl.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_ir.py` & `amaranth-0.4.5/tests/test_hdl_ir.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_mem.py` & `amaranth-0.4.5/tests/test_hdl_mem.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_rec.py` & `amaranth-0.4.5/tests/test_hdl_rec.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_hdl_xfrm.py` & `amaranth-0.4.5/tests/test_hdl_xfrm.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_cdc.py` & `amaranth-0.4.5/tests/test_lib_cdc.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_coding.py` & `amaranth-0.4.5/tests/test_lib_coding.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_crc.py` & `amaranth-0.4.5/tests/test_lib_crc.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_data.py` & `amaranth-0.4.5/tests/test_lib_data.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_enum.py` & `amaranth-0.4.5/tests/test_lib_enum.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_fifo.py` & `amaranth-0.4.5/tests/test_lib_fifo.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_io.py` & `amaranth-0.4.5/tests/test_lib_io.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_scheduler.py` & `amaranth-0.4.5/tests/test_lib_scheduler.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_lib_wiring.py` & `amaranth-0.4.5/tests/test_lib_wiring.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_sim.py` & `amaranth-0.4.5/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/test_tracer.py` & `amaranth-0.4.5/tests/test_tracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 from amaranth.hdl.ast import *
+from amaranth.hdl import ast
 from types import SimpleNamespace
 
 from .utils import *
 
 class TracerTestCase(FHDLTestCase):
     def test_fast(self):
         s1 = Signal()
         self.assertEqual(s1.name, "s1")
         s2 = Signal()
         self.assertEqual(s2.name, "s2")
 
+    def test_call_variants(self):
+        args = []
+        kwargs = {}
+        s1 = Signal()
+        self.assertEqual(s1.name, "s1")
+        s2 = Signal(reset=0)
+        self.assertEqual(s2.name, "s2")
+        s3 = Signal(*args, **kwargs)
+        self.assertEqual(s3.name, "s3")
+        s4 = ast.Signal()
+        self.assertEqual(s4.name, "s4")
+        s5 = ast.Signal(reset=0)
+        self.assertEqual(s5.name, "s5")
+        s6 = ast.Signal(*args, **kwargs)
+        self.assertEqual(s6.name, "s6")
+
     def test_name(self):
         class Dummy:
             s1 = Signal()
             self.assertEqual(s1.name, "s1")
             s2 = Signal()
             self.assertEqual(s2.name, "s2")
```

### Comparing `amaranth-0.4.4/tests/test_utils.py` & `amaranth-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/tests/utils.py` & `amaranth-0.4.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `amaranth-0.4.4/PKG-INFO` & `amaranth-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amaranth
-Version: 0.4.4
+Version: 0.4.5
 Summary: Amaranth hardware definition language
 Author: Amaranth HDL contributors
 License: Copyright (C) 2019-2023 Amaranth HDL contributors
         Copyright (C) 2011-2019 M-Labs Limited
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -22,15 +22,15 @@
         ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
         (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
         LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
         ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Homepage, https://amaranth-lang.org/
-Project-URL: Documentation, https://amaranth-lang.org/docs/amaranth/v0.4.4
+Project-URL: Documentation, https://amaranth-lang.org/docs/amaranth/v0.4.5
 Project-URL: Source code, https://github.com/amaranth-lang/amaranth
 Project-URL: Bug tracker, https://github.com/amaranth-lang/amaranth/issues
 Requires-Python: ~=3.8
 Requires-Dist: importlib_resources; python_version < "3.9"
 Requires-Dist: pyvcd<0.5,>=0.2.2
 Requires-Dist: Jinja2~=3.0
 Requires-Dist: amaranth-yosys>=0.38; extra == "builtin-yosys"
```

