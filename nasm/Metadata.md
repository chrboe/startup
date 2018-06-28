# Versions

```shell
$ nasm -v
NASM version 2.13.03 compiled on May 14 2018

$ file a.out
a.out: ELF 64-bit LSB executable, x86-64, version 1 (SYSV), statically linked, not stripped
```

# Benchmark command

```shell
$ nasm -f elf64 main.s     # (not measured)
$ ld main.o                # (not measured)
$ perf stat -r 100 ./a.out 2> results.txt
```
