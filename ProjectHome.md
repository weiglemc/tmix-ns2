The basic idea behind Tmix is to generate realistic Internet traffic. In ns, we take _connection vectors_ and generate TCP connections starting at the specified time and sending the specified amount of data. Each connection has an _initiator_ (the node that starts the connection) and an _acceptor_ (the node that accepts the connection). These are generally on opposite sides of the network from each other.

Tmix has been included in the standard codebase of ns-2 since [ns-2.34](http://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.34/) (June 2009).

Tmix for one-way TCP has been included since
[ns-2.35](http://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.35/) (Nov 2011).

Validation Graphs and Examples - [Tmix in ns-2 Wiki](http://code.google.com/p/tmix-ns2/wiki/Home)

Documentation - [Tmix in ns-2 Manual](http://nsnam.isi.edu/nsnam/index.php/Manual:_Tmix:_Internet_Traffic_Generation)

For more information on Tmix, see
  * Weigle, M. C., Adurthi, P., Hernández-Campos, F., Jeffay, K., and Smith, F. D. Tmix: a tool for generating realistic TCP application workloads in ns-2. SIGCOMM Comput. Commun. Rev. 36, 3 (Jul. 2006), 65-76. http://doi.acm.org/10.1145/1140086.1140094
  * [Tmix at ODU](http://www.cs.odu.edu/inets/Tmix/)

For more information on ns-2, see the [ns-2 Wiki](http://nsnam.isi.edu/nsnam/index.php/Main_Page)