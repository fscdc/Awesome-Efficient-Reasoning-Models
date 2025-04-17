<div align="center">

  <h2><b> Efficient Reasoning Models: A Survey </b></h2>
  <h4> An overview of research in efficient reasoning models</h4>

</div>


<div align="center">

![](https://img.shields.io/github/stars/fscdc/Awesome-Efficient-Reasoning-Models?color=yellow)
![](https://img.shields.io/github/forks/fscdc/Awesome-Efficient-Reasoning-Models?color=lightblue)
![](https://img.shields.io/github/last-commit/fscdc/Awesome-Efficient-Reasoning-Models?color=green)
![](https://img.shields.io/badge/PRs-Welcome-blue)
<a href="https://arxiv.org/abs/2504.10903" target="_blank"><img src="https://img.shields.io/badge/arXiv-2504.10903-009688.svg" alt="arXiv"></a>

</div>

<div align="center">

**[<a href="https://arxiv.org/abs/2504.10903">arXiv</a>]** **[<a href="https://huggingface.co/papers/2504.10903">HuggingFace</a>]**

</div>



This repository is for our paper:

> **[Efficient Reasoning Models: A Survey](https://arxiv.org/abs/2504.10903)** \
> [Sicheng Feng](https://fscdc.github.io/)<sup>1,2</sup>, [Gongfan Fang](https://fangggf.github.io/)<sup>1</sup>, [Xinyin Ma](https://horseee.github.io/)<sup>1</sup>, [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)<sup>1,*</sup> \
> <sup>1</sup>National University of Singapore, Singapore \
> <sup>2</sup>Nankai University, Tianjin, China \
> <sup>∗</sup>Corresponding author: xinchao@nus.edu.sg

---
>
> 🙋 Please let us know if you find out a mistake or have any suggestions!
> 
> 🌟 If you find this resource helpful, please consider to star this repository and cite our [research](#citation)!

<p align="center">
<img src="assets/figure2.svg" width = "95%" alt="" align=center />
</p>


## Updates

- 2025-04-16: 📝 The survey is now available on [arXiv](https://arxiv.org/abs/2504.10903)!
- 2025-04-11: 📚 The full paper list is now available and our survey is coming soon!
- 2025-03-16: 🚀 Efficient Reasoning Repo launched!


## Full list


> **Contributions**
>
> If you want to add your paper or update details like conference info or code URLs, please submit a pull request. You can generate the necessary markdown for each paper by filling out `generate_item.py` and running `python generate_item.py`. We greatly appreciate your contributions. Alternatively, you can email me ([Gmail](fscnkucs@gmail.com)) the links to your paper and code, and I will add your paper to the list as soon as possible.

---
<p align="center">
<img src="assets/taxonomy.png" width = "95%" alt="" align=center />
</p>

### Quick Links
  - [Make Long CoT Short](#Make-Long-CoT-Short)
    - [SFT-based Methods](#SFT-based-Methods)
    - [RL-based Methods](#RL-based-Methods)
    - [Prompt-driven Methods](#Prompt-driven-Methods)
    - [Latent Reasoning](#Latent-Reasoning)
  - [Build SLM with Strong Reasoning Ability](#Build-SLM-with-Strong-Reasoning-Ability)
    - [Distillation](#Distillation)
    - [Quantization and Pruning](#Quantization-and-Pruning)
    - [RL-based Methods](#RL-based-Methods)
  - [Let Decoding More Efficient](#Let-Decoding-More-Efficient)
    - [Efficient TTS](#Efficient-TTS)
    - [Other Optimal Methods](#Other-Optimal-Methods)
  - [Evaluation and Benchmarks](#Evaluation-and-Benchmarks)
  - [Background Papers](#Background-Papers)





### Make Long CoT Short

#### SFT-based Methods
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/horseee/CoT-Valve.svg?style=social&label=Star)](https://github.com/horseee/CoT-Valve)<br>[CoT-Valve: Length-Compressible Chain-of-Thought Tuning](https://arxiv.org/abs/2502.09601) <br> Xinyin Ma, Guangnian Wan, Runpeng Yu, Gongfan Fang, Xinchao Wang |<img width="1002" alt="image" src="figures/cot_valve.png"> |[Github](https://github.com/horseee/CoT-Valve) <br> [Paper](https://arxiv.org/abs/2502.09601)|[//]: #03/16
|[![Publish](https://img.shields.io/badge/Conference-AAAI_2025-blue)]()<br>[C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness](https://arxiv.org/abs/2412.11664) <br> Yu Kang, Xianghui Sun, Liangyu Chen, Wei Zou |<img width="1002" alt="image" src="figures/co3t.png"> |[Paper](https://arxiv.org/abs/2412.11664)|[//]: #03/16
|[![Star](https://img.shields.io/github/stars/tengxiaoliu/LM_skip.svg?style=social&label=Star)](https://github.com/tengxiaoliu/LM_skip) [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2024-blue)]()<br>[Can Language Models Learn to Skip Steps?](https://arxiv.org/abs/2411.01855) <br> Tengxiao Liu, Qipeng Guo, Xiangkun Hu, Cheng Jiayang, Yue Zhang, Xipeng Qiu, Zheng Zhang |<img width="1002" alt="image" src="figures/skip_step.png"> |[Github](https://github.com/tengxiaoliu/LM_skip) <br> [Paper](https://arxiv.org/abs/2411.01855)|[//]: #03/16
|[Distilling System 2 into System 1](https://arxiv.org/abs/2407.06023) <br> Ping Yu, Jing Xu, Jason Weston, Ilia Kulikov |<img width="1002" alt="image" src="figures/distill_sys1_sys2.png"> |[Paper](https://arxiv.org/abs/2407.06023)|[//]: #03/16
|[![Star](https://img.shields.io/github/stars/hemingkx/TokenSkip.svg?style=social&label=Star)](https://github.com/hemingkx/TokenSkip)<br>[TokenSkip: Controllable Chain-of-Thought Compression in LLMs](https://arxiv.org/abs/2502.12067) <br> Heming Xia, Yongqi Li, Chak Tou Leong, Wenjie Wang, Wenjie Li |<img width="1002" alt="image" src="figures/TokenSkip.png"> |[Github](https://github.com/hemingkx/TokenSkip) <br> [Paper](https://arxiv.org/abs/2502.12067)|[//]: #03/20
|[Stepwise Perplexity-Guided Refinement for Efficient Chain-of-Thought Reasoning in Large Language Models](https://arxiv.org/abs/2502.13260) <br> Yingqian Cui, Pengfei He, Jingying Zeng, Hui Liu, Xianfeng Tang, Zhenwei Dai, Yan Han, Chen Luo, Jing Huang, Zhen Li, Suhang Wang, Yue Xing, Jiliang Tang, Qi He |<img width="1002" alt="image" src="https://arxiv.org/html/2502.13260v1/extracted/6214965/pics/merge.png"> |[Paper](https://arxiv.org/abs/2502.13260)| [//]: #04/08
|[Towards Thinking-Optimal Scaling of Test-Time Compute for LLM Reasoning](https://arxiv.org/abs/2502.18080) <br> Wenkai Yang, Shuming Ma, Yankai Lin, Furu Wei |<img width="1002" alt="image" src="https://arxiv.org/html/2502.18080v1/x10.png"> |[Paper](https://arxiv.org/abs/2502.18080)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/TergelMunkhbat/concise-reasoning.svg?style=social&label=Star)](https://github.com/TergelMunkhbat/concise-reasoning)<br>[Self-Training Elicits Concise Reasoning in Large Language Models](https://arxiv.org/abs/2502.20122) <br> Tergel Munkhbat, Namgyu Ho, Seo Hyun Kim, Yongjin Yang, Yujin Kim, Se-Young Yun |<img width="1002" alt="image" src="https://arxiv.org/html/2502.20122v2/x1.png"> |[Github](https://github.com/TergelMunkhbat/concise-reasoning) <br> [Paper](https://arxiv.org/abs/2502.20122)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/GeniusHTX/TALE.svg?style=social&label=Star)](https://github.com/GeniusHTX/TALE)<br>[Token-Budget-Aware LLM Reasoning](https://arxiv.org/abs/2412.18547) <br> Tingxu Han, Zhenting Wang, Chunrong Fang, Shiyu Zhao, Shiqing Ma, Zhenyu Chen |<img width="1002" alt="image" src="https://arxiv.org/html/2412.18547v4/x10.png"> |[Github](https://github.com/GeniusHTX/TALE) <br> [Paper](https://arxiv.org/abs/2412.18547)| [//]: #04/08


#### RL-based Methods
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/StarDewXXX/O1-Pruner.svg?style=social&label=Star)](https://github.com/StarDewXXX/O1-Pruner)<br>[O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning](https://arxiv.org/abs/2501.12570) <br> Haotian Luo, Li Shen, Haiying He, Yibo Wang, Shiwei Liu, Wei Li, Naiqiang Tan, Xiaochun Cao, Dacheng Tao |<img width="1002" alt="image" src="figures/o1_pruner.png"> |[Github](https://github.com/StarDewXXX/O1-Pruner) <br> [Paper](https://arxiv.org/abs/2501.12570)|[//]: #03/16
|[Kimi k1.5: Scaling Reinforcement Learning with LLMs](https://arxiv.org/abs/2501.12599) <br> Kimi Team |<img width="1002" alt="image" src="https://arxiv.org/html/2501.12599v2/x3.png"> |[Paper](https://arxiv.org/abs/2501.12599)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/eddycmu/demystify-long-cot.svg?style=social&label=Star)](https://github.com/eddycmu/demystify-long-cot)<br>[Demystifying Long Chain-of-Thought Reasoning in LLMs](https://arxiv.org/abs/2502.03373) <br> Edward Yeo, Yuxuan Tong, Morry Niu, Graham Neubig, Xiang Yue |<img width="1002" alt="image" src="https://arxiv.org/html/2502.03373v1/x1.png"> |[Github](https://github.com/eddycmu/demystify-long-cot) <br> [Paper](https://arxiv.org/abs/2502.03373)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Zanette-Labs/efficient-reasoning.svg?style=social&label=Star)](https://github.com/Zanette-Labs/efficient-reasoning)<br>[Training Language Models to Reason Efficiently](https://arxiv.org/abs/2502.04463) <br> Daman Arora, Andrea Zanette |<img width="1002" alt="image" src="https://arxiv.org/html/2502.04463v2/x3.png"> |[Github](https://github.com/Zanette-Labs/efficient-reasoning) <br> [Paper](https://arxiv.org/abs/2502.04463)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/cmu-l3/l1.svg?style=social&label=Star)](https://github.com/cmu-l3/l1)<br>[L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning](https://www.arxiv.org/abs/2503.04697) <br> Pranjal Aggarwal, Sean Welleck |<img width="1002" alt="image" src="https://arxiv.org/html/2503.04697v1/x2.png"> |[Github](https://github.com/cmu-l3/l1) <br> [Paper](https://www.arxiv.org/abs/2503.04697)| [//]: #04/08
|[DAST: Difficulty-Adaptive Slow-Thinking for Large Reasoning Models](https://arxiv.org/abs/2503.04472) <br> Yi Shen, Jian Zhang, Jieyun Huang, Shuming Shi, Wenjing Zhang, Jiangze Yan, Ning Wang, Kai Wang, Shiguo Lian |<img width="1002" alt="image" src="https://arxiv.org/html/2503.04472v1/extracted/6254851/DAST.png"> |[Paper](https://arxiv.org/abs/2503.04472)| [//]: #04/08
|[Adaptive Group Policy Optimization: Towards Stable Training and Token-Efficient Reasoning](https://arxiv.org/abs/2503.15952) <br> Chen Li, Nazhou Liu, Kai Yang |<img width="1002" alt="image" src="figures/agpo.png"> |[Paper](https://arxiv.org/abs/2503.15952)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/UCSB-NLP-Chang/ThinkPrune.svg?style=social&label=Star)](https://github.com/UCSB-NLP-Chang/ThinkPrune)<br>[ThinkPrune: Pruning Long Chain-of-Thought of LLMs via Reinforcement Learning](https://arxiv.org/abs/2504.01296) <br> Bairu Hou, Yang Zhang, Jiabao Ji, Yujian Liu, Kaizhi Qian, Jacob Andreas, Shiyu Chang |<img width="1002" alt="image" src="https://arxiv.org/html/2504.01296v1/x1.png"> |[Github](https://github.com/UCSB-NLP-Chang/ThinkPrune) <br> [Paper](https://arxiv.org/abs/2504.01296)| [//]: #04/08
|[Think When You Need: Self-Adaptive Chain-of-Thought Learning](https://arxiv.org/abs/2504.03234) <br> Junjie Yang, Ke Lin, Xing Yu |<img width="1002" alt="image" src="https://arxiv.org/html/2504.03234v1/extracted/6335120/alg_illu.png"> |[Paper](https://arxiv.org/abs/2504.03234)| [//]: #04/08



#### Prompt-driven Methods

##### Prompt-guided Efficint Reasoning

| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/GeniusHTX/TALE.svg?style=social&label=Star)](https://github.com/GeniusHTX/TALE)<br>[Token-Budget-Aware LLM Reasoning](https://arxiv.org/abs/2412.18547) <br> Tingxu Han, Zhenting Wang, Chunrong Fang, Shiyu Zhao, Shiqing Ma, Zhenyu Chen |<img width="1002" alt="image" src="https://arxiv.org/html/2412.18547v4/x10.png"> |[Github](https://github.com/GeniusHTX/TALE) <br> [Paper](https://arxiv.org/abs/2412.18547)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/matthewrenze/jhu-concise-cot.svg?style=social&label=Star)](https://github.com/matthewrenze/jhu-concise-cot) [![Publish](https://img.shields.io/badge/Conference-FLLM_2024-blue)]()<br>[The Benefits of a Concise Chain of Thought on Problem-Solving in Large Language Models](https://arxiv.org/abs/2401.05618) <br> Matthew Renze, Erhan Guven |<img width="1002" alt="image" src="https://arxiv.org/html/2401.05618v3/x1.png"> |[Github](https://github.com/matthewrenze/jhu-concise-cot) <br> [Paper](https://arxiv.org/abs/2401.05618)| [//]: #04/08
|[Break the Chain: Large Language Models Can be Shortcut Reasoners](https://arxiv.org/abs/2406.06580) <br> Mengru Ding, Hanmeng Liu, Zhizhang Fu, Jian Song, Wenbo Xie, Yue Zhang |<img width="1002" alt="image" src="https://arxiv.org/html/2406.06580v1/x1.png"> |[Paper](https://arxiv.org/abs/2406.06580)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/sileix/chain-of-draft.svg?style=social&label=Star)](https://github.com/sileix/chain-of-draft)<br>[Chain of Draft: Thinking Faster by Writing Less](https://arxiv.org/abs/2502.18600) <br> Silei Xu, Wenhao Xie, Lingxiao Zhao, Pengcheng He |<img width="1002" alt="image" src="https://arxiv.org/html/2502.18600v2/extracted/6244873/plot.png"> |[Github](https://github.com/sileix/chain-of-draft) <br> [Paper](https://arxiv.org/abs/2502.18600)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/LightChen233/reasoning-boundary.svg?style=social&label=Star)](https://github.com/LightChen233/reasoning-boundary) [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2024-blue)]()<br>[Unlocking the Capabilities of Thought: A Reasoning Boundary Framework to Quantify and Optimize Chain-of-Thought](https://arxiv.org/abs/2410.05695) <br> Qiguang Chen, Libo Qin, Jiaqi Wang, Jinxuan Zhou, Wanxiang Che |<img width="1002" alt="image" src="https://arxiv.org/html/2410.05695v2/x1.png"> |[Github](https://github.com/LightChen233/reasoning-boundary) <br> [Paper](https://arxiv.org/abs/2410.05695)| [//]: #04/08
|[How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach](https://arxiv.org/abs/2503.01141) <br> Ayeong Lee, Ethan Che, Tianyi Peng |<img src="https://arxiv.org/html/2503.01141v2/extracted/6325669/plot/mmlu-pro-legend.png" width="45%"> <img src="https://arxiv.org/html/2503.01141v2/extracted/6325669/plot/Anthropic/claude-3-5-sonnet-20241022-mmlu-main.png" width="45%"> |[Paper](https://arxiv.org/abs/2503.01141)| [//]: #04/08



##### Prompt Attribute-Aware Reasoning Routing

| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach](https://arxiv.org/abs/2503.01141) <br> Ayeong Lee, Ethan Che, Tianyi Peng |<img src="https://arxiv.org/html/2503.01141v2/extracted/6325669/plot/mmlu-pro-legend.png" width="45%"> <img src="https://arxiv.org/html/2503.01141v2/extracted/6325669/plot/Anthropic/claude-3-5-sonnet-20241022-mmlu-main.png" width="45%"> |[Paper](https://arxiv.org/abs/2503.01141)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br>[RouteLLM: Learning to Route LLMs with Preference Data](https://arxiv.org/abs/2406.18665) <br> Isaac Ong, Amjad Almahairi, Vincent Wu, Wei-Lin Chiang, Tianhao Wu, Joseph E. Gonzalez, M Waleed Kadous, Ion Stoica |<img width="1002" alt="image" src="https://arxiv.org/html/2406.18665v4/extracted/6226172/Figs/gsm8k.png"> |[Paper](https://arxiv.org/abs/2406.18665)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/SimonAytes/SoT.svg?style=social&label=Star)](https://github.com/SimonAytes/SoT)<br>[Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching](https://arxiv.org/abs/2503.05179) <br> Simon A. Aytes, Jinheon Baek, Sung Ju Hwang |<img width="1002" alt="image" src="https://arxiv.org/html/2503.05179v1/x1.png"> |[Github](https://github.com/SimonAytes/SoT) <br> [Paper](https://arxiv.org/abs/2503.05179)| [//]: #04/08
|[Learning to Route LLMs with Confidence Tokens](https://arxiv.org/abs/2410.13284) <br> Yu-Neng Chuang, Helen Zhou, Prathusha Kameswara Sarma, Parikshit Gopalan, John Boccio, Sara Bolouki, Xia Hu |<img width="1002" alt="image" src="https://arxiv.org/html/2410.13284v2/x1.png"> |[Paper](https://arxiv.org/abs/2410.13284)| [//]: #04/08
|[Confident or Seek Stronger: Exploring Uncertainty-Based On-device LLM Routing From Benchmarking to Generalization](https://arxiv.org/abs/2502.04428) <br> Yu-Neng Chuang, Leisheng Yu, Guanchu Wang, Lizhe Zhang, Zirui Liu, Xuanting Cai, Yang Sui, Vladimir Braverman, Xia Hu |<img width="1002" alt="image" src="https://arxiv.org/html/2502.04428v1/x1.png"> |[Paper](https://arxiv.org/abs/2502.04428)| [//]: #04/08

###### Blog
* [Claude 3.7 Sonnet](https://www.anthropic.com/news/claude-3-7-sonnet). Claude team. [[Paper]](https://www.anthropic.com/news/claude-3-7-sonnet)


#### Latent Reasoning
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[Beyond Chains of Thought: Benchmarking Latent-Space Reasoning Abilities in Large Language Models](https://arxiv.org/abs/2504.10615) <br> Thilo Hagendorff, Sarah Fabi |<img width="1002" alt="image" src="./figures/BCoT.png"> |[Paper](https://arxiv.org/abs/2504.10615)|[//]: #04/17
|[Distilling System 2 into System 1](https://arxiv.org/abs/2407.06023) <br> Ping Yu, Jing Xu, Jason Weston, Ilia Kulikov |<img width="1002" alt="image" src="figures/distill_sys1_sys2.png"> |[Paper](https://arxiv.org/abs/2407.06023)|[//]: #03/16
|[![Star](https://img.shields.io/github/stars/da03/implicit_chain_of_thought.svg?style=social&label=Star)](https://github.com/da03/implicit_chain_of_thought/)<br>[Implicit Chain of Thought Reasoning via Knowledge Distillation](https://arxiv.org/abs/2311.01460) <br> Yuntian Deng, Kiran Prasad, Roland Fernandez, Paul Smolensky, Vishrav Chaudhary, Stuart Shieber |<img width="1002" alt="image" src="figures/explicit2implicit.png"> |[Github](https://github.com/da03/implicit_chain_of_thought/) <br> [Paper](https://arxiv.org/abs/2311.01460)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/HKUNLP/diffusion-of-thoughts.svg?style=social&label=Star)](https://github.com/HKUNLP/diffusion-of-thoughts) [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2024-blue)]()<br>[Diffusion of Thoughts: Chain-of-Thought Reasoning in Diffusion Language Models](https://arxiv.org/abs/2402.07754) <br> Jiacheng Ye, Shansan Gong, Liheng Chen, Lin Zheng, Jiahui Gao, Han Shi, Chuan Wu, Xin Jiang, Zhenguo Li, Wei Bi, Lingpeng Kong |<img width="1002" alt="image" src="figures/diffusion_thought.png"> |[Github](https://github.com/HKUNLP/diffusion-of-thoughts) <br> [Paper](https://arxiv.org/abs/2402.07754)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/da03/Internalize_CoT_Step_by_Step.svg?style=social&label=Star)](https://github.com/da03/Internalize_CoT_Step_by_Step)<br>[From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step](https://arxiv.org/abs/2405.14838) <br> Yuntian Deng, Yejin Choi, Stuart Shieber |<img width="1002" alt="image" src="https://arxiv.org/html/2405.14838v1/extracted/2405.14838v1/training_illustration.png"> |[Github](https://github.com/da03/Internalize_CoT_Step_by_Step) <br> [Paper](https://arxiv.org/abs/2405.14838)| [//]: #04/08
|[Compressed Chain of Thought: Efficient Reasoning Through Dense Representations](https://arxiv.org/abs/2412.13171) <br> Jeffrey Cheng, Benjamin Van Durme |<img width="1002" alt="image" src="https://arxiv.org/html/2412.13171v1/extracted/6074157/figures/fig1.png"> |[Paper](https://arxiv.org/abs/2412.13171)| [//]: #04/08
|[SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs](https://arxiv.org/abs/2502.12134) <br> Yige Xu, Xu Guo, Zhiwei Zeng, Chunyan Miao |<img width="1002" alt="image" src="https://arxiv.org/html/2502.12134v1/x1.png"> |[Paper](https://arxiv.org/abs/2502.12134)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br>[Reasoning with Latent Thoughts: On the Power of Looped Transformers](https://arxiv.org/abs/2502.17416) <br> Nikunj Saunshi, Nishanth Dikkala, Zhiyuan Li, Sanjiv Kumar, Sashank J. Reddi |<img width="1002" alt="image" src="https://arxiv.org/html/2502.17416v1/extracted/6229618/Media/looping_illustration2.png"> |[Paper](https://arxiv.org/abs/2502.17416)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/qifanyu/RELAY.svg?style=social&label=Star)](https://github.com/qifanyu/RELAY)<br>[Enhancing Auto-regressive Chain-of-Thought through Loop-Aligned Reasoning](https://arxiv.org/abs/2502.08482) <br> Qifan Yu, Zhenyu He, Sijie Li, Xun Zhou, Jun Zhang, Jingjing Xu, Di He |<img width="1002" alt="image" src="https://arxiv.org/html/2502.08482v1/x1.png"> |[Github](https://github.com/qifanyu/RELAY) <br> [Paper](https://arxiv.org/abs/2502.08482)| [//]: #04/08
|[CODI: Compressing Chain-of-Thought into Continuous Space via Self-Distillation](https://arxiv.org/abs/2502.21074) <br> Zhenyi Shen, Hanqi Yan, Linhai Zhang, Zhanghao Hu, Yali Du, Yulan He |<img width="1002" alt="image" src="https://arxiv.org/html/2502.21074v1/extracted/6241542/figures/codi_illustrate12.png"> |[Paper](https://arxiv.org/abs/2502.21074)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/zjunlp/LightThinker.svg?style=social&label=Star)](https://github.com/zjunlp/LightThinker)<br>[LightThinker: Thinking Step-by-Step Compression](https://arxiv.org/abs/2502.15589) <br> Jintian Zhang, Yuqi Zhu, Mengshu Sun, Yujie Luo, Shuofei Qiao, Lun Du, Da Zheng, Huajun Chen, Ningyu Zhang |<img width="1002" alt="image" src="https://arxiv.org/html/2502.15589v1/x1.png"> |[Github](https://github.com/zjunlp/LightThinker) <br> [Paper](https://arxiv.org/abs/2502.15589)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/WANGXinyiLinda/planning_tokens.svg?style=social&label=Star)](https://github.com/WANGXinyiLinda/planning_tokens) [![Publish](https://img.shields.io/badge/Conference-COLM_2024-blue)]()<br>[Guiding Language Model Reasoning with Planning Tokens](https://arxiv.org/abs/2310.05707) <br> Xinyi Wang, Lucas Caccia, Oleksiy Ostapenko, Xingdi Yuan, William Yang Wang, Alessandro Sordoni |<img width="1002" alt="image" src="https://arxiv.org/html/2310.05707v4/extracted/5777851/img/overview.png"> |[Github](https://github.com/WANGXinyiLinda/planning_tokens) <br> [Paper](https://arxiv.org/abs/2310.05707)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/JacobPfau/fillerTokens.svg?style=social&label=Star)](https://github.com/JacobPfau/fillerTokens) [![Publish](https://img.shields.io/badge/Conference-COLM_2024-blue)]()<br>[Let's Think Dot by Dot: Hidden Computation in Transformer Language Models](https://arxiv.org/abs/2404.15758) <br> Jacob Pfau, William Merrill, Samuel R. Bowman |<img width="1002" alt="image" src="https://arxiv.org/html/2404.15758v1/extracted/2404.15758v1/figs/scale_len.png"> |[Github](https://github.com/JacobPfau/fillerTokens) <br> [Paper](https://arxiv.org/abs/2404.15758)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/MingyuJ666/Disentangling-Memory-and-Reasoning.svg?style=social&label=Star)](https://github.com/MingyuJ666/Disentangling-Memory-and-Reasoning)<br>[Disentangling Memory and Reasoning Ability in Large Language Models](https://arxiv.org/abs/2411.13504) <br> Mingyu Jin, Weidi Luo, Sitao Cheng, Xinyi Wang, Wenyue Hua, Ruixiang Tang, William Yang Wang, Yongfeng Zhang |<img width="1002" alt="image" src="https://arxiv.org/html/2411.13504v2/x1.png"> |[Github](https://github.com/MingyuJ666/Disentangling-Memory-and-Reasoning) <br> [Paper](https://arxiv.org/abs/2411.13504)| [//]: #04/08
|[Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning](https://arxiv.org/abs/2502.03275) <br> DiJia Su, Hanlin Zhu, Yingchen Xu, Jiantao Jiao, Yuandong Tian, Qinqing Zheng |<img width="1002" alt="image" src="https://arxiv.org/html/2502.03275v1/x1.png"> |[Paper](https://arxiv.org/abs/2502.03275)| [//]: #04/08
|[Training Large Language Models to Reason in a Continuous Latent Space](https://arxiv.org/abs/2412.06769) <br> Shibo Hao, Sainbayar Sukhbaatar, DiJia Su, Xian Li, Zhiting Hu, Jason Weston, Yuandong Tian |<img width="1002" alt="image" src="https://arxiv.org/html/2412.06769v2/extracted/6060815/figures/figure_1_meta_3.png"> |[Paper](https://arxiv.org/abs/2412.06769)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/shawnricecake/Heima.svg?style=social&label=Star)](https://github.com/shawnricecake/Heima)<br>[Efficient Reasoning with Hidden Thinking](https://arxiv.org/abs/2501.19201) <br> Xuan Shen, Yizhou Wang, Xiangxi Shi, Yanzhi Wang, Pu Zhao, Jiuxiang Gu |<img width="1002" alt="image" src="https://arxiv.org/html/2501.19201v1/x1.png"> |[Github](https://github.com/shawnricecake/Heima) <br> [Paper](https://arxiv.org/abs/2501.19201)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2024-blue)]()<br>[Think before you speak: Training Language Models With Pause Tokens](https://arxiv.org/abs/2310.02226) <br> Sachin Goyal, Ziwei Ji, Ankit Singh Rawat, Aditya Krishna Menon, Sanjiv Kumar, Vaishnavh Nagarajan |<img width="1002" alt="image" src="figures/pause_token.png"> |[Paper](https://arxiv.org/abs/2310.02226)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/seal-rg/recurrent-pretraining.svg?style=social&label=Star)](https://github.com/seal-rg/recurrent-pretraining)<br>[Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach](https://arxiv.org/abs/2502.05171) <br> Jonas Geiping, Sean McLeish, Neel Jain, John Kirchenbauer, Siddharth Singh, Brian R. Bartoldson, Bhavya Kailkhura, Abhinav Bhatele, Tom Goldstein |<img width="1002" alt="image" src="https://arxiv.org/html/2502.05171v2/x2.png"> |[Github](https://github.com/seal-rg/recurrent-pretraining) <br> [Paper](https://arxiv.org/abs/2502.05171)| [//]: #04/08
|[Weight-of-Thought Reasoning: Exploring Neural Network Weights for Enhanced LLM Reasoning](https://arxiv.org/abs/2504.10646) <br> Saif Punjwani, Larry Heck |<img width="1002" alt="image" src="https://arxiv.org/html/2504.10646v1/extracted/6355099/cotvswot.png"> |[Paper](https://arxiv.org/abs/2504.10646)|[//]: #04/16


### Build SLM with Strong Reasoning Ability


#### Distillation 
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
| [![Publish](https://img.shields.io/badge/Conference-ACL_2023-blue)]()<br>[Teaching Small Language Models to Reason](https://arxiv.org/abs/2212.08410) <br> Lucie Charlotte Magister, Jonathan Mallinson, Jakub Adamek, Eric Malmi, Aliaksei Severyn |<img width="1002" alt="image" src="figures/slm_kd.png"> |[Paper](https://arxiv.org/abs/2212.08410)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2024-blue)]()<br>[Mixed Distillation Helps Smaller Language Model Better Reasoning](https://arxiv.org/abs/2312.10730) <br> Chenglin Li, Qianglong Chen, Liangyue Li, Caiyu Wang, Yicheng Li, Zulong Chen, Yin Zhang |<img width="1002" alt="image" src="figures/mix_distillation.png"> |[Paper](https://arxiv.org/abs/2312.10730)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Small-Model-Gap/Small-Model-Learnability-Gap.svg?style=social&label=Star)](https://github.com/Small-Model-Gap/Small-Model-Learnability-Gap)<br>[Small Models Struggle to Learn from Strong Reasoners](https://arxiv.org/abs/2502.12143) <br> Yuetai Li, Xiang Yue, Zhangchen Xu, Fengqing Jiang, Luyao Niu, Bill Yuchen Lin, Bhaskar Ramasubramanian, Radha Poovendran |<img width="1002" alt="image" src="https://arxiv.org/html/2502.12143v2/x1.png"> |[Github](https://github.com/Small-Model-Gap/Small-Model-Learnability-Gap) <br> [Paper](https://arxiv.org/abs/2502.12143)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Yiwei98/TDG.svg?style=social&label=Star)](https://github.com/Yiwei98/TDG) [![Publish](https://img.shields.io/badge/Conference-AAAI_2024-blue)]()<br>[Turning Dust into Gold: Distilling Complex Reasoning Capabilities from LLMs by Leveraging Negative Data](https://arxiv.org/abs/2312.12832) <br> Yiwei Li, Peiwen Yuan, Shaoxiong Feng, Boyuan Pan, Bin Sun, Xinglin Wang, Heda Wang, Kan Li |<img width="1002" alt="image" src="https://arxiv.org/html/2312.12832v1/x1.png"> |[Github](https://github.com/Yiwei98/TDG) <br> [Paper](https://arxiv.org/abs/2312.12832)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2024-blue)]()<br>[Teaching Small Language Models Reasoning through Counterfactual Distillation](https://aclanthology.org/2024.emnlp-main.333/) <br> Tao Feng, Yicheng Li, Li Chenglin, Hao Chen, Fei Yu, Yin Zhang |<img width="1002" alt="image" src="figures/counterfactual_distillation.png"> |[Paper](https://aclanthology.org/2024.emnlp-main.333/)| [//]: #04/08
|[Deconstructing Long Chain-of-Thought: A Structured Reasoning Optimization Framework for Long CoT Distillation](https://arxiv.org/abs/2503.16385) <br> Yijia Luo, Yulin Song, Xingyao Zhang, Jiaheng Liu, Weixun Wang, GengRu Chen, Wenbo Su, Bo Zheng |<img width="1002" alt="image" src="https://arxiv.org/html/2503.16385v1/x3.png"> |[Paper](https://arxiv.org/abs/2503.16385)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/yunx-z/SCORE.svg?style=social&label=Star)](https://github.com/yunx-z/SCORE) [![Publish](https://img.shields.io/badge/Conference-ACL_Findings_2024-blue)]()<br>[Small Language Models Need Strong Verifiers to Self-Correct Reasoning](https://arxiv.org/abs/2404.17140) <br> Yunxiang Zhang, Muhammad Khalifa, Lajanugen Logeswaran, Jaekyeom Kim, Moontae Lee, Honglak Lee, Lu Wang |<img width="1002" alt="image" src="https://arxiv.org/html/2404.17140v2/x1.png"> |[Github](https://github.com/yunx-z/SCORE) <br> [Paper](https://arxiv.org/abs/2404.17140)| [//]: #04/08
|[Improving Mathematical Reasoning Capabilities of Small Language Models via Feedback-Driven Distillation](https://arxiv.org/abs/2411.14698) <br> Xunyu Zhu, Jian Li, Can Ma, Weiping Wang |<img width="1002" alt="image" src="https://arxiv.org/html/2411.14698v1/x1.png"> |[Paper](https://arxiv.org/abs/2411.14698)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Xnhyacinth/SKIntern.svg?style=social&label=Star)](https://github.com/Xnhyacinth/SKIntern) [![Publish](https://img.shields.io/badge/Conference-COLING_2025-blue)]()<br>[SKIntern : Internalizing Symbolic Knowledge for Distilling Better CoT Capabilities into Small Language Models](https://arxiv.org/abs/2409.13183) <br> Huanxuan Liao, Shizhu He, Yupu Hao, Xiang Li, Yuanzhe Zhang, Jun Zhao, Kang Liu |<img width="1002" alt="image" src="https://arxiv.org/html/2409.13183v2/x1.png"> |[Github](https://github.com/Xnhyacinth/SKIntern) <br> [Paper](https://arxiv.org/abs/2409.13183)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-COLING_2024-blue)]()<br>[Probe then Retrieve and Reason: Distilling Probing and Reasoning Capabilities into Smaller Language Models](https://aclanthology.org/2024.lrec-main.1140.pdf) <br> Yichun Zhao, Shuheng Zhou, Huijia Zhu |<img width="1002" alt="image" src="figures/prr.png"> |[Paper](https://aclanthology.org/2024.lrec-main.1140.pdf)| [//]: #04/08
|[Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners](https://arxiv.org/abs/2502.20339) <br> Daniele Paliotta, Junxiong Wang, Matteo Pagliardini, Kevin Y. Li, Aviv Bick, J. Zico Kolter, Albert Gu, François Fleuret, Tri Dao |<img width="1002" alt="image" src="https://arxiv.org/html/2502.20339v1/x1.png"> |[Paper](https://arxiv.org/abs/2502.20339)| [//]: #04/08
|[Distilling Reasoning Ability from Large Language Models with Adaptive Thinking](https://arxiv.org/abs/2404.09170) <br> Xiaoshu Chen, Sihang Zhou, Ke Liang, Xinwang Liu |<img width="1002" alt="image" src="https://arxiv.org/html/2404.09170v5/x1.png"> |[Paper](https://arxiv.org/abs/2404.09170)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/EIT-NLP/Distilling-CoT-Reasoning.svg?style=social&label=Star)](https://github.com/EIT-NLP/Distilling-CoT-Reasoning)<br>[Unveiling the Key Factors for Distilling Chain-of-Thought Reasoning](https://arxiv.org/abs/2502.18001) <br> Xinghao Chen, Zhijing Sun, Wenjin Guo, Miaoran Zhang, Yanjun Chen, Yirong Sun, Hui Su, Yijie Pan, Dietrich Klakow, Wenjie Li, Xiaoyu Shen |<img width="1002" alt="image" src="https://arxiv.org/html/2502.18001v1/x1.png"> |[Github](https://github.com/EIT-NLP/Distilling-CoT-Reasoning) <br> [Paper](https://arxiv.org/abs/2502.18001)| [//]: #04/08

#### Quantization and Pruning
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[Towards Reasoning Ability of Small Language Models](https://arxiv.org/abs/2502.11569) <br> Gaurav Srivastava, Shuxiang Cao, Xuan Wang |<img width="1002" alt="image" src="figures/slm_reasoning.png"> |[Paper](https://arxiv.org/abs/2502.11569)| [//]: #04/14
|[![Star](https://img.shields.io/github/stars/ruikangliu/Quantized-Reasoning-Models.svg?style=social&label=Star)](https://github.com/ruikangliu/Quantized-Reasoning-Models)<br>[Quantization Hurts Reasoning? An Empirical Study on Quantized Reasoning Models](https://arxiv.org/abs/2504.04823) <br> Ruikang Liu, Yuxuan Sun, Manyi Zhang, Haoli Bai, Xianzhi Yu, Tiezheng Yu, Chun Yuan, Lu Hou |<img width="1002" alt="image" src="figures/quant_hurt.png"> |[Github](https://github.com/ruikangliu/Quantized-Reasoning-Models) <br> [Paper](https://arxiv.org/abs/2504.04823)| [//]: #04/14
|[When Reasoning Meets Compression: Benchmarking Compressed Large Reasoning Models on Complex Reasoning Tasks](https://arxiv.org/abs/2504.02010) <br> Nan Zhang, Yusen Zhang, Prasenjit Mitra, Rui Zhang |<img width="1002" alt="image" src="figures/when_compression.png"> |[Paper](https://arxiv.org/abs/2504.02010)| [//]: #04/14



#### RL-based Methods
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/knoveleng/open-rs.svg?style=social&label=Star)](https://github.com/knoveleng/open-rs)<br>[Reinforcement Learning for Reasoning in Small LLMs: What Works and What Doesn't](https://arxiv.org/abs/2503.16219) <br> Quy-Anh Dang, Chris Ngo |<img src="https://arxiv.org/html/2503.16219v1/extracted/6296504/images/pass1.png" width="45%"> <img src="https://arxiv.org/html/2503.16219v1/extracted/6296504/images/costs.png" width="45%"> |[Github](https://github.com/knoveleng/open-rs) <br> [Paper](https://arxiv.org/abs/2503.16219)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/hkust-nlp/simpleRL-reason.svg?style=social&label=Star)](https://github.com/hkust-nlp/simpleRL-reason)<br>[SimpleRL-Zoo: Investigating and Taming Zero Reinforcement Learning for Open Base Models in the Wild](https://arxiv.org/abs/2503.18892) <br> Weihao Zeng, Yuzhen Huang, Qian Liu, Wei Liu, Keqing He, Zejun Ma, Junxian He |<img width="1002" alt="image" src="figures/simplerl_zoo.png"> |[Github](https://github.com/hkust-nlp/simpleRL-reason) <br> [Paper](https://arxiv.org/abs/2503.18892)| [//]: #04/08

###### Repo

* [DeepScaleR](https://github.com/agentica-project/deepscaler). DeepScaleR team. [Webpage](https://agentica-project.com/)



### Let Decoding More Efficient


#### Efficient TTS
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/Pranjal2041/AdaptiveConsistency.svg?style=social&label=Star)](https://github.com/Pranjal2041/AdaptiveConsistency)<br>[Let's Sample Step by Step: Adaptive-Consistency for Efficient Reasoning and Coding with LLMs](https://arxiv.org/abs/2305.11860) <br> Pranjal Aggarwal, Aman Madaan, Yiming Yang, Mausam |<img width="1002" alt="image" src="figures/asc.png"> |[Github](https://github.com/Pranjal2041/AdaptiveConsistency) <br> [Paper](https://arxiv.org/abs/2305.11860)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Yiwei98/ESC.svg?style=social&label=Star)](https://github.com/Yiwei98/ESC) [![Publish](https://img.shields.io/badge/Conference-ICLR_2024-blue)]()<br>[Escape Sky-high Cost: Early-stopping Self-Consistency for Multi-step Reasoning](https://arxiv.org/abs/2401.10480) <br> Yiwei Li, Peiwen Yuan, Shaoxiong Feng, Boyuan Pan, Xinglin Wang, Bin Sun, Heda Wang, Kan Li |<img width="1002" alt="image" src="https://arxiv.org/html/2401.10480v1/x1.png"> |[Github](https://github.com/Yiwei98/ESC) <br> [Paper](https://arxiv.org/abs/2401.10480)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/WangXinglin/DSC.svg?style=social&label=Star)](https://github.com/WangXinglin/DSC) [![Publish](https://img.shields.io/badge/Conference-NAACL_Findings_2025-blue)]()<br>[Make Every Penny Count: Difficulty-Adaptive Self-Consistency for Cost-Efficient Reasoning](https://arxiv.org/abs/2408.13457) <br> Xinglin Wang, Shaoxiong Feng, Yiwei Li, Peiwen Yuan, Yueqi Zhang, Chuyi Tan, Boyuan Pan, Yao Hu, Kan Li |<img width="1002" alt="image" src="https://arxiv.org/html/2408.13457v3/x3.png"> |[Github](https://github.com/WangXinglin/DSC) <br> [Paper](https://arxiv.org/abs/2408.13457)| [//]: #04/08
|[Path-Consistency: Prefix Enhancement for Efficient Inference in LLM](https://arxiv.org/abs/2409.01281) <br> Jiace Zhu, Yingtao Shen, Jie Zhao, An Zou |<img width="1002" alt="image" src="https://arxiv.org/html/2409.01281v2/x1.png"> |[Paper](https://arxiv.org/abs/2409.01281)| [//]: #04/08
|[Bridging Internal Probability and Self-Consistency for Effective and Efficient LLM Reasoning](https://arxiv.org/abs/2502.00511) <br> Zhi Zhou, Tan Yuhao, Zenan Li, Yuan Yao, Lan-Zhe Guo, Xiaoxing Ma, Yu-Feng Li |<img width="1002" alt="image" src="https://arxiv.org/html/2502.00511v2/x3.png"> |[Paper](https://arxiv.org/abs/2502.00511)| [//]: #04/08
|[Confidence Improves Self-Consistency in LLMs](https://arxiv.org/abs/2502.06233) <br> Amir Taubenfeld, Tom Sheffer, Eran Ofek, Amir Feder, Ariel Goldstein, Zorik Gekhman, Gal Yona |<img width="1002" alt="image" src="figures/cisc.png"> |[Paper](https://arxiv.org/abs/2502.06233)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Chengsong-Huang/Self-Calibration.svg?style=social&label=Star)](https://github.com/Chengsong-Huang/Self-Calibration)<br>[Efficient Test-Time Scaling via Self-Calibration](https://arxiv.org/abs/2503.00031) <br> Chengsong Huang, Langlin Huang, Jixuan Leng, Jiacheng Liu, Jiaxin Huang |<img width="1002" alt="image" src="https://arxiv.org/html/2503.00031v1/x2.png"> |[Github](https://github.com/Chengsong-Huang/Self-Calibration) <br> [Paper](https://arxiv.org/abs/2503.00031)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Zanette-Labs/SpeculativeRejection.svg?style=social&label=Star)](https://github.com/Zanette-Labs/SpeculativeRejection) [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2024-blue)]()<br>[Fast Best-of-N Decoding via Speculative Rejection](https://arxiv.org/abs/2410.20290) <br> Hanshi Sun, Momin Haider, Ruiqi Zhang, Huitao Yang, Jiahao Qiu, Ming Yin, Mengdi Wang, Peter Bartlett, Andrea Zanette |<img width="1002" alt="image" src="https://arxiv.org/html/2410.20290v2/x1.png"> |[Github](https://github.com/Zanette-Labs/SpeculativeRejection) <br> [Paper](https://arxiv.org/abs/2410.20290)| [//]: #04/08
|[Sampling-Efficient Test-Time Scaling: Self-Estimating the Best-of-N Sampling in Early Decoding](https://arxiv.org/abs/2503.01422) <br> Yiming Wang, Pei Zhang, Siyuan Huang, Baosong Yang, Zhuosheng Zhang, Fei Huang, Rui Wang |<img width="1002" alt="image" src="https://arxiv.org/html/2503.01422v1/x1.png"> |[Paper](https://arxiv.org/abs/2503.01422)| [//]: #04/08
|[FastMCTS: A Simple Sampling Strategy for Data Synthesis](https://www.arxiv.org/abs/2502.11476) <br> Peiji Li, Kai Lv, Yunfan Shao, Yichuan Ma, Linyang Li, Xiaoqing Zheng, Xipeng Qiu, Qipeng Guo |<img width="1002" alt="image" src="https://arxiv.org/html/2502.11476v1/x2.png"> |[Paper](https://www.arxiv.org/abs/2502.11476)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/chang-github-00/LLM-Predictive-Decoding.svg?style=social&label=Star)](https://github.com/chang-github-00/LLM-Predictive-Decoding) [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br>[Non-myopic Generation of Language Models for Reasoning and Planning](https://arxiv.org/abs/2410.17195) <br> Chang Ma, Haiteng Zhao, Junlei Zhang, Junxian He, Lingpeng Kong |<img width="1002" alt="image" src="figures/predictive_decoding.png"> |[Github](https://github.com/chang-github-00/LLM-Predictive-Decoding) <br> [Paper](https://arxiv.org/abs/2410.17195)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/ethanm88/self-taught-lookahead.svg?style=social&label=Star)](https://github.com/ethanm88/self-taught-lookahead)<br>[Language Models can Self-Improve at State-Value Estimation for Better Search](https://arxiv.org/abs/2503.02878) <br> Ethan Mendes, Alan Ritter |<img width="1002" alt="image" src="https://arxiv.org/html/2503.02878v1/x1.png"> |[Github](https://github.com/ethanm88/self-taught-lookahead) <br> [Paper](https://arxiv.org/abs/2503.02878)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/xufangzhi/phi-Decoding.svg?style=social&label=Star)](https://github.com/xufangzhi/phi-Decoding)<br>[ϕ-Decoding: Adaptive Foresight Sampling for Balanced Inference-Time Exploration and Exploitation](https://arxiv.org/abs/2503.13288) <br> Fangzhi Xu, Hang Yan, Chang Ma, Haiteng Zhao, Jun Liu, Qika Lin, Zhiyong Wu |<img width="1002" alt="image" src="https://arxiv.org/html/2503.13288v1/x2.png"> |[Github](https://github.com/xufangzhi/phi-Decoding) <br> [Paper](https://arxiv.org/abs/2503.13288)| [//]: #04/08
|[Dynamic Parallel Tree Search for Efficient LLM Reasoning](https://arxiv.org/abs/2502.16235) <br> Yifu Ding, Wentao Jiang, Shunyu Liu, Yongcheng Jing, Jinyang Guo, Yingjie Wang, Jing Zhang, Zengmao Wang, Ziwei Liu, Bo Du, Xianglong Liu, Dacheng Tao |<img width="1002" alt="image" src="https://arxiv.org/html/2502.16235v2/x5.png"> |[Paper](https://arxiv.org/abs/2502.16235)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Soistesimmer/Fetch.svg?style=social&label=Star)](https://github.com/Soistesimmer/Fetch)<br>[Don't Get Lost in the Trees: Streamlining LLM Reasoning by Overcoming Tree Search Exploration Pitfalls](https://arxiv.org/abs/2502.11183) <br> Ante Wang, Linfeng Song, Ye Tian, Dian Yu, Haitao Mi, Xiangyu Duan, Zhaopeng Tu, Jinsong Su, Dong Yu |<img width="1002" alt="image" src="https://arxiv.org/html/2502.11183v2/extracted/6301324/figures/method.png"> |[Github](https://github.com/Soistesimmer/Fetch) <br> [Paper](https://arxiv.org/abs/2502.11183)| [//]: #04/08



#### Other Optimal Methods
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/imagination-research/sot.svg?style=social&label=Star)](https://github.com/imagination-research/sot) [![Publish](https://img.shields.io/badge/Conference-ICLR_2024-blue)]()<br>[Skeleton-of-Thought: Prompting LLMs for Efficient Parallel Generation](https://arxiv.org/abs/2307.15337) <br> Xuefei Ning, Zinan Lin, Zixuan Zhou, Zifu Wang, Huazhong Yang, Yu Wang |<img width="1002" alt="image" src="figures/skeleton_ot.png"> |[Github](https://github.com/imagination-research/sot) <br> [Paper](https://arxiv.org/abs/2307.15337)| [//]: #04/08
|[Adaptive Skeleton Graph Decoding](https://arxiv.org/abs/2402.12280) <br> Shuowei Jin, Yongji Wu, Haizhong Zheng, Qingzhao Zhang, Matthew Lentz, Z. Morley Mao, Atul Prakash, Feng Qian, Danyang Zhuo |<img width="1002" alt="image" src="figures/sgd.png"> |[Paper](https://arxiv.org/abs/2402.12280)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/BaohaoLiao/RSD.svg?style=social&label=Star)](https://github.com/BaohaoLiao/RSD)<br>[Reward-Guided Speculative Decoding for Efficient LLM Reasoning](https://arxiv.org/abs/2501.19324) <br> Baohao Liao, Yuhui Xu, Hanze Dong, Junnan Li, Christof Monz, Silvio Savarese, Doyen Sahoo, Caiming Xiong |<img width="1002" alt="image" src="figures/rsd.png"> |[Github](https://github.com/BaohaoLiao/RSD) <br> [Paper](https://arxiv.org/abs/2501.19324)| [//]: #04/08
|[Meta-Reasoner: Dynamic Guidance for Optimized Inference-time Reasoning in Large Language Models](https://arxiv.org/abs/2502.19918) <br> Yuan Sui, Yufei He, Tri Cao, Simeng Han, Bryan Hooi |<img width="1002" alt="image" src="figures/meta_reasoner.png"> |[Paper](https://arxiv.org/abs/2502.19918)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/qixucen/atom.svg?style=social&label=Star)](https://github.com/qixucen/atom)<br>[Atom of Thoughts for Markov LLM Test-Time Scaling](https://arxiv.org/abs/2502.12018) <br> Fengwei Teng, Zhaoyang Yu, Quan Shi, Jiayi Zhang, Chenglin Wu, Yuyu Luo |<img width="1002" alt="image" src="figures/aot.png"> |[Github](https://github.com/qixucen/atom) <br> [Paper](https://arxiv.org/abs/2502.12018)| [//]: #04/08
|[DISC: Dynamic Decomposition Improves LLM Inference Scaling](https://arxiv.org/abs/2502.16706) <br> Jonathan Light, Wei Cheng, Wu Yue, Masafumi Oyamada, Mengdi Wang, Santiago Paternain, Haifeng Chen |<img width="1002" alt="image" src="figures/disc.png"> |[Paper](https://arxiv.org/abs/2502.16706)| [//]: #04/08
|[From Chaos to Order: The Atomic Reasoner Framework for Fine-grained Reasoning in Large Language Models](https://arxiv.org/abs/2503.15944) <br> Jinyi Liu, Yan Zheng, Rong Cheng, Qiyu Wu, Wei Guo, Fei Ni, Hebin Liang, Yifu Yuan, Hangyu Mao, Fuzheng Zhang, Jianye Hao |<img width="1002" alt="image" src="figures/ar.png"> |[Paper](https://arxiv.org/abs/2503.15944)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/Quinn777/AtomThink.svg?style=social&label=Star)](https://github.com/Quinn777/AtomThink)<br>[Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?](https://arxiv.org/abs/2503.06252) <br> Kun Xiang, Zhili Liu, Zihao Jiang, Yunshuang Nie, Kaixin Cai, Yiyang Yin, Runhui Huang, Haoxiang Fan, Hanhui Li, Weiran Huang, Yihan Zeng, Yu-Jie Yuan, Jianhua Han, Lanqing Hong, Hang Xu, Xiaodan Liang |<img width="1002" alt="image" src="figures/atom.png"> |[Github](https://github.com/Quinn777/AtomThink) <br> [Paper](https://arxiv.org/abs/2503.06252)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br>[Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters](https://arxiv.org/abs/2408.03314) <br> Charlie Snell, Jaehoon Lee, Kelvin Xu, Aviral Kumar |<img width="1002" alt="image" src="figures/tts_effective.png"> |[Paper](https://arxiv.org/abs/2408.03314)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/thu-wyz/inference_scaling.svg?style=social&label=Star)](https://github.com/thu-wyz/inference_scaling) [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br>[Inference Scaling Laws: An Empirical Analysis of Compute-Optimal Inference for Problem-Solving with Language Models](https://arxiv.org/abs/2408.00724) <br> Yangzhen Wu, Zhiqing Sun, Shanda Li, Sean Welleck, Yiming Yang |<img width="1002" alt="image" src="figures/scaling_law.png"> |[Github](https://github.com/thu-wyz/inference_scaling) <br> [Paper](https://arxiv.org/abs/2408.00724)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/CMU-AIRe/MRT.svg?style=social&label=Star)](https://github.com/CMU-AIRe/MRT)<br>[Optimizing Test-Time Compute via Meta Reinforcement Fine-Tuning](https://arxiv.org/abs/2503.07572) <br> Yuxiao Qu, Matthew Y. R. Yang, Amrith Setlur, Lewis Tunstall, Edward Emanuel Beeching, Ruslan Salakhutdinov, Aviral Kumar |<img width="1002" alt="image" src="figures/mrt.png"> |[Github](https://github.com/CMU-AIRe/MRT) <br> [Paper](https://arxiv.org/abs/2503.07572)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/ruipeterpan/specreason.svg?style=social&label=Star)](https://github.com/ruipeterpan/specreason)<br>[SpecReason: Fast and Accurate Inference-Time Compute via Speculative Reasoning](https://arxiv.org/abs/2504.07891) <br> Rui Pan, Yinwei Dai, Zhihao Zhang, Gabriele Oliaro, Zhihao Jia, Ravi Netravali |<img width="1002" alt="image" src="figures/specreason.png"> |[Github](https://github.com/ruipeterpan/specreason) <br> [Paper](https://arxiv.org/abs/2504.07891)| [//]: #04/14

### Evaluation and Benchmarks


#### Metric
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs](https://arxiv.org/abs/2412.21187) <br> Xingyu Chen, Jiahao Xu, Tian Liang, Zhiwei He, Jianhui Pang, Dian Yu, Linfeng Song, Qiuzhi Liu, Mengfei Zhou, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu |<img width="1002" alt="image" src="https://arxiv.org/html/2412.21187v2/x2.png"> |[Paper](https://arxiv.org/abs/2412.21187)|[//]: #03/16
|[![Star](https://img.shields.io/github/stars/horseee/CoT-Valve.svg?style=social&label=Star)](https://github.com/horseee/CoT-Valve)<br>[CoT-Valve: Length-Compressible Chain-of-Thought Tuning](https://arxiv.org/abs/2502.09601) <br> Xinyin Ma, Guangnian Wan, Runpeng Yu, Gongfan Fang, Xinchao Wang |<img width="1002" alt="image" src="figures/cot_valve.png"> |[Github](https://github.com/horseee/CoT-Valve) <br> [Paper](https://arxiv.org/abs/2502.09601)|[//]: #03/16
|[![Star](https://img.shields.io/github/stars/breckbaldwin/llm-stability.svg?style=social&label=Star)](https://github.com/breckbaldwin/llm-stability)<br>[Non-Determinism of "Deterministic" LLM Settings](https://arxiv.org/abs/2408.04667) <br> Berk Atil, Sarp Aykent, Alexa Chittams, Lisheng Fu, Rebecca J. Passonneau, Evan Radcliffe, Guru Rajan Rajagopal, Adam Sloan, Tomasz Tudrej, Ferhan Ture, Zhe Wu, Lixinyu Xu, Breck Baldwin |<img width="1002" alt="image" src="https://arxiv.org/html/2408.04667v5/extracted/6331111/max_min_diff.png"> |[Github](https://github.com/breckbaldwin/llm-stability) <br> [Paper](https://arxiv.org/abs/2408.04667)| [//]: #04/08
|[The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks](https://arxiv.org/abs/2502.08235) <br> Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang, Yichuan Wang, Siyuan Zhuang, Shu Liu, Luis Gaspar Schroeder, Tian Xia, Huanzhi Mao, Nicholas Thumiger, Aditya Desai, Ion Stoica, Ana Klimovic, Graham Neubig, Joseph E. Gonzalez |<img width="1002" alt="image" src="figures/openhands.png"> |[Paper](https://arxiv.org/abs/2502.08235)| [//]: #04/08
|[Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374) <br> Mark Chen, Jerry Tworek, et al. |<img width="1002" alt="image" src="figures/passk.png"> |[Paper](https://arxiv.org/abs/2107.03374)| [//]: #04/08
|[τ-bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains](https://arxiv.org/abs/2406.12045) <br> Shunyu Yao, Noah Shinn, Pedram Razavi, Karthik Narasimhan |<img width="1002" alt="image" src="figures/agent_bench.png"> |[Paper](https://arxiv.org/abs/2406.12045)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/open-compass/GPassK.svg?style=social&label=Star)](https://github.com/open-compass/GPassK)<br>[Are Your LLMs Capable of Stable Reasoning?](https://arxiv.org/abs/2412.13147) <br> Junnan Liu, Hongwei Liu, Linchen Xiao, Ziyi Wang, Kuikun Liu, Songyang Gao, Wenwei Zhang, Songyang Zhang, Kai Chen |<img width="1002" alt="image" src="https://arxiv.org/html/2412.13147v3/x1.png"> |[Github](https://github.com/open-compass/GPassK) <br> [Paper](https://arxiv.org/abs/2412.13147)| [//]: #04/08


#### Benchmark
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs](https://arxiv.org/abs/2412.21187) <br> Xingyu Chen, Jiahao Xu, Tian Liang, Zhiwei He, Jianhui Pang, Dian Yu, Linfeng Song, Qiuzhi Liu, Mengfei Zhou, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu |<img width="1002" alt="image" src="https://arxiv.org/html/2412.21187v2/x2.png"> |[Paper](https://arxiv.org/abs/2412.21187)|[//]: #03/16
|[The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks](https://arxiv.org/abs/2502.08235) <br> Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang, Yichuan Wang, Siyuan Zhuang, Shu Liu, Luis Gaspar Schroeder, Tian Xia, Huanzhi Mao, Nicholas Thumiger, Aditya Desai, Ion Stoica, Ana Klimovic, Graham Neubig, Joseph E. Gonzalez |<img width="1002" alt="image" src="figures/openhands.png"> |[Paper](https://arxiv.org/abs/2502.08235)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/divelab/sys2bench.svg?style=social&label=Star)](https://github.com/divelab/sys2bench)<br>[Inference-Time Computations for LLM Reasoning and Planning: A Benchmark and Insights](https://arxiv.org/abs/2502.12521) <br> Shubham Parashar, Blake Olson, Sambhav Khurana, Eric Li, Hongyi Ling, James Caverlee, Shuiwang Ji |<img width="1002" alt="image" src="https://arxiv.org/html/2502.12521v1/x1.png"> |[Github](https://github.com/divelab/sys2bench) <br> [Paper](https://arxiv.org/abs/2502.12521)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/usail-hkust/benchmark_inference_time_computation_LLM.svg?style=social&label=Star)](https://github.com/usail-hkust/benchmark_inference_time_computation_LLM)<br>[Bag of Tricks for Inference-time Computation of LLM Reasoning](https://arxiv.org/abs/2502.07191) <br> Fan Liu, Wenshuo Chao, Naiqiang Tan, Hao Liu |<img width="1002" alt="image" src="https://arxiv.org/html/2502.07191v4/x1.png"> |[Github](https://github.com/usail-hkust/benchmark_inference_time_computation_LLM) <br> [Paper](https://arxiv.org/abs/2502.07191)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/RyanLiu112/compute-optimal-tts.svg?style=social&label=Star)](https://github.com/RyanLiu112/compute-optimal-tts)<br>[Can 1B LLM Surpass 405B LLM? Rethinking Compute-Optimal Test-Time Scaling](https://arxiv.org/abs/2502.06703) <br> Runze Liu, Junqi Gao, Jian Zhao, Kaiyan Zhang, Xiu Li, Biqing Qi, Wanli Ouyang, Bowen Zhou |<img width="1002" alt="image" src="https://arxiv.org/html/2502.06703v1/x2.png"> |[Github](https://github.com/RyanLiu112/compute-optimal-tts) <br> [Paper](https://arxiv.org/abs/2502.06703)| [//]: #04/08
|[DNA Bench: When Silence is Smarter -- Benchmarking Over-Reasoning in Reasoning LLMs](https://arxiv.org/abs/2503.15793) <br> Masoud Hashemi, Oluwanifemi Bamgbose, Sathwik Tejaswi Madhusudhan, Jishnu Sethumadhavan Nair, Aman Tiwari, Vikas Yadav |<img width="1002" alt="image" src="https://arxiv.org/html/2503.15793v3/x5.png"> |[Paper](https://arxiv.org/abs/2503.15793)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/zhishuifeiqian/VCR-Bench.svg?style=social&label=Star)](https://github.com/zhishuifeiqian/VCR-Bench)<br>[VCR-Bench: A Comprehensive Evaluation Framework for Video Chain-of-Thought Reasoning](https://arxiv.org/abs/2504.07956) <br> Yukun Qi, Yiming Zhao, Yu Zeng, Xikun Bao, Wenxuan Huang, Lin Chen, Zehui Chen, Jie Zhao, Zhongang Qi, Feng Zhao |<img width="1002" alt="image" src="figures/video.png"> |[Github](https://github.com/zhishuifeiqian/VCR-Bench) <br> [Paper](https://arxiv.org/abs/2504.07956)| [//]: #04/16

### Background Papers
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
| [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2022-blue)]()<br>[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903) <br> Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed Chi, Quoc Le, Denny Zhou |<img width="1002" alt="image" src="figures/cot_prompting.png"> |[Paper](https://arxiv.org/abs/2201.11903)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/princeton-nlp/tree-of-thought-llm.svg?style=social&label=Star)](https://github.com/princeton-nlp/tree-of-thought-llm) [![Publish](https://img.shields.io/badge/Conference-NeurIPS_2023-blue)]()<br>[Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/abs/2305.10601) <br> Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Thomas L. Griffiths, Yuan Cao, Karthik Narasimhan |<img width="1002" alt="image" src="https://arxiv.org/html/2305.10601v2/x1.png"> |[Github](https://github.com/princeton-nlp/tree-of-thought-llm) <br> [Paper](https://arxiv.org/abs/2305.10601)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/spcl/graph-of-thoughts.svg?style=social&label=Star)](https://github.com/spcl/graph-of-thoughts) [![Publish](https://img.shields.io/badge/Conference-AAAI_2024-blue)]()<br>[Graph of Thoughts: Solving Elaborate Problems with Large Language Models](https://arxiv.org/abs/2308.09687) <br> Maciej Besta, Nils Blach, Ales Kubicek, Robert Gerstenberger, Michal Podstawski, Lukas Gianinazzi, Joanna Gajda, Tomasz Lehmann, Hubert Niewiadomski, Piotr Nyczyk, Torsten Hoefler |<img width="1002" alt="image" src="figures/got.png"> |[Github](https://github.com/spcl/graph-of-thoughts) <br> [Paper](https://arxiv.org/abs/2308.09687)| [//]: #04/08
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2023-blue)]()<br>[Self-Consistency Improves Chain of Thought Reasoning in Language Models](https://arxiv.org/abs/2203.11171) <br> Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Sharan Narang, Aakanksha Chowdhery, Denny Zhou |<img width="1002" alt="image" src="figures/sc.png"> |[Paper](https://arxiv.org/abs/2203.11171)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/TIGER-AI-Lab/Program-of-Thoughts.svg?style=social&label=Star)](https://github.com/TIGER-AI-Lab/Program-of-Thoughts) [![Publish](https://img.shields.io/badge/Conference-TMLR_2023-blue)]()<br>[Program of Thoughts Prompting: Disentangling Computation from Reasoning for Numerical Reasoning Tasks](https://arxiv.org/abs/2211.12588) <br> Wenhu Chen, Xueguang Ma, Xinyi Wang, William W. Cohen |<img width="1002" alt="image" src="figures/pot.png"> |[Github](https://github.com/TIGER-AI-Lab/Program-of-Thoughts) <br> [Paper](https://arxiv.org/abs/2211.12588)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/hanxuhu/chain-of-symbol-planning.svg?style=social&label=Star)](https://github.com/hanxuhu/chain-of-symbol-planning) [![Publish](https://img.shields.io/badge/Conference-COLM_2024-blue)]()<br>[Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models](https://arxiv.org/abs/2305.10276) <br> Hanxu Hu, Hongyuan Lu, Huajian Zhang, Yun-Ze Song, Wai Lam, Yue Zhang |<img width="1002" alt="image" src="https://arxiv.org/html/2305.10276v7/x1.png"> |[Github](https://github.com/hanxuhu/chain-of-symbol-planning) <br> [Paper](https://arxiv.org/abs/2305.10276)| [//]: #04/08

###### Survey
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[Thinking Machines: A Survey of LLM based Reasoning Strategies](https://arxiv.org/abs/2503.10814) <br> Dibyanayan Bandyopadhyay, Soham Bhattacharjee, Asif Ekbal |<img width="1002" alt="image" src="https://arxiv.org/html/2503.10814v1/x1.png"> |[Paper](https://arxiv.org/abs/2503.10814)| [//]: #04/08
|[![Star](https://img.shields.io/github/stars/zzli2022/Awesome-System2-Reasoning-LLM.svg?style=social&label=Star)](https://github.com/zzli2022/Awesome-System2-Reasoning-LLM)<br>[From System 1 to System 2: A Survey of Reasoning Large Language Models](https://arxiv.org/abs/2502.17419) <br> Zhong-Zhi Li, Duzhen Zhang, Ming-Liang Zhang, Jiaxin Zhang, Zengyan Liu, Yuxuan Yao, Haotian Xu, Junhao Zheng, Pei-Jie Wang, Xiuyi Chen, Yingying Zhang, Fei Yin, Jiahua Dong, Zhijiang Guo, Le Song, Cheng-Lin Liu |<img width="1002" alt="image" src="https://arxiv.org/html/2502.17419v2/extracted/6232702/images/timeline.png"> |[Github](https://github.com/zzli2022/Awesome-System2-Reasoning-LLM) <br> [Paper](https://arxiv.org/abs/2502.17419)| [//]: #04/08



## Acknowledgement

This repository is inspired by [Awesome-Efficient-LLM](https://github.com/horseee/Awesome-Efficient-LLM/)


## Citation

```bibtex
@article{,
    title={Efficient Reasoning Models: A Survey},
    author={Feng, Sicheng and Fang, Gongfan and Ma, Xinyin and Wang, Xinchao},
    journal={arXiv preprint arXiv:2504.10903},
    year={2025},
}
```
