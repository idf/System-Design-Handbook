# High-Level Concepts
## ACID Properties
Database transaction. 
* **Atomicity.** Atomicity requires that each transaction be "all or nothing": if one part of the transaction fails, the entire transaction fails, and the database state is left unchanged. 
* **Consistency.** The consistency property ensures that any transaction will bring the database from one valid state to another.
* **Isolation.** The isolation property ensures that the concurrent execution of transactions results in a system state that would be obtained if transactions were executed serially.
* **Durability.** Durability means that once a transaction has been committed, it will remain so, even in the event of power loss, crashes, or errors.

## CAP Theorem
![CAP](/img/CAP.png =250x)

* **Consistency** all nodes see the same data at the same time.
* **Availability** a guarantee that every request receives a response about whether it succeeded or failed. It means that IF you can talk to a node in the cluster, THEN it can read and write data. If you cannot talk to a node, then there is no requirement for the db read or write data. It is subtly different from usual meaning. 
* **Partition tolerance** means that the cluster can survive communication breakages in the cluster that separate the cluster into multiple partitions unable to communicate with each other (situation known as a split brain).

## Data Partitioning
### Sharding 

### Replication
