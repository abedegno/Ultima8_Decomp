# Ultima 8 Decompile

This working copy adapts [Kitrinx/Ultima8_Decomp](https://github.com/Kitrinx/Ultima8_Decomp) to the GOG DOS 2.13 executable (`Nov 18 1995`, `10:28:46`). The upstream project recovered the source structure and most names from retail debug information; helper libraries and the DOS extender remain binary.

The C, C++, and assembly sources rebuild with Borland C++ 3.1 and the Phar Lap 286 SDK. With `--strip-tdinfo`, the resulting `out/U8.EXE` is byte-for-byte identical to the supplied GOG executable. The unstripped linker output is preserved as `out/U8-TDINFO.EXE` for debugging. See `BUILD.md` for the reproducible build.