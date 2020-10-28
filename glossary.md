# Glossary

### Weak Consistency
Related to `Concurrent Programming`.
A protocol is said to support weak consistency if:
* All accesses to `synchronization variables` are seen by all processes (or nodes, processors) in the same order (sequentially) - these are `synchronization operations`. Accesses to critical sections are seen sequentially.
* All other accesses may be seen in different order on different processes (or nodes, processors).
* The set of both read and write operations in between different synchronization operations is the same in each process.