# thread-fair-lock

Causes of Starvation in Java:

The following three common causes can lead to starvation of threads in Java:

    Threads with high priority swallow all CPU time from threads with lower priority.

    Threads are blocked indefinately waiting to enter a synchronized block, because other threads are constantly allowed access before it.

    Threads waiting on an object (called wait() on it) remain waiting indefinitely because other threads are constantly awakened instead of it.

fairlock : 
While it is not possible to implement 100% fairness in Java we can still implement our synchronization constructs to increase fairness between threads. 

example with fairlock : 

![image](https://user-images.githubusercontent.com/36199753/134081052-319d2310-9de6-41bb-9329-1c069560ddb2.png)
