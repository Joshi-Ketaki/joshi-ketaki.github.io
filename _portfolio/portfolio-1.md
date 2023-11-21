---
title: "Mitigating Catastrophic Forgetting using Context-Dependent Learning"
excerpt: "<br/><img src='/images/NN_task_context_learning.png'> 
<br/>
Catastrophic Forgetting is a fundamental challenge faced by all systems that learn online. We propose leveraging the cognitive inspiration of context-dependent learning to reduce forgetting in a resource-efficient manner."
collection: portfolio
---
Every online learning system faces the fundamental challenge of catastrophic forgetting. To prevent forgetfulness, we suggest utilizing cognitive inspired context-dependent learning. Here, we provide a catastrophic forgetting mitigation strategy that leverages the current neural network architecture in its essence. Our method is simpler, faster and requires less storage than current catastrophic forgetting mitigation strategies.
<br/>
<br/><img src='/images/NN_No_task_context_learning.png'> 

<br/>
<br/><img src='/images/NN_task_context_learning.png'>
<br/>
More specifically, we look at the recently proposed LSTMs for memory access prefetching which is an important sequential problem in 
computer systems memory management. We study how catatstrophic forgetting manifests in LSTMs and propose an implementation of context-dependent learning for the LSTM architecture which utilizes separate cell-state memories for each task. We demonstrate a reduction in required storage by a factor of 16 compared to existing catastrophic forgetting mitigation tactic of replay. We also demonstrate a speedup by a factor of 1.6 compared to state-of-the-art regularization methods of catastrophic forgetting mitigation. 
We plan to further extenb this investigation for other neural network architectures, specifically transformers.

<br/>
Paper: Note that this research is currently in progress and being updated continuously.
<br/>
**Joshi, Ketaki**, Pothukuchi, Raghav. Pradyumna., Wibisono, Andre., & Bhattacharjee, Abhishek. (2023). Mitigating Catastrophic Forgetting in Long Short-Term Memory Networks. ArXiv. /abs/2305.17244

