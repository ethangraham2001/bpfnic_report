# BPFNIC

Report for my EPFL Bachelor Semester project that focused on exploring receive side scaling implemented in eBPF.

## Abstract

Receive-side scaling (RSS) is a crucial technique for improving network performance in modern
high-throughput systems by efficiently distributing incoming packet processing across multiple
CPU cores. This load balancing is vital to fully utilize multi-core processors and prevent bottlenecks
that can degrade system performance. Traditional dataplane operating systems, designed for high-
performance packet processing, often employ static load balancing schemes or specialized hardware,
which can lead to trade-offs in terms of flexibility, scalability, and ease of deployment. These systems
may lack the adaptability required to optimize for diverse and dynamic traffic patterns, and their
complexity can pose challenges for development and maintenance.
In contrast, the emergence of eBPF (extended Berkeley Packet Filter) as a programmable, high-
performance packet processing framework offers a compelling alternative. eBPF allows for dynamic
and fine-grained control over packet handling directly within the Linux kernel that can be controlled
and monitored from user-space, enabling more responsive and adaptable RSS implementations.
This programmability facilitates the development of custom load balancing algorithms that can
adjust to real-time traffic conditions, offering improved efficiency and reduced overhead compared
to traditional methods. Moreover, eBPF’s ability to be deployed without significant changes to
existing infrastructure makes it a versatile solution for a wide range of use cases. My thesis explores
the advantages of eBPF-based receive-side scaling, highlighting how it addresses the limitations of
conventional dataplane operating systems and demonstrating its potential for enhancing network
performance in diverse environments.
