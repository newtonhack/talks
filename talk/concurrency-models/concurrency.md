###  Outline





### Concepts
- We want to run a single task or set of task (may be inter-related)
- What do we mean by Concurrency? 
    Concurrency is all about dealing with multiple things at once. 
- How is it different from Parallelism?
    Parallelism is all about doing multiple things at once.

### Basics
- Concurrency and parallelism are often confused because traditional threads and locks don’t provide any direct support 
for parallelism. 
- If you want to exploit multiple cores, your only choice is to create a 
concurrent program and then run it on parallel hardware.  
- There will always be a need to communicate across parallel or concurrent running tasks. (Tony Hoare Paper)
- The beauty lies in how efficiently you communicate (if need-be) between parallel/concurrent running tasks with lesser waits 

### Parallel Architecture
- Parallel Architectures exists when we don't need/very less communication 
  between execution  
  - Bit-Level Parallelism 
     Why is a 32-bit computer faster than an 8-bit one? Parallelism
  - Instruction-Level Parallelism
  - Data Parallelism
  - Task Level Parallelism
  

### OS concepts
- These concepts exits/originate from OS fundamentals 
    -> OS have Multiple Processes.
    -> Multiple Processes run enabling feature like Multi-processing OR dealing with Multiple things are once.
    -> If you want to communicate across multiple processes then the solution is using IPC.
    -> Threads are another level abstraction inside process itself. 
    -> A Process can have Multiple threads. 
    -> Threads can run parallel or run concurrently depends on how they are programmed.
    -> Fundamentally, For Developer's it all "Depends on how your runtime support is available and how you leverage it".

### Need pictures related to Process, threads and how they interact.

### A level of abstraction.
- Even though Thread is a OS low level concept, and languages support that, Multi-threaded programming is hard
- But still when asked about "Is your code multi-threaded? Non-Blocking? Fast?" we see low credence. 
- Reason, low level plumbing is often complicated. 
   There can be too many locks, there can be no locks. the order of locks can go incorrect. 
   Detect incorrectness an recover from it. 
- To make complicate things simplified, we create abstractions. 
- So what we have for this one, we have models/mechanisms to efficiently deal with concurrency. 
    ( models which help's you deal with concurrency with efficient data sharing between them )

    
### Blocking vs Non-Blocking, Locking vs Lock-Free
Nature of Multi-threaded of code. 
- Blocking -> When we block one thread waiting for other thread or IO for execution, it is Blocking.  ( Thread wait no spin cycle ).
- Non-Blocking -> When a thread not waiting for execution other thread, it is non-blocking ( With help of Atomic/ CAS supported data structures).
Mechanism used in Multi-threaded code 
- Locking -> A way to synchronize / (make two thread's run in sequence)/ Serialize multi-threaded code for task. (With help of Mutex's and semaphore's)
- Lock-Free -> A way to help multi-threaded code share data/state between themselves.

### Transactional
 - Some times Let's say in distributed computing world or even multi-processor computing world, data is passed to cores.
 - It may so happens that data passed to a core is not more valid and got changed to something else.
 - This problem is very similar to a problem from database world, multiple read and write of data should guarantee ACID 
 and a mechanism of rollback or commit.   
 - They are transactions.
 
### Types of Transactions
 - Pessimistic Transactions
 - Optimistic Transactions
 - Semi-Optimistic Transactions 


### But a Question?
- What is bottle-neck in between Parallel-Multi-Core-Fast & Need of you code to go blocking..?
   Shared Mutable State
- If one can achieve to eliminate one of these Shared/Mutable/State we can achieve concurrency without a worry.
OR 
  Make the data share transactional. Remember Transactional (ACID properties)
 
- And all the models which exists till date sort of tries to eliminate one of (shared/mutable/state) or make things transactional. 



### What are different types of Concurrency Models
- Threads and Locks
- Atomic and Thread-local's
- Functional Programming
- Actors
- Communicating Sequential Process
- Software Transaction Memory
- Data-Parallelism
- Lambda Architecture
- Event-Driven Architecture
- Grid-Computing




### Anatomy of Concurrency & Parallelism with Programming languages
- Java
- Python
- Golang
- Javascript
- C/C++
 
