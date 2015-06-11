## Runtime ##

Experiments were run on a machine with 2 Quad-core Xeon 2.33 GHz CPUs running Ubuntu Linux 2.6.32-31 with 16 GB RAM.

| **Experiment** | **Runtime (hrs)** | **Memory Usage (MB)** |
|:---------------|:------------------|:----------------------|
|One-way TCP Lossy, FIN 1 sec	| 9.39              | 14325.80              |
|One-way TCP Lossless, FIN 1 sec	| 9.55              | 14519.95              |
|One-way TCP Lossless, FIN 100 ms	| 9.03              | 11534.73              |
|One-way TCP Lossless, FIN 10 ms	| 8.33              | 9473.75               |
|Full-TCP Lossy, FIN 1 sec		| 2.43              | 676.98                |
|Full-TCP Lossless, FIN 1 sec	| 2.39              | 674.64                |
|Full-TCP Lossless, FIN 100 ms	| 2.38              | 672.64                |
|Full-TCP Lossless, FIN 10 ms	| 2.37              | 672.12                |

![http://tmix-ns2.googlecode.com/svn/wiki/ns2-graphs/runtimes/runtimes.png](http://tmix-ns2.googlecode.com/svn/wiki/ns2-graphs/runtimes/runtimes.png)