# Tmix Internet Traffic Generator for the ns-2 Network Simulator #

The basic idea behind Tmix is to generate realistic Internet traffic. In ns, we take *connection vectors* and 
generate TCP connections starting at the specified time and sending the specified amount of data. Each connection has 
an *initiator* (the node that starts the connection) and an *acceptor* (the node that accepts the connection). These are 
generally on opposite sides of the network from each other. 

Tmix has been included in the standard codebase of ns-2 since 
[ns-2.34] (http://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.34/) (June 2009).

Tmix for one-way TCP has been included since 
[ns-2.35] (http://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.35/) (Nov 2011).

Validation Graphs and Examples - [Tmix in ns-2 Wiki] (https://github.com/weiglemc/tmix-ns2/wiki)

Documentation - [Tmix in ns-2 Manual](http://nsnam.isi.edu/nsnam/index.php/Manual:_Tmix:_Internet_Traffic_Generation)

Note: The source code is delivered 'as-is', and we cannot offer any support. Code last updated in 2012.

For more information on Tmix, see
 * http://www.cs.odu.edu/~mweigle/papers/ccr06.pdf
 * http://www.cs.odu.edu/~mweigle/papers/adurthi-tmix-TR06.pdf
 * [Tmix at ODU](http://www.cs.odu.edu/~inets/Public/Tmix)

For more information on ns-2, see the [ns-2 Wiki](http://nsnam.isi.edu/nsnam/index.php/Main_Page)

Citation Request: If you use this in your work, please cite 

> Weigle, M. C., Adurthi, P., Hernández-Campos, F., Jeffay, K., and Smith, F. D. Tmix: a tool for generating 
>  realistic TCP application workloads in ns-2. *SIGCOMM Compututing Commununications Review* 36, 3 (Jul. 2006), 65-76. 
 * http://doi.acm.org/10.1145/1140086.1140094
 * http://www.cs.odu.edu/~mweigle/papers/ccr06.pdf
