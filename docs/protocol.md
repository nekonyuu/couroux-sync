# Protocol specification

The protocol is simply text-based, as we don't need that much 
information passed between nodes.

## Heartbeats

Each node shall announce its presence by sending a multicast packet 
on the network containing `<hostname>|ANY1 GOT SAMMICH?`, sent 
every 10 seconds (configurable).

A node should consider another node dead when no message have been sent
in the last 3x<interval> seconds.

## Service state

TODO
