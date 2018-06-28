# Versions

* glibc version 2.27-r5

```shell
$ gcc -v
Using built-in specs.
COLLECT_GCC=gcc
COLLECT_LTO_WRAPPER=/usr/libexec/gcc/x86_64-pc-linux-gnu/7.3.0/lto-wrapper
Target: x86_64-pc-linux-gnu
Configured with: /var/tmp/portage/sys-devel/gcc-7.3.0-r3/work/gcc-7.3.0/configure --host=x86_64-pc-linux-gnu --build=x86_64-pc-linux-gnu --prefix=/usr --bindir=/usr/x86_64-pc-linux-gnu/gcc-bin/7.3.0 --includedir=/usr/lib/gcc/x86_64-pc-linux-gnu/7.3.0/include --datadir=/usr/share/gcc-data/x86_64-pc-linux-gnu/7.3.0 --mandir=/usr/share/gcc-data/x86_64-pc-linux-gnu/7.3.0/man --infodir=/usr/share/gcc-data/x86_64-pc-linux-gnu/7.3.0/info --with-gxx-include-dir=/usr/lib/gcc/x86_64-pc-linux-gnu/7.3.0/include/g++-v7 --with-python-dir=/share/gcc-data/x86_64-pc-linux-gnu/7.3.0/python --enable-languages=c,c++,fortran --enable-obsolete --enable-secureplt --disable-werror --with-system-zlib --disable-nls --enable-checking=release --with-bugurl=https://bugs.gentoo.org/ --with-pkgversion='Gentoo 7.3.0-r3 p1.4' --disable-esp --enable-libstdcxx-time --enable-shared --enable-threads=posix --enable-__cxa_atexit --enable-clocale=gnu --enable-multilib --with-multilib-list=m32,m64 --disable-altivec --disable-fixed-point --enable-targets=all --disable-libgcj --enable-libgomp --disable-libmudflap --disable-libssp --disable-libcilkrts --disable-libmpx --enable-vtable-verify --enable-libvtv --enable-lto --without-isl --enable-libsanitizer --enable-default-pie --enable-default-ssp
Thread model: posix
gcc version 7.3.0 (Gentoo 7.3.0-r3 p1.4)

$ file a.out
a.out: ELF 64-bit LSB pie executable x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, with debug_info, not stripped
```

# Benchmark command

```shell
$ gcc main.c     # (not measured)
$ perf stat -r 100 ./a.out 2> results.txt
```
