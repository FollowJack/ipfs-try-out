# ipfs-try-out
As Blockchain developer, I'd like to investigate in IPFS in order to see the beauty of that technology.

See: https://github.com/FollowJack/ipfs-try-out/wiki 

Brainstorming:
Install: https://ipfs.io/docs/install
Getting started: https://ipfs.io/docs/getting-started/
Wikipedia: https://en.wikipedia.org/wiki/InterPlanetary_File_System

Why?
connect all the computing devices with the same system of files
Distributed content delivery saves bandwidth and prevent DDoS attacks (HTTP struggles)
IPFS has no single point of failure, and nodes do not need to trust each other, except for every node they are connected to.
Files are identified by their hashes, so it's caching-friendly.

What?
Protocol to create a permanent and decentralized method of storing and sharing files.
content-addressable, peer-to-peer hypermedia distribution protocol.
IPFS = Single BitTorrent swarm.

How?
IPFS combines a distributed hash table, an incentivized block exchange, and a self-certifying namespace IPFS provides a high-throughput, content-addressed block storage model, with content-addressed hyperlinks.
Files are identified by their hashes, so it's caching-friendly.
Every Merkle Tree (HashTree) is a directed acyclic graph (DAG). Each node is accessed via its name.

IPFS since 2014

DAG Why? any decent automated build tool (make, ant, scons, etc.) will use DAGs to ensure proper build order of the components of a program.

What?
graph = structure consisting of nodes, that are connected to each other with edges
directed = the connections between the nodes (edges) have a direction: A -> B is not the same as B -> A
acyclic = "non-circular" = moving from node to node by following the edges, you will never encounter the same node for the second time.

How?
A good example of a directed acyclic graph is a tree. Note, however, that not all directed acyclic graphs are trees.

peer adress: /ipfs/

Get objects from your peer ipfs cat /ipfs//

Calling it: http://localhost:5001/ipfs/QmPhnvn747LqwPYMJmQVorMaGbMSgA7mRRoyyZYz3DoZRQ/#/

Example to get img via ipfs in a smart contract (JS)
