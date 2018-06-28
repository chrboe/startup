# Versions

```shell
$ go version
go version go1.10.3 linux/amd64
```

# Benchmark command

```shell
$ go build     # (not measured)
$ perf stat -r 100 ./go 2> results.txt
```
