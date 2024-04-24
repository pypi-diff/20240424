# Comparing `tmp/splat64-0.24.0.tar.gz` & `tmp/splat64-0.24.1.tar.gz`

## Comparing `splat64-0.24.0.tar` & `splat64-0.24.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0    50026 2020-02-02 00:00:00.000000 splat64-0.24.0/CHANGELOG.md
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 splat64-0.24.0/create_config.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 splat64-0.24.0/mypy.ini
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 splat64-0.24.0/requirements.txt
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 splat64-0.24.0/split.py
--rwxr-xr-x   0        0        0    16295 2020-02-02 00:00:00.000000 splat64-0.24.0/test.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/black.yml
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/publish_docs_to_wiki.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/test_lib.yml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 splat64-0.24.0/.github/workflows/unit_tests.yml
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Adding-Symbols.md
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Advanced.md
--rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Configuration.md
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Examples.md
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/General-Workflow.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Home.md
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Quickstart.md
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/Segments.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 splat64-0.24.0/docs/VramClasses.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/py.typed
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/disassembler.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/disassembler_instance.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/disassembler_section.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/null_disassembler.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/disassembler/spimdisasm_disassembler.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/platforms/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/platforms/n64.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/platforms/ps2.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/platforms/psp.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/platforms/psx.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/scripts/__init__.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/scripts/capy.py
--rw-r--r--   0        0        0     6634 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/scripts/create_config.py
--rw-r--r--   0        0        0    20351 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/scripts/split.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/__init__.py
--rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/linker_entry.py
--rw-r--r--   0        0        0    25214 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/segment.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/__init__.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/asm.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/bin.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/bss.py
--rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/c.py
--rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/code.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/codesubsegment.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/cpp.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/data.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/databin.py
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/group.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/hasm.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/header.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/lib.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/pad.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/rdata.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/rodata.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/rodatabin.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/sbss.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/sdata.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/segment.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/common/textbin.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/asm.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ci.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ci4.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ci8.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/decompressor.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/gfx.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/hasm.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/header.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/i1.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/i4.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/i8.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ia16.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ia4.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ia8.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/img.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/ipl3.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/linker_offset.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/mio0.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/palette.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/rgba16.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/rgba32.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/rsp.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/segment.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/vtx.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/n64/yay0.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/asm.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/ctor.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/lit4.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/lit8.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/ps2/vtables.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psp/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psp/segment.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psx/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psx/asm.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psx/header.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/segtypes/psx/segment.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/cache_handler.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/color.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/compiler.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/log.py
--rw-r--r--   0        0        0    25718 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/options.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/palettes.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/progress_bar.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/relocs.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/statistics.py
--rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/symbols.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/vram_classes.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/n64/__init__.py
--rwxr-xr-x   0        0        0     1414 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/n64/find_code_length.py
--rwxr-xr-x   0        0        0     9046 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/n64/rominfo.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/psx/__init__.py
--rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 splat64-0.24.0/src/splat/util/psx/psxexeinfo.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 splat64-0.24.0/test/Dockerfile
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 splat64-0.24.0/test/README.md
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 splat64-0.24.0/test/test_gen_expected.sh
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/.gitignore
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/Makefile
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/dummy_ipl3.s
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/handwritten.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/header.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/main.c
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/.splache
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/undefined_funcs_auto.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/undefined_syms_auto.txt
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/handwritten.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/header.s
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/data/main.bss.s
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/data/main.data.s
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/nonmatchings/main/D_80000510.s
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/assets/dummy_ipl3.bin
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 splat64-0.24.0/test/basic_app/expected/src/main.c
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 splat64-0.24.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 splat64-0.24.0/LICENSE
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 splat64-0.24.0/README.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 splat64-0.24.0/pyproject.toml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 splat64-0.24.0/PKG-INFO
+-rw-r--r--   0        0        0    50176 2020-02-02 00:00:00.000000 splat64-0.24.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 splat64-0.24.1/create_config.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 splat64-0.24.1/mypy.ini
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 splat64-0.24.1/requirements.txt
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 splat64-0.24.1/split.py
+-rwxr-xr-x   0        0        0    16295 2020-02-02 00:00:00.000000 splat64-0.24.1/test.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/publish_docs_to_wiki.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/test_lib.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 splat64-0.24.1/.github/workflows/unit_tests.yml
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Adding-Symbols.md
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Advanced.md
+-rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Configuration.md
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Examples.md
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/General-Workflow.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Home.md
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Quickstart.md
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/Segments.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 splat64-0.24.1/docs/VramClasses.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/py.typed
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/disassembler.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/disassembler_instance.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/disassembler_section.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/null_disassembler.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/disassembler/spimdisasm_disassembler.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/platforms/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/platforms/n64.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/platforms/ps2.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/platforms/psp.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/platforms/psx.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/scripts/__init__.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/scripts/capy.py
+-rw-r--r--   0        0        0     6634 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/scripts/create_config.py
+-rw-r--r--   0        0        0    20351 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/scripts/split.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/__init__.py
+-rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/linker_entry.py
+-rw-r--r--   0        0        0    25214 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/segment.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/__init__.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/asm.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/bin.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/bss.py
+-rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/c.py
+-rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/code.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/codesubsegment.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/cpp.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/data.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/databin.py
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/group.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/hasm.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/header.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/lib.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/pad.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/rdata.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/rodata.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/rodatabin.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/sbss.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/sdata.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/segment.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/common/textbin.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/asm.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ci.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ci4.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ci8.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/decompressor.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/gfx.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/hasm.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/header.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/i1.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/i4.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/i8.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ia16.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ia4.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ia8.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/img.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/ipl3.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/linker_offset.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/mio0.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/palette.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/rgba16.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/rgba32.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/rsp.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/segment.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/vtx.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/n64/yay0.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/asm.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/ctor.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/lit4.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/lit8.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/ps2/vtables.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psp/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psp/segment.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psx/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psx/asm.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psx/header.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/segtypes/psx/segment.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/cache_handler.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/color.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/compiler.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/log.py
+-rw-r--r--   0        0        0    25718 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/options.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/palettes.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/progress_bar.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/relocs.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/statistics.py
+-rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/symbols.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/vram_classes.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/n64/__init__.py
+-rwxr-xr-x   0        0        0     1414 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/n64/find_code_length.py
+-rwxr-xr-x   0        0        0     9046 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/n64/rominfo.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/psx/__init__.py
+-rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 splat64-0.24.1/src/splat/util/psx/psxexeinfo.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 splat64-0.24.1/test/Dockerfile
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 splat64-0.24.1/test/README.md
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 splat64-0.24.1/test/test_gen_expected.sh
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/.gitignore
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/Makefile
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/dummy_ipl3.s
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/handwritten.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/header.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/main.c
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/.splache
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/undefined_funcs_auto.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/undefined_syms_auto.txt
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/handwritten.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/header.s
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/data/main.bss.s
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/data/main.data.s
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/nonmatchings/main/D_80000510.s
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/assets/dummy_ipl3.bin
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 splat64-0.24.1/test/basic_app/expected/src/main.c
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 splat64-0.24.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 splat64-0.24.1/LICENSE
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 splat64-0.24.1/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 splat64-0.24.1/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 splat64-0.24.1/PKG-INFO
```

### Comparing `splat64-0.24.0/CHANGELOG.md` & `splat64-0.24.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # splat Release Notes
 
