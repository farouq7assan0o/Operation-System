# Operating Systems Project – Fall and Spring 2023–2024

## **Overview**

This project explores key concepts of modern operating systems through theoretical analysis, applied calculations, and practical comparisons. It covers scheduling algorithms, memory management, concurrency, distributed systems, cloud integration, and process communication. It includes real-world technologies like RPC, RMI, and multilevel memory paging.

## **Project Contents**

- CPU Scheduling Algorithms (FCFS, SJF, Round Robin, Priority, MFQS)
- Memory Management and Virtual Memory
- Concurrency and Threading
- Distributed vs Centralized OS
- Interrupt Handling and Device Communication
- Static vs Dynamic Linking and Loading
- Multi-Level Page Table Hierarchies
- RPC vs RMI Comparison
- Cloud Operating System Models (IaaS, PaaS, SaaS)

## **Scheduling Analysis**

### Round Robin, Priority, and SJF Algorithms
- Calculated turnaround and waiting times
- Simulated ready/running queue timelines
- Compared average metrics across models

### Multilevel Feedback Queue (MFQS)
- Dynamic prioritization and aging mechanisms
- Prevents starvation, improves responsiveness
- Adaptively adjusts to workload conditions

## **Memory Management**

### Virtual Memory
- Demand paging, address abstraction, and process isolation
- LRU and FIFO page replacement
- Thrashing control through multiprogramming limits
- Effective access time and performance tuning

### Multi-Level Page Table (44-bit address space)
- Page size: 16 KB
- Entry size: 16 bytes
- Structure: Three levels (inner, first outer, second outer)
- Logical address divided into:
  - 10 bits for each level
  - 14-bit offset

## **Concurrency and Interrupts**

### Concurrency
- Shared memory vs message passing
- Deadlocks, starvation, and CPU utilization
- Use of thread pools for efficiency

### Interrupt Handling Sequence
1. Device sends signal via Interrupt Request Line (IRL)
2. CPU consults Interrupt Vector Table (IVT)
3. Corresponding ISR executes
4. Device driver handles data transfer
5. CPU resumes interrupted task

## **Distributed Operating Systems**

- Distributed OS manages multiple nodes as one logical system
- Resource transparency, scalability, and load balancing
- Examples: AWS, Azure, GCP
- Compared to centralized OS in architecture, fault tolerance, and flexibility

## **Remote Communication**

### Remote Procedure Call (RPC)
- Client-side stub sends request
- Server-side stub unpacks and calls the method
- Emphasizes performance, binding, and fault tolerance

### Remote Method Invocation (RMI)
- Java-based object invocation across JVMs
- Includes stubs, skeletons, and RRL
- Supports object passing, garbage collection, and type safety

## **Static vs Dynamic Linking**

### Static Linking
- All code compiled and embedded in executable
- Larger files, fewer runtime dependencies
- Ideal for consistency and offline execution

### Dynamic Linking
- Libraries loaded at runtime
- Smaller binaries, shared memory usage
- On-demand loading reduces memory footprint

## **Cloud Operating System Integration**

### Infrastructure as a Service (IaaS)
- Resource provisioning over distributed nodes
- OS-like control over VMs and storage

### Platform as a Service (PaaS)
- Full app lifecycle management in cloud
- Runtime environments for developers

### Software as a Service (SaaS)
- Cloud-hosted applications accessible via browser
- Multi-user support, centralized updates

### OS-Level Comparison

| Feature                | Linux                                       | Windows                                      |
|------------------------|---------------------------------------------|----------------------------------------------|
| Paging                 | 2–4 level paging                            | 2–4 level paging                             |
| Swapping               | Full or partial process swap                | SuperFetch, ReadyBoost                       |
| Replacement Algorithm  | LRU                                         | FIFO, modified LRU                           |
| Interface              | CLI or GUI (KDE, GNOME)                     | GUI-based                                    |
| Licensing              | Open Source (GPL)                           | Proprietary                                  |
| Use Case               | Servers, developers                         | General users and desktop computing          |

## **Learning Outcomes**

- Developed OS-level reasoning through scheduling models
- Analyzed system-level memory management and paging structures
- Compared OS design approaches across platforms and use cases
- Understood distributed communication through RPC and RMI
- Evaluated OS integration in cloud models (IaaS, PaaS, SaaS)
- Demonstrated problem-solving through diagramming and logical flow

## **Author**

**Farouq Hassan**  
Fall and Spring 2023–2024  
HTU – Operating Systems  
Instructors: Dr. Loai Tawalbeh, Dr. Malek Louzi
