---
title: "Access Guided Eviction for Unified Virtual Memory"
collection: talks
type: "Internship talk"
permalink: /talks/summer_2022
venue: "Nvidia"
date: 2022-08-26
---
Today's systems are heterogeneous. When we look at CPU-GPU systems, we can see that CPUs have more memory capacity and lower bandwidth than GPU systems. 
Furthermore, limited bandwidth interconnects make overall data flow between system components difficult to optimize. As a result, it is critical to position the data as close to the compute unit as possible and, if possible, to decrease the number of migrations between different system components.
The majority of migration costs are related to page fault latency and slow interconnects. As a result, it is critical that we decrease the number of page faults and are aware of what is evicted from GPU memory that may cause page faults later. In other words, we don't want to evict data only having to migrate it again. This is especially essential in workloads when data is reused. My research focused on enhancing the performance of the present Unified Virtual Memory (UVM) eviction mechanism, which performs miserably in workloads with data reuse. This is because the existing policy does not take access information into account. 
I created an eviction policy that attributes access patterns and access information of a workload to prevent evicting data that can be used in the near future. 
We were effective in accounting for access information and avoiding the removal of data that will be required in the near future. As a result, the number of page faults is reduced. This is in contrast to the current policy, which simply evicted data that was least recently migrated without taking into account its usage pattern. We were able to demonstrate two orders of magnitude speedup in terms of end-to-end application time when the GPU memory was oversubscribed i.e. was full and required evictions. 
This talk was given as an end of internship talk for Nvidia.
