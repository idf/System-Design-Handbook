# High-Level Concepts
## CAP Theorem
![CAP](/img/CAP.png)

**Consistency** is pretty much as we’ve defined it so far. **Availability** has a particular meaning in the context of CAP—it means that if you can talk to a node in the cluster, it can read and write data. That’s subtly different from the usual meaning, which we’ll explore later. **Partition tolerance** means that the cluster can survive communication breakages in the cluster that separate the cluster into multiple partitions unable to communicate with each other (situation known as a split brain).

#
