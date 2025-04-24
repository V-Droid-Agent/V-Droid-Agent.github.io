<div align="center">
<h1>V-Droid: Advancing Mobile&nbsp;GUI&nbsp;Agents with a Verifier-Driven Paradigm</h1>

[Gaole Dai](https://maginadai.github.io/daigaole/)<sup>1*</sup>†, 
[Shiqi Jiang]((https://chrisplus.me/))<sup>1*</sup>, 
[Ting Cao](https://github.com/ticao)<sup>1</sup>, 
[Yuanchun Li](https://paperswithcode.com/author/yuanchun-li)<sup>3</sup>, 
[Yuqing Yang](https://github.com/yuqyang)<sup>1</sup>, 
[Rui Tan](https://tanrui.me/)<sup>2</sup>, 
[Mo Li](https://cse.hkust.edu.hk/faculty/lim/)<sup>4</sup>, 
[Lili Qiu](https://www.microsoft.com/en-us/research/people/liliqiu/)<sup>1‡</sup>  

<sup>1</sup> Microsoft Research   <sup>2</sup> Nanyang Technological University   <sup>3</sup> AIR @ Tsinghua University   <sup>4</sup> Hong Kong University of Science & Technology  

<sup>*</sup> Equal Contribution <sup>†</sup> Project Lead <sup>‡</sup> Corresponding Author  

<a href="https://arxiv.org/abs/2503.15937">
  <img src="https://img.shields.io/badge/arXiv-2503.15937-red" alt="Paper PDF">
</a>
<a href="[https://v-droid-gui.github.io](https://v-droid-agent.github.io/)/">
  <img src="https://img.shields.io/badge/Project_Page-V-Droid-green" alt="Project Page">
</a>
<a href="https://github.com/v-droid-gui/V-Droid">
  <img src="https://img.shields.io/badge/Code-GitHub-blue" alt="Code Repo">
</a>
</div>


## Overview
V-Droid is the **first mobile agent that treats large language models as _verifiers_ rather than _generators_**, dramatically boosting both decision accuracy and interaction speed on real Android devices.&#8203;:contentReference[oaicite:0]{index=0}  
Our framework constructs a finite action space from accessibility events, scores every candidate in parallel with a lightweight 8 B LLM, and executes the top-ranked action in under a second.&#8203;:contentReference[oaicite:1]{index=1}

![Demo GIF](./assets/v-droid-intro.gif)


### Key Findings
1. **Verifier-Driven Decision Making**  
   V-Droid decouples action generation from evaluation: a task-agnostic extractor proposes UI actions, and an LLM verifier picks the best one via Pairwise-Process Preference (P3) training.&#8203;:contentReference[oaicite:2]{index=2}  

2. **State-of-the-Art Success Rates**  
   *59.5 %* on **AndroidWorld**, *38.3 %* on **AndroidLab**, and *49.0 %* on **MobileAgentBench**—improvements of 9.5 %, 2.1 %, and 9 % over the previous best agents.&#8203;:contentReference[oaicite:3]{index=3}  

3. **Near-Real-Time Latency**  
   With a prefilling-only workflow and batched verification, the agent acts in **0.7 s per step** on dual RTX 4090 GPUs, meeting real-time interaction constraints for the first time.&#8203;:contentReference[oaicite:4]{index=4}  

4. **Scalable Data Pipeline**  
   A Human-Agent Joint Annotation scheme halves manual labeling by flagging high-entropy steps, while P3 fine-tuning yields robust verifiers with <100 K annotations.&#8203;:contentReference[oaicite:5]{index=5}  

5. **Open & Reproducible**  
   Code, datasets, and one-command Docker benchmarking scripts are released under MIT to accelerate community progress.&#8203;:contentReference[oaicite:6]{index=6}  


## Citation
```bibtex
@article{dai2025vdroid,
  title     = {Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment},
  author    = {Dai, Gaole and Jiang, Shiqi and Cao, Ting and Li, Yuanchun and
               Yang, Yuqing and Tan, Rui and Li, Mo and Qiu, Lili},
  journal   = {arXiv preprint arXiv:2503.15937},
  year      = {2025}
}
