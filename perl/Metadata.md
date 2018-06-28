# Versions

```shell
$ perl --version

This is perl 5, version 26, subversion 2 (v5.26.2) built for x86_64-linux
(with 28 registered patches, see perl -V for more detail)

Copyright 1987-2018, Larry Wall

Perl may be copied only under the terms of either the Artistic License or the
GNU General Public License, which may be found in the Perl 5 source kit.

Complete documentation for Perl, including FAQ lists, should be found on
this system using "man perl" or "perldoc perl".  If you have access to the
Internet, point your browser at http://www.perl.org/, the Perl Home Page.
```

# Benchmark command

```shell
$ perf stat -r 100 perl main.pl 2> results.txt
```