+### 0.24.1
+
+* Tweak the disassembler's configuration for PSP platform to improve assembly analysis.
+  * Should improve function start/end detection.
+
 ### 0.24.0
 
 * Added PSP as a new platform.
 * `spimdisasm` 1.25.0 or above is now required
 * `rabbitizer` 1.10.0 or above is now required
 
 ### 0.23.2
```

### Comparing `splat64-0.24.0/test.py` & `splat64-0.24.1/test.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/.github/workflows/mypy.yml` & `splat64-0.24.1/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/.github/workflows/publish_docs_to_wiki.yml` & `splat64-0.24.1/.github/workflows/publish_docs_to_wiki.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/.github/workflows/pypi.yml` & `splat64-0.24.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/.github/workflows/unit_tests.yml` & `splat64-0.24.1/.github/workflows/unit_tests.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Adding-Symbols.md` & `splat64-0.24.1/docs/Adding-Symbols.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Configuration.md` & `splat64-0.24.1/docs/Configuration.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Examples.md` & `splat64-0.24.1/docs/Examples.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/General-Workflow.md` & `splat64-0.24.1/docs/General-Workflow.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Home.md` & `splat64-0.24.1/docs/Home.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Quickstart.md` & `splat64-0.24.1/docs/Quickstart.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/Segments.md` & `splat64-0.24.1/docs/Segments.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/docs/VramClasses.md` & `splat64-0.24.1/docs/VramClasses.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/__main__.py` & `splat64-0.24.1/src/splat/__main__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/disassembler/disassembler_instance.py` & `splat64-0.24.1/src/splat/disassembler/disassembler_instance.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/disassembler/disassembler_section.py` & `splat64-0.24.1/src/splat/disassembler/disassembler_section.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/disassembler/spimdisasm_disassembler.py` & `splat64-0.24.1/src/splat/disassembler/spimdisasm_disassembler.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/scripts/capy.py` & `splat64-0.24.1/src/splat/scripts/capy.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/scripts/create_config.py` & `splat64-0.24.1/src/splat/scripts/create_config.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/scripts/split.py` & `splat64-0.24.1/src/splat/scripts/split.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/linker_entry.py` & `splat64-0.24.1/src/splat/segtypes/linker_entry.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/segment.py` & `splat64-0.24.1/src/splat/segtypes/segment.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/__init__.py` & `splat64-0.24.1/src/splat/segtypes/common/__init__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/asm.py` & `splat64-0.24.1/src/splat/segtypes/common/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/bin.py` & `splat64-0.24.1/src/splat/segtypes/common/bin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/bss.py` & `splat64-0.24.1/src/splat/segtypes/common/bss.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/c.py` & `splat64-0.24.1/src/splat/segtypes/common/c.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/code.py` & `splat64-0.24.1/src/splat/segtypes/common/code.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/codesubsegment.py` & `splat64-0.24.1/src/splat/segtypes/common/codesubsegment.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/data.py` & `splat64-0.24.1/src/splat/segtypes/common/data.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/databin.py` & `splat64-0.24.1/src/splat/segtypes/common/databin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/group.py` & `splat64-0.24.1/src/splat/segtypes/common/group.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/hasm.py` & `splat64-0.24.1/src/splat/segtypes/common/hasm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/header.py` & `splat64-0.24.1/src/splat/segtypes/common/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/lib.py` & `splat64-0.24.1/src/splat/segtypes/common/lib.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/pad.py` & `splat64-0.24.1/src/splat/segtypes/common/pad.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/rodata.py` & `splat64-0.24.1/src/splat/segtypes/common/rodata.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/rodatabin.py` & `splat64-0.24.1/src/splat/segtypes/common/rodatabin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/common/textbin.py` & `splat64-0.24.1/src/splat/segtypes/common/textbin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/__init__.py` & `splat64-0.24.1/src/splat/segtypes/n64/__init__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/asm.py` & `splat64-0.24.1/src/splat/segtypes/n64/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/ci.py` & `splat64-0.24.1/src/splat/segtypes/n64/ci.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/decompressor.py` & `splat64-0.24.1/src/splat/segtypes/n64/decompressor.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/gfx.py` & `splat64-0.24.1/src/splat/segtypes/n64/gfx.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/hasm.py` & `splat64-0.24.1/src/splat/segtypes/n64/hasm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/header.py` & `splat64-0.24.1/src/splat/segtypes/n64/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/img.py` & `splat64-0.24.1/src/splat/segtypes/n64/img.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/linker_offset.py` & `splat64-0.24.1/src/splat/segtypes/n64/linker_offset.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/palette.py` & `splat64-0.24.1/src/splat/segtypes/n64/palette.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/n64/vtx.py` & `splat64-0.24.1/src/splat/segtypes/n64/vtx.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/ps2/asm.py` & `splat64-0.24.1/src/splat/segtypes/ps2/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/ps2/ctor.py` & `splat64-0.24.1/src/splat/segtypes/ps2/ctor.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/ps2/lit4.py` & `splat64-0.24.1/src/splat/segtypes/ps2/lit4.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/ps2/lit8.py` & `splat64-0.24.1/src/splat/segtypes/ps2/lit8.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/ps2/vtables.py` & `splat64-0.24.1/src/splat/segtypes/ps2/vtables.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/psx/asm.py` & `splat64-0.24.1/src/splat/segtypes/psx/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/segtypes/psx/header.py` & `splat64-0.24.1/src/splat/segtypes/psx/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/cache_handler.py` & `splat64-0.24.1/src/splat/util/cache_handler.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/compiler.py` & `splat64-0.24.1/src/splat/util/compiler.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/log.py` & `splat64-0.24.1/src/splat/util/log.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/options.py` & `splat64-0.24.1/src/splat/util/options.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/palettes.py` & `splat64-0.24.1/src/splat/util/palettes.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/relocs.py` & `splat64-0.24.1/src/splat/util/relocs.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/statistics.py` & `splat64-0.24.1/src/splat/util/statistics.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/symbols.py` & `splat64-0.24.1/src/splat/util/symbols.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/vram_classes.py` & `splat64-0.24.1/src/splat/util/vram_classes.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/n64/find_code_length.py` & `splat64-0.24.1/src/splat/util/n64/find_code_length.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/n64/rominfo.py` & `splat64-0.24.1/src/splat/util/n64/rominfo.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/src/splat/util/psx/psxexeinfo.py` & `splat64-0.24.1/src/splat/util/psx/psxexeinfo.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/README.md` & `splat64-0.24.1/test/README.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/Makefile` & `splat64-0.24.1/test/basic_app/Makefile`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/header.s` & `splat64-0.24.1/test/basic_app/header.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/main.c` & `splat64-0.24.1/test/basic_app/main.c`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/expected/.splache` & `splat64-0.24.1/test/basic_app/expected/.splache`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/expected/asm/handwritten.s` & `splat64-0.24.1/test/basic_app/expected/asm/handwritten.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/expected/asm/header.s` & `splat64-0.24.1/test/basic_app/expected/asm/header.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s` & `splat64-0.24.1/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s` & `splat64-0.24.1/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/LICENSE` & `splat64-0.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splat64-0.24.0/README.md` & `splat64-0.24.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 The brackets corresponds to the optional dependencies to install while installing splat. Refer to [Optional dependencies](#optional-dependencies) to see the list of available groups.
 
 If you use a `requirements.txt` file in your repository, then you can add this library with the following line:
 
 ```txt
