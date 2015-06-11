### Overview ###

The validation experiments used the [connection vectors from our CCR 2006 paper](http://code.google.com/p/tmix-ns2/downloads/detail?name=ccr06-traces.tgz) (src direction uses outbound.cvec, dst direction uses inbound.cvec).  The TCL script used is [tmix.tcl](http://code.google.com/p/tmix-ns2/downloads/detail?name=tmix.tcl).

Experiment topology:

<img src='http://www.cs.odu.edu/~inets/files/tmix-fig.jpg' alt='' width='400'>

We ran 8 experiments, each run for 3600 seconds:<br>
<ul><li>one-way TCP lossy, FIN 1 s<br>
</li><li>one-way TCP lossless, FIN 1 s<br>
</li><li>one-way TCP lossless, FIN 100 ms<br>
</li><li>one-way TCP lossless, FIN 10 ms<br>
</li><li>Full-TCP lossy, FIN 1 s<br>
</li><li>Full-TCP lossless, FIN 1 s<br>
</li><li>Full-TCP lossless, FIN 100 ms<br>
</li><li>Full-TCP lossless, FIN 10 ms</li></ul>

<h3>FIN Wait Times</h3>
For many connection vectors, there was no TCP FIN packet recorded, so we do not know exactly when the connection was completed.  For many metrics, we need to know the duration of the connection.  For those connections that do not have a FIN, we inserted an artificial FIN.<br>
<br>
The FIN time (1 sec, 100 ms, 10 ms) in the experiment indicates the time between when the last data unit was sent and the sending of the artificial FIN.  Shorter FIN times result in shorter connections, lower active connections, and faster runtimes.<br>
<br>
The impact of the artificial FIN is most apparent for one-way TCP.  Waiting longer before sending the artificial FIN ensures that all packets in the connection have been received before the TCP connection closes, producing results that more closely match the original and testbed.  The tradeoff is that the running time and memory usage are increased.  We show all results so that users are aware of the tradeoff.  The default value for the FIN wait time is 1 second.<br>
<br>
<h3>Graphs</h3>

Each set of graphs (except runtime) includes the following metrics:<br>
<ul><li>number of active connections each second<br>
</li><li>CDF of goodput for each completed connection<br>
</li><li>packet arrivals per second in each direction<br>
</li><li>CDF of HTTP response times for each completed connection<br>
</li><li>CDF of RTTs for each connection<br>
</li><li>throughput per second in each direction</li></ul>

Validation Graphs<br>
<ul><li><a href='ValidationGraphsRuntime.md'>Runtime</a>
</li><li><a href='ValidationGraphsLossless.md'>Lossless </a> - original, testbed, Full-TCP, One-Way TCP<br>
</li><li><a href='ValidationGraphsLossy.md'>Lossy </a> - original, testbed, Full-TCP, One-Way TCP<br>
</li><li><a href='ValidationGraphsFullLossless.md'>Full-TCP Lossless </a> - original, testbed, FIN 1s, FIN 100 ms, FIN 10 ms<br>
</li><li><a href='ValidationGraphsOnewayLossless.md'>One-way TCP Lossless </a> - original, testbed, FIN 1s, FIN 100 ms, FIN 10 ms