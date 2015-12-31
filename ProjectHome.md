`thriftbench` is a benchmarking utility like `http_load` for Thrift services. It is written in Python and expects a Python client for the thrift service to benchmark. The service itself could be in any language.

Here's a sample run:
```
$ ./thriftbench -h localhost:9090 -s HelloService -t 10 -d 10 ~/calllist 
     sayHello: 002454 fetches (244.957372/sec). 00000 errors. 40.81 ms
(avg). 39.00 ms (50th %ile). 62.16 ms (90th %ile).  4.51 ms
(min). 249.13 ms (max) 
```

`thriftbench` was originally implemented in [Lulu India](http://lulu.com)