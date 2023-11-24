---
title: "Mitigating Catastrophic Forgetting using Context-Dependent Learning"
excerpt: "<img src='/images/NN_task_context_learning.png'> <br/>



Catastrophic Forgetting is a fundamental challenge faced by all systems that learn online. We propose leveraging the cognitive inspiration of context-dependent learning to reduce forgetting in a resource-efficient manner."
collection: portfolio
---

Online machine learning faces the fundamental issue of catastrophic forgetting (CF). This is a critical issue as it affects the model’s accuracy in learning data over time. Existing CF mitigation tactics are storage and time-consuming. This makes it difficult to deploy them in resource-constrained real-time systems. We propose an resource-efficient strategy for CF mitigation based on learning principles found in the human brain, specifically, context dependent learning.

We examine this for the usecase of building resource-efficient, accurate and adaptable memory management techniues. Virtual memory management techniques such as prefetching and eviction are important sequential problems. They affect the throughput and application turnaround time. With the emergence of new applications and the need for dynamic execution, memory management techniques that can learn memory access patterns must be developed rather than relying on hard-coded heuristics that cannot adapt to newer patterns. Memory access prefetching is a good problem to demonstrate how learning-based mechanisms are required to be accurate i.e. resistant to catastrophic forgetting and resource-efficient while adapting to emerging applications. We specifically examine the recently created memory access prefetchers based on LSTMs.

<br/><img src='/images/NN_No_task_context_learning.png'>

We are investigating how CF manifests in neural network architectures. In LSTMs, we find that when new tasks are learned, task-relevant information from previous tasks is removed from the cell-state memory, resulting in the manifestation of CF.

<br/><img src='/images/NN_task_context_learning.png'> 

We observe that similar to a neural network, the human brain is constantly confronted with tasks. It discovers and employs contextual cues to learn and recall these tasks. We use this observation and deploy context-dependent learning in neural networks, which mitigates CF while being more resource-efficient than existing CF mitigation strategies. We propose maintaining distinct cell-state memories for each task in order to maintain distinct contexts. The initial prototype studies with the proposed method show 16 times less external storage usage and is 1.6 times faster in training time compared to existing CF mitigation strategies. 
We plan to further continue this investigation of implementing context-dependent recall to mitigate catastrophic forgetting in more neural network architectures such as transformers. 

Note that this research is currently in progress and being updated continuously.
<br/>
Paper: 
<br/>
**Joshi, Ketaki**, Pothukuchi, Raghav. Pradyumna., Wibisono, Andre., & Bhattacharjee, Abhishek. (2023). Mitigating Catastrophic Forgetting in Long Short-Term Memory Networks. ArXiv. /abs/2305.17244

