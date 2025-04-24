<div align="center">
<h1>Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment</h1>

[Gaole Dai](https://maginadai.github.io/daigaole/)<sup>1,2</sup>, 
[Shiqi Jiang](https://chrisplus.me/)<sup>1</sup>, 
[Ting Cao](https://www.microsoft.com/en-us/research/people/ticao/?msockid=3c64cad47a496d892332df017e4966ec)<sup>1</sup>, 
[Yuanchun Li](http://yuanchun-li.github.io/)<sup>3</sup>, 
[Yuqing Yang](https://www.microsoft.com/en-us/research/people/yuqyang/?msockid=3c64cad47a496d892332df017e4966ec)<sup>1</sup>, 
[Rui Tan](https://personal.ntu.edu.sg/tanrui/)<sup>2</sup>, 
[Mo Li](https://cse.hkust.edu.hk/~lim/)<sup>4</sup>, 
[Lili Qiu](https://www.microsoft.com/en-us/research/people/liliqiu/)<sup>1</sup>  

<sup>1</sup> Microsoft Research   <sup>2</sup> Nanyang Technological University   <sup>3</sup> AIR @ Tsinghua University   <sup>4</sup> Hong Kong University of Science & Technology  

<a href="https://arxiv.org/abs/2503.15937">
  <img src="https://img.shields.io/badge/arXiv-2503.15937-red" alt="Paper PDF">
</a>
<a href="https://v-droid-agent.github.io">
  <img src="https://img.shields.io/badge/Project%20Page-V--Droid-green"
       alt="Project Page">
</a>
<a href="https://github.com/V-Droid-Agent/V-Droid-Agent.github.io">
  <img src="https://img.shields.io/badge/Code-GitHub-blue" alt="Code Repo">
</a>
</div>


## Overview
Introducing V-Droid – the first mobile GUI agent with near-real-time, high-quality decision making ability. Unlike traditional agents that rely on large language models (LLMs) to generate actions at every step, V-Droid employes LLMs as verifiers evaluating candidate actions to ensure optimal decision-making.

V-Droid features:

1. Discretized Action Space & Prefilling-Only Workflow: Accelerates decision-making by verifying candidate actions in parallel using prefix caching.

2. Pair-Wise Progress Preference Training: Enhances the verifier’s decision-making and self-correction capabilities through progress-aware training.

3. Scalable Human-Agent Joint Annotation: V-Droid quickly takes the lead role in the annotation process after just two training rounds, significantly reducing overhead while boosting performance.

V-Droid has set new benchmarks in mobile tasks automation, achieving state-of-the-art task success rates of 59.5% on AndroidWorld, 38.3% on AndroidLab, and 49% on MobileAgentBench, outperforming existing agents by 9.5%, 2.1%, and 9%, respectively. Furthermore, V-Droid achieves an low latency of 0.7 seconds per decision, which is 32.8X faster than existing agents.



## Citation
```bibtex
@article{dai2025advancing,
  title={Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment},
  author={Dai, Gaole and Jiang, Shiqi and Cao, Ting and Li, Yuanchun and Yang, Yuqing and Tan, Rui and Li, Mo and Qiu, Lili},
  journal={arXiv preprint arXiv:2503.15937},
  year={2025}
}
