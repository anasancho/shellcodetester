# Shellcode Tester

[![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml)
[![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml)
[![Downloads](https://pepy.tech/badge/shellcodetester/month)](https://pepy.tech/project/shellcodetester)
[![Supported Versions](https://img.shields.io/pypi/pyversions/shellcodetester.svg)](https://pypi.org/project/shellcodetester)
[![Contributors](https://img.shields.io/github/contributors/helviojunior/shellcodetester.svg)](https://github.com/helviojunior/shellcodetester/graphs/contributors)
[![PyPI version](https://img.shields.io/pypi/v/shellcodetester.svg)](https://pypi.org/project/shellcodetester/)
[![License: GPL-3.0](https://img.shields.io/pypi/l/shellcodetester.svg)](https://github.com/helviojunior/shellcodetester/blob/master/LICENSE)

ShellcodeTester officially supports Python 3.8+.

## Main features

* [x] Assembly ASM file (32 and 64 bits)
* [x] Assembly ASM file to Windows, Linux and MacOS
* [x] Check badchars
* [x] Output to several formats
* [x] Other amazing features...

## Getting stats

```bash
shellcodetester -asm file.asm
```

This command will assembly the ASM file and compile an ELF binary

```bash

ShellcodeTester v0.2.0 by Helvio Junior (M4v3r1ck)
ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
https://github.com/helviojunior/shellcodetester

 [+] Startup parameters
     command line: shellcodetester -asm test_linux.asm
     log level: NOTSET
     transform format: RAW
     bad chars: 0x00

 [+] start time 2023-02-12 01:53:56
 [+] Assembling x86 file teste_linux.asm to /home/shellcodetester/st_test_linux.o
 [+] Compiling x86 binary to /home/shellcodetester/st_test_linux.elf32
 [+] Payload size: 65 bytes
 [+] Final size of RAW data: 160 bytes
31c0b00431dbb301eb1259ba00000000b220cd8031c0b00131dbcd80e8e9ffffff4c616220303120636f6d706c657461646f20636f6d207375636573736f210a00

 [+] End time 2023-02-12 01:53:56

```

## Installation

```bash
pip3 install --upgrade shellcodetester
```

# Help

```bash
$ shellcodetester -h

ShellcodeTester v0.2.0 by Helvio Junior (M4v3r1ck)
ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
https://github.com/helviojunior/shellcodetester

options:
  -h, --help                      show this help message and exit

General Setting:
  -asm [ASM file name]            Assembly file to be assembled
  -o [output file]                Save output to disk (default: none)

Custom Settings:
  --break-point                   Set software breakpoint (INT3) before shellcode (default: false)
  --bad-chars [bad char list]     List of bad chars to highlight (ex: \x00\x0a, default: \0x00)
  --fill-with-nop                 Fill entire page with NOP (default: false)
  --list                          List all supported output format
  -f [format], --format [format]  Output format (use --list formats to list)
  -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
```

# Windows Users

Check specific instructions by Windows Users

[Windows Instructions](WINDOWS.md)