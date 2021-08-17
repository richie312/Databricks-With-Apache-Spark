# Introduction To Spark Architecture View
## Core Concepts

    * Drivers
    * Executors
    * Clusters
    * Nodes
    * Parallelization
    * Scheduling
    * Partitions
    * Job, Stages and tasks
    * Slots/Cores/Thread

### Drivers

Driver is a program that runs on the master node of the machine which declares transformations and actions on knowledge RDDs. In easy terms, the driver in Spark creates SparkContext, connected to a given Spark Master.It conjointly delivers the RDD graphs to Master, wherever the standalone cluster manager runs.

### Executors

The driver program ask for resources to the cluster manager to launch executors. Its just the space where
we can execute the operations.

### Nodes

Collections of Executors in a spark cluster.

### Parallelization

Maximum of 12 tasks; 6 Executors with 2 cores.

### Task

A single unit of work against a single partition of data

### Job

Consist of one or more stages

### Application
 Consists of more jobs

### Stage

Consists of one or more tasks