-splat64[mips]>=0.24.0,<1.0.0
+splat64[mips]>=0.24.1,<1.0.0
 ```
 
 ### Optional dependencies
 
 - `mips`: Required when using the N64, PSX, PS2 or PSp platforms.
 - `dev`: Installs all the available dependencies groups and other packages for development.
```

### Comparing `splat64-0.24.0/pyproject.toml` & `splat64-0.24.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "splat64"
 # Should be synced with src/splat/__init__.py
-version = "0.24.0"
+version = "0.24.1"
 description = "A binary splitting tool to assist with decompilation and modding projects"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `splat64-0.24.0/PKG-INFO` & `splat64-0.24.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: splat64
-Version: 0.24.0
+Version: 0.24.1
 Summary: A binary splitting tool to assist with decompilation and modding projects
 Project-URL: Repository, https://github.com/ethteck/splat
 Project-URL: Issues, https://github.com/ethteck/splat/issues
 Project-URL: Changelog, https://github.com/ethteck/splat/blob/master/CHANGELOG.md
 License: MIT License
         
         Copyright (c) 2021 Ethan Roseman
@@ -72,15 +72,15 @@
 ```
 
 The brackets corresponds to the optional dependencies to install while installing splat. Refer to [Optional dependencies](#optional-dependencies) to see the list of available groups.
 
 If you use a `requirements.txt` file in your repository, then you can add this library with the following line:
 
 ```txt
-splat64[mips]>=0.24.0,<1.0.0
+splat64[mips]>=0.24.1,<1.0.0
 ```
 
 ### Optional dependencies
 
 - `mips`: Required when using the N64, PSX, PS2 or PSp platforms.
 - `dev`: Installs all the available dependencies groups and other packages for development.
```

