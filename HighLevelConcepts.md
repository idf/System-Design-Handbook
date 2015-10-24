# High-Level Concepts
## CAP Theorem
![CAP](/img/CAP.png)

* **Consistency** all nodes see the same data at the same time.
* **Availability** a guarantee that every request receives a response about whether it succeeded or failed. It means that IF you can talk to a node in the cluster, THEN it can read and write data. If you cannot talk to a node, then there is no requirement for the db read or write data. It is subtly different from usual meaning. 
* **Partition tolerance** means that the cluster can survive communication breakages in the cluster that separate the cluster into multiple partitions unable to communicate with each other (situation known as a split brain).

## Data Partitioning
### Sharding 

### Replication
