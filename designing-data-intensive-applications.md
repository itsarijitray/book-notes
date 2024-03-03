# [Designing Data-Intensive Applications](https://dataintensive.net/)

- [Designing Data-Intensive Applications](#designing-data-intensive-applications)
  - [Reliable, scalable, and maintainable applications](#reliable-scalable-and-maintainable-applications)
    - [Reliability](#reliability)


## Reliable, scalable, and maintainable applications
Data intensive applications are usually required to:
- Store and retrieve data (databases)
- memorize results of expensive ops (caches)
- Allow data to be searched by keywords or filters (indexes)
- send message to other processes to be handles asynchronously (stream processing)
- Load large chunk of data periodically (batch processing)

### Reliability
The idea is that "the software should continue to work correctly even when things go wrong (faults)"

Fault != Failure

Failure is when the software stops giving the required services. 

It is very difficult to make a system completely fault tolerant.

One way to ensure that a system is fault toleralant is to deliberatlely introduce faults in the system to excercise fault tolerance (case in point: [Netflix's Chaos Monkey](https://netflixtechblog.com/the-netflix-simian-army-16e57fbab116))

