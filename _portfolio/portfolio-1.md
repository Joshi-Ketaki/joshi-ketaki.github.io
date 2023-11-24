---
title: "Mitigating Catastrophic Forgetting using Context-Dependent Learning"
excerpt: "<br/><img src='/images/NN_task_context_learning.png'> 
Catastrophic Forgetting is a fundamental challenge faced by all systems that learn online. We propose leveraging the cognitive inspiration of context-dependent learning to reduce forgetting in a resource-efficient manner."
collection: portfolio
---

We consider the fundamental challenge of learning online accurately and without catastrophic forgetting. We propose an effective strategy inspired by cognitive learning principles. We see that the human brain is constantly confronted with tasks and that it discovers and employs contextual cues to learn and recall tasks. We investigate this for the purpose of developing deep learning-based virtual memory management techniques. Virtual memory management techniques such as prefetching and eviction are important sequential problems. They demonstrate how learning-based mechanisms are required to be accurate and resource-efficient while adapting to emerging applications.
<br/><img src='/images/NN_No_task_context_learning.png'> 
<br/><img src='/images/NN_task_context_learning.png'>
We study how catastrophic forgetting manifests in neural networks. We specifically examine the recently created memory access prefetchers based on LSTMs. We notice that forgetting occurs when information is erased from the cell-state memory in LSTMs. So, we propose maintaining separate contexts in form of task-specific cell-state memories in LSTMs to mitigate forgetting.
When compared to current CF mitigation tactics, the context-dependent learning mechanism that we proposed is efficient in terms of both storage and latency. Compared to the replay technique of CF mitigation, we observer a reduction in external storage by a factor of 16 in the initial prototype studies. When compared to the regularization strategy of CF mitigation, we observe a speedup by factor of 1.6.

We plan to further continue this investigation of implementing context-dependent recall to mitigate catastrophic forgetting in more neural network architectures such as transformers. 

Note that this research is currently in progress and being updated continuously.
<br/>
Paper: 
<br/>
**Joshi, Ketaki**, Pothukuchi, Raghav. Pradyumna., Wibisono, Andre., & Bhattacharjee, Abhishek. (2023). Mitigating Catastrophic Forgetting in Long Short-Term Memory Networks. ArXiv. /abs/2305.17244

