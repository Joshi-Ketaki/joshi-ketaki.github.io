---
title: "Mitigating Catastrophic Forgetting using Context-Dependent Learning"
excerpt: "<br/><img src='/images/NN_task_context_learning.png'> 
<br/>
Catastrophic Forgetting is a fundamental challenge faced by all systems that learn online. We propose leveraging the cognitive inspiration of context-dependent learning to reduce forgetting in a resource-efficient manner."
collection: portfolio
---
We consider the fundamental challenge of learning online accurately and without catastrophic forgetting. We propose an effective strategy inspired by cognitive learning principles. We see that the human brain is constantly confronted with tasks and that it discovers and employs contextual cues to learn and recall tasks. We use this observation to deploy context-dependent learning in neural networks, which mitigates CF while being more resource-efficient than existing CF mitigation strategies.
<br/>
<br/><img src='/images/NN_No_task_context_learning.png'> 

<br/>
<br/><img src='/images/NN_task_context_learning.png'>
<br/>
We then use this approach to develop deep learning-based resource-efficient, accurate and adaptable virtual memory management techniques. We specifically examine the recently created memory access prefetchers based on LSTMs. To recognize various memory access patterns while adhering to resource limitations, a learning-based mechanism is needed which is adaptable, accurate and resource-efficient. When compared to current CF mitigation tactics, the context-dependent learning mechanism that we proposed is efficient in terms of both storage and latency. Compared to the replay technique of CF mitigation, 16X less storage has been used in the initial prototype studies. When compared to the regularization strategy of CF mitigation, we observe a speedup by factor of 1.6.
We plan to further continue this investigation of implementing context-dependent recall to mitigate catastrophic forgetting in more neural network architectures such as transformers. 

Note that this research is currently in progress and being updated continuously.
<br/>
Paper: 
<br/>
**Joshi, Ketaki**, Pothukuchi, Raghav. Pradyumna., Wibisono, Andre., & Bhattacharjee, Abhishek. (2023). Mitigating Catastrophic Forgetting in Long Short-Term Memory Networks. ArXiv. /abs/2305.17244

