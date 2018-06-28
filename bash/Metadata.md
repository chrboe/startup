# Versions

```shell
$ bash --version
GNU bash, version 4.4.23(1)-release (x86_64-pc-linux-gnu)
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>

This is free software; you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
```

# Benchmark command

```shell
$ perf stat -r 100 bash main.sh 2> results.txt
```
