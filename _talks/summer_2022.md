---
title: "Access Guided Eviction for Unified Virtual Memory"
collection: talks
type: "Internship talk"
permalink: /talks/summer_2022
venue: "Nvidia"
date: 2022-08-26
location: "Santa Clara, California"
---
Today’s systems are heterogeneous. Specifically, if we look at CPU-GPU systems, we notice that CPUs have higher memory capacity and lower bandwidth compared to GPU systems. 
Additionally low bandwidth interconnects makes the overall data transfer between different system components a hard problem to optimize. Hence, it becomes very important to place the data as close to location
of compute and if not, reduce the number of migrations between different system components. Migration costs are majorly attributed to page fault latency and slow interconnects. Hence, it is
important that we reduce the number of page faults and are cognizant of what is evicted from GPU memory that can cause page faults later. In other words, we do not want to evict data just to
fault on it again and add to the migrations. This is typically important in workloads that exhibit data reuse.
My work focused on improving the performance of current Unified Virtual Memory (UVM) eviction policy which fails badly for workloads that display data reuse. This is because
the current policy does not consider access information. 
I developed an eviction policy that attributes access patterns and access information of a workload to avoid evicting data that can be used in the near
future. This is unlike the current policy which simply evicted data that was least recently migrated without accounting for its usage pattern. We were able to show two orders of magnitude performance improvement
w.r.t end-to-end application time in cases where the GPU memory was oversubscribed i.e. was
full and needed evictions. The performance managed to come at-par with the undersubscribed i.e. no migration overhead case for same problem size and same number of computations. We
also displayed that for workloads that do not show data reuse, our policy fared as good as the existing policy; which was expected. We were successful in accounting for access information and
not evicting out pages that will be needed in the near future. Hence, reducing the number of page faults and evictions.
