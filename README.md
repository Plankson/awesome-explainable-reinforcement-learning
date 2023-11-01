# Awesome Explainable Reinforcement Learning


[![arXiv](https://img.shields.io/badge/arXiv-2211.06665-b31b1b.svg)](https://arxiv.org/abs/2211.06665)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Awesome XRL](https://img.shields.io/badge/Awesome-XRL-blue)](https://github.com/topics/awesome)
[![Document](https://img.shields.io/badge/Document-Yes-green)](https://github.com/topics/document)

A list of selected paper and possible corresponding codes in our review paper [A Survey on Explainable Reinforcement Learning: Concepts, Algorithms, Challenges](https://arxiv.org/abs/2211.06665).

*If you find there is a missed paper or a possible mistake in our survey, please feel free to email me (<qingyunpeng@zju.edu.cn>) or pull a request here. I am more than glad to receive your advice. Thanks!*

## Citation

If you find this survey useful for your research, please consider citing

```
@article{qing2022XRLsurvey,
  title={A Survey on Explainable Reinforcement Learning: Concepts, Algorithms, Challenges},
  author={Qing, Yunpeng and Liu, Shunyu and Song, Jie and Wang, Huiqiong and Song, Mingli},
  journal={arXiv preprint arXiv:2211.06665},
  year={2022}
}
```

## Table of Contents

- [Overview](#Overview)
- [Surveys](#Surveys)
- [Explainability in RL](#Explainability-in-RL)
  - [Agent Model Explaining](#Agent-Model-Explaining)
  - [Reward Explaining](#Reward-Explaining)
  - [State Explaining](#State-Explaining)
  - [Task Explaining](#Task-Explaining)

- [Human knowledge for RL paradigm](#Human-knowledge-for-RL-paradigm)

- [Explainable AI Library](#A-summary-of-Explainable-AI-library)

## ✨ Overview

- [x] **📖 RL paradigm-based Explainable RL Taxonomy**
- [x] **👓 Review of human knowledge-based RL explainability**
- [x] **🚀 List of Current XRL research literatures and codes links** 
<!-- We review current explainable reinforcement learning framework and explainability of human knowledge-based reinforcement learning framework. We creatively propose a new taxonomy for existing explainable reinforcement learning based on reinforcement learning paradigm. Specifically, we divide existing explainable reinforcement learning methods into four categories: agent model-explaining, reward-explaining, state-explaining, task-explaining as shown below: -->

<div align="center">
<img src="https://github.com/plankson/awesome-explainable-reinforcement-learning/blob/main/Fig/categorize.png" width="100%">
</div>

The Figure above illustrate how to enhance explainability to different part of RL paradigm, which include model(agent), reward, state and the task itself.
<!-- - Agent Model Explaining: trains the agent to be explainable by having understandable logic operation in its inner structure
- Reward Explaining: reconstructs reward function towards an explainable one $r'_t$  and makes it possible to see how the goal influences the agent
- State Explaining: adds a submodule for introspection to quantify the influences of different state features towards the decision-making as $w(s_{t'})$.
- Task Explaining: gets an architectural level explainability in complex environments by multilevel agents, the high-level agent schedule low-level agents by the subgoal signal $g_t$ which could be utilized for explanations.
 -->
 
To know more about existing XRL framework and our taxonomy, the existing XRL papers within different typs are listed below and summerized in the next Figure. These literatures are categorize into our taxonomy. For each paper, we provide the soure file and the project code if the paper has source code and the code is pubilic. 


<div align="center">
<img src="https://github.com/plankson/awesome-explainable-reinforcement-learning/blob/main/Fig/Taxonomy.png" width="100%">
</div>


## 📝 Surveys

- Explainable Reinforcement Learning: A Survey
  - E. Puiutta and E. Veith.  *CD-MAKE 2020*.  [[paper]](https://arxiv.org/pdf/2005.06247.pdf)
- A Survey on Interpretable Reinforcement Learning
  - C. Glanois, P. Weng, M. Zimmer, D. Li, T. Yang,  J. Hao and W. Liu.  *arXiv 2021*.  [[paper]](https://arxiv.org/pdf/2112.13112.pdf)
- Explainable Reinforcement Learning for Broad-XAI: A Conceptual Framework and Survey
  - R. Dazeley, P. Vamplew and F.Cruz. *arXiv 2021*.  [[paper]](https://arxiv.org/pdf/2108.09003)
- Explainable AI and Reinforcement Learning—A Systematic Review of Current Approaches and Trends
  - Lindsay Wells and Tomasz Bednarz.  *FRAI 2021*.  [[paper]](https://www.frontiersin.org/articles/10.3389/frai.2021.550030/full)
- Explainability in deep reinforcement learning
  - A. Heuillet, F. Couthouis and N. Díaz-Rodríguez.  *KBS 2021*. [[paper]](https://www.sciencedirect.com/science/article/am/pii/S0950705120308145)
- Explainable Deep Reinforcement Learning: State of the Art and Challenges
  - G. Vouros.  *CSUR 2022*.  [[paper]](https://scholar.archive.org/work/tpfqi5iggnhybfgz7u6qsiwm5i/access/wayback/https://dl.acm.org/doi/pdf/10.1145/3527448)
- Explainable Reinforcement Learning: A Survey and Comparative Review
  - S. Milani, N. Topin, M .Veloso and F. Fang. *CSUR 2023*. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3616864)

**[⬆ back to top](#table-of-contents)**

## Explainability in RL

### Agent Model-Explaining

#### Self-**Explainable**

- A Reduction of Imitation Learning and Structured Prediction to No-Regret Online Learning 
  - S. Ross, G. Gordon and D. Bagnell.  *AISTATS 2011*.  [[paper]](http://proceedings.mlr.press/v15/ross11a/ross11a.pdf)  [[code]](https://paperswithcode.com/paper/a-reduction-of-imitation-learning-and)
- Policy Search in a Space of Simple Closed-form Formulas: Towards Interpretability of Reinforcement Learning
  - F. Maes, R. Fonteneau, L. Wehenkel and D. Ernst.  *DS 2012*.  [[paper]](https://orbi.uliege.be/bitstream/2268/135635/1/Maes2012Ds.pdf)
- Particle swarm optimization for generating interpretable fuzzy reinforcement learning policies
  - D. Hein, A. Hentschel,T Runkler and S Udluft.  *EAAI 2017*.  [[paper]](https://arxiv.org/pdf/1610.05984)
- Toward Interpretable Deep Reinforcement Learning with Linear Model U-Trees
  - G. Liu, O. Schulte, W. Zhu and Q. Li.  *ECML PKDD 2018*.  [[paper]](https://arxiv.org/pdf/1807.05887)  [[code]](https://github.com/Guiliang/uTree_mimic_mountain_car)
- Programmatically Interpretable Reinforcement Learning
  - A. Verma, V. Murali, R. Singh, P. Kohli and S. Chaudhuri.  *ICML 2018*.  [[paper]](http://proceedings.mlr.press/v80/verma18a/verma18a.pdf)  [[code]](https://github.com/VAIBHAV-2303/PiRL)
- Interpretable policies for reinforcement learning by genetic programming
  - D. Hein, S. Udluft and T. Runkler.  *EAAI 2018*.  [[paper]](https://arxiv.org/pdf/1712.04170)
- Verifiable Reinforcement Learning via Policy Extraction
  - O. Bastani, Y. Pu and A. Solar-Lezama.  *NeurIPS 2018*.  [[paper]](https://proceedings.neurips.cc/paper/2018/file/e6d8545daa42d5ced125a4bf747b3688-Paper.pdf)  [[code]](https://github.com/quantumiracle/Cascading-Decision-Tree)
- Generating interpretable reinforcement learning policies using genetic programming
  - D. Hein, S. Udluft and T. Runkler.  *GECCO 2019*.  [[paper]](https://dl.acm.org/doi/10.1145/3319619.3326755)
- Imitation-projected programmatic reinforcement learning
  - A. Verma, H. Le, Y. Yue and S. Chaudhuri.  *NeurIPS 2019*.  [[paper]](https://proceedings.neurips.cc/paper/2019/file/5a44a53b7d26bb1e54c05222f186dcfb-Paper.pdf)  [[code]](https://bitbucket.org/averma8053/propel/src/master/)
- Towards Reinforcement Learning of Human Readable Policies
  - R. Akrour, D. Tateo and J. Peters.  *Workshop 2019*.  [[paper]](https://www.ias.informatik.tu-darmstadt.de/uploads/Team/RiadAkrour/decodeml2019.pdf)
- Neural Logic Reinforcement Learning
  - Z. Jiang and S. Luo.  *ICML 2019*.  [[paper]](http://proceedings.mlr.press/v97/jiang19a/jiang19a.pdf)  [[code]](https://github.com/ZhengyaoJiang/NLRL)
- Inductive logic programming via differentiable deep neural logic networks
  - A. Payani and F. Fekri.  *arXiv 2019*.  [[paper]](https://arxiv.org/pdf/1906.03523)  [[code]](https://github.com/apayani/ILP)
- Conservative q-improvement: Reinforcement learning for an interpretable decision-tree policy
  - A. Roth, N. Topin, P. Jamshidi and M. Veloso.  *arXiv 2019*.  [[paper]](https://arxiv.org/pdf/1907.01180)  [[code]](https://github.com/AMR-/Conservative-Q-Improvement)
- Generation of policy-level explanations for reinforcement learning
  - N. Topin and M. Veloso.  *AAAI 2019*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/4097/3975)
- Incorporating relational background knowledge into reinforcement learning via differentiable inductive logic programming
  - A. Payani and F. Fekri.  *arXiv 2020*.  [[paper]](https://arxiv.org/pdf/2003.10386)  [[code]](https://github.com/ling-k/RRL)
- Evolutionary learning of interpretable decision trees
  - LL. Custode and G. Iacca.  *arXiv 2020*.  [[paper]](https://arxiv.org/abs/2012.07723)  [[code]](https://gitlab.com/leocus/ge_q_dts)
- Optimization methods for interpretable differentiable decision trees applied to reinforcement learning
  - A. Silva, M. Gombolay, T. Killian, I. Jimenez and S. Son.  *AISTATS 2020*.  [[paper]](http://proceedings.mlr.press/v108/silva20a/silva20a.pdf)
- Neurosymbolic transformers for multi-agent communication
  - J. Inala, Y. Yang, J. Paulos, Y. Pu, O. Bastani, V. Kumar, M. Rinard and A. Solar-Lezama.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/9d740bd0f36aaa312c8d504e28c42163-Paper.pdf)  [[code]](https://github.com/jinala/multi-agent-neurosym-transformers)
- Learning to synthesize programs as interpretable and generalizable policies
  - D. Trivedi, J. Zhang, S. Sun and J. Lim.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/d37124c4c79f357cb02c655671a432fa-Paper.pdf)  [[code]](https://github.com/clvrai/leaps)
- Symbolic Regression via Deep Reinforcement Learning Enhanced Genetic Programming Seeding
  - T. Mundhenk, M. Landajuela, R. Glatt, C. Santiago, D. Faissol and B. Petersen.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/d073bb8d0c47f317dd39de9c9f004e9d-Paper.pdf)  [[code]](https://github.com/brendenpetersen/deep-symbolic-optimization)
- Discovering symbolic policies with deep reinforcement learning
  - M. Landajuela, B. Petersen, S. Kim, C. Santiago, R. Glatt, T. Mundhenk, J. Pettit and D. Faissol.  *ICML 2021*.  [[paper]](http://proceedings.mlr.press/v139/landajuela21a/landajuela21a.pdf)  [[code]](https://www.github.com/brendenpetersen/deep-symbolic-optimization)
- Iterative Bounding MDPs: Learning Interpretable Policies via Non-Interpretable Methods
  - N. Topin, S. Milani, F. Fang and M Veloso.  *AAAI 2021*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/17192/16999)
- MAVIPER: Learning Decision Tree Policies for Interpretable Multi-Agent Reinforcement Learning
  - S. Milani, Z. Zhang, N. Topin, Z. Shi, C. Kamhoua, E. Papalexakis and F. Fang.  *arXiv 2022*.  [[paper]](https://arxiv.org/pdf/2205.12449)  [[code]](https://stephmilani.github.io/maviper/)


#### Explanation Generating

- Explainable Reinforcement Learning through a Causal Lens
  - P. Madumal, T. Miller, L. Sonenberg and F. Vetere.  *AAAI 2020*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/5631/5487)  [[code]](https://github.com/NinaPi/Lunar_Causal_Network)
- Counterfactual state explanations for reinforcement learning agents via generative deep learning
  - M. Olson, R. Khanna, L. Neal, F. Li and W. Wong.  *AI 2021*.  [[paper]](https://www.sciencedirect.com/science/article/am/pii/S0004370221000060)  [[code]](https://github.com/mattolson93/counterfactual-state-explanations)
- Generating high-quality explanations for navigation in partially-revealed environments
  - G. Stein.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/926ec030f29f83ce5318754fdb631a33-Paper.pdf)  [[code]](https://github.com/rail-group/xai-nav-under-uncertainty-neurips2021)
- Explainable Reinforcement Learning via a Causal World Model
  - Z. Yu, J. Ruan and D. Xing.  *IJCAI 2023*.  [[paper]](https://arxiv.org/pdf/2305.02749)  [[code]](https://github.com/EaseOnway/Explainable-Causal-Reinforcement-Learning)
- Autonomous self-explanation of behavior for interactive reinforcement learning agents
  - Y. Fukuchi, M. Osawa, H. Yamakawa and M. Imai.  *HAI 2017*.  [[paper]](https://arxiv.org/pdf/1810.08811)
- Application of Instruction-Based Behavior Explanation to a Reinforcement Learning Agent with Changing Policy
  - Y. Fukuchi, M. Osawa, H. Yamakawa and M. Imai.  *ICONIP 2017*.  [[paper]](https://www.researchgate.net/profile/Yosuke-Fukuchi/publication/320580397_Application_of_Instruction-Based_Behavior_Explanation_to_a_Reinforcement_Learning_Agent_with_Changing_Policy/links/5a0d42630f7e9b9e33a9f490/Application-of-Instruction-Based-Behavior-Explanation-to-a-Reinforcement-Learning-Agent-with-Changing-Policy.pdf)
- Improving Robot Controller Transparency Through Autonomous Policy Explanation
  - B. Hayes and J. Shah.  *HRI 2017*.  [[paper]](https://dspace.mit.edu/bitstream/handle/1721.1/116013/hri17.pdf?sequence=1&isAllowed=y)
- Toward Policy Explanations for Multi-Agent Reinforcement Learning
  - K. Boggess, S. Kraus and L. Feng.  *IJCAI 2022*.  [[paper]](https://arxiv.org/pdf/2204.12568)  [[code]](https://github.com/kjboggess/IJCAI2022/blob/main/MissionGifExample.gif)
- Explainable Multi-Agent Reinforcement Learning for Temporal Queries
  - K. Boggess, S. Kraus and L. Feng.  *IJCAI 2023*.  [[paper]](https://arxiv.org/pdf/2305.10378)  [[code]](https://github.com/kjboggess/ijcai23)
- Verifying Deep-RL-Driven Systems
  - Y. Kazak , C. Barrett , G. Katz and M. Schapira  *NetAI 2019*.  [[paper]](https://dl.acm.org/doi/pdf/10.1145/3341216.3342218)
- Neurosymbolic reinforcement learning with formally verified exploration
  - G. Anderson, A. Verma, I. Dillig and S. Chaudhuri.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/448d5eda79895153938a8431919f4c9f-Paper.pdf)  [[code]](https://github.com/gavlegoat/safe-learning)
- An inductive synthesis framework for verifiable reinforcement learning
  - H. Zhu, Z. Xiong, S. Magill and S. Jagannathan.  *PLDI 2019*.  [[paper]](https://dl.acm.org/doi/pdf/10.1145/3314221.3314638)
- A CEGAR-Driven Training and Verification Framework for Safe Deep Reinforcement Learning
  - P. Jin, J. Tian, D. Zhi, X. Wen and M. Zhang.  *CAV 2022*.  [[paper]](https://link.springer.com/chapter/10.1007/978-3-031-13185-1_10)  [[code]](https://github.com/aptx4869tjx/RL_verification)


**[⬆ back to top](#table-of-contents)**

### Reward Explaining

#### Reward Decomposition

- Counterfactual multi-agent policy gradients
  - J. Foerster, G. Farquhar, T. Afouras, N. Nardelli and S. Whiteson.  *AAAI 2018*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/11794/11653)  [[code]](https://paperswithcode.com/paper/counterfactual-multi-agent-policy-gradients#code)
- Explainable reinforcement learning via reward decomposition
  - Z. Juozapaitis, A. Koul. A. Fern, M. Erwig and F. Doshi-Velez.  *IJCAI 2019*.  [[paper]](https://par.nsf.gov/servlets/purl/10159391)
- Shapley Q-value: A local reward approach to solve global reward games
  - J. Wang, Y. Zhang, T. Kim and Y. Gu.  *AAAI 2020*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/6220/6076)  [[code]](https://paperswithcode.com/paper/rethink-global-reward-game-and-credit)
- Shapley counterfactual credits for multi-agent reinforcement learning
  - J. Li, K. Kuang, B. Wang, F. Liu, L. Chen, F. Wu and J. Xiao.  *KDD 2021*.  [[paper]](https://arxiv.org/pdf/2106.00285)  

#### Reward Shaping

- Ella: Exploration through learned language abstraction
  - S. Mirchandani, S. Karamcheti and D. Sadigh.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/f6f154417c4665861583f9b9c4afafa2-Paper.pdf)  [[code]](https://github.com/Stanford-ILIAD/ELLA)
- Improving Human-Robot Interaction Through Explainable Reinforcement Learning
  - A. Tabrez and B. Hayes.  *HRI 2019*.  [[paper]](http://www.bradhayes.info/papers/hripioneers19.pdf)  
- SDRL: interpretable and data-efficient deep reinforcement learning leveraging symbolic planning
  - D. Lyu, F. Yang, B. Liu and S. Gustafson.  *AAAI 2019*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/4153/4031)
- Creativity of AI: Automatic Symbolic Option Discovery for Facilitating Deep Reinforcement Learning
  - M. Jin, Z. Ma, K. Jin, H. Zhuo, C. Chen and C. Yu.  *AAAI 2022*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/20663/20422)
- Tree-structured policy based progressive reinforcement learning for temporally language grounding in video
  - J. Wu, G. Li, S. Liu and L. Lin.  *AAAI 2020*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/6924/6778)  [[code]](https://github.com/WuJie1010/TSP-PRL)
- Self-supervised attention-aware reinforcement learning
  - H. Wu, K. Khetarpal and D. Precup.  *AAAI 2021*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/17235/17042)
- Dynamic Inverse Reinforcement Learning for Characterizing Animal Behavior
  - Z. Ashwood, A. Jha and JW. Pillow.  *NeurIPS 2022*.  [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/bf215fa7fe70a38c5e967e59c44a99d0-Paper-Conference.pdf)  [[code]](https://github.com/markusmeister/Rosenberg-2021-Repository)
**[⬆ back to top](#table-of-contents)**

### State Explaining

#### History Trajectory

- Robust bayesian inverse reinforcement learning with sparse behavior noise
  - J. Zheng, S. Liu and L. Ni.  *AAAI 2014*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/8979/8838)
- Visual sparse Bayesian reinforcement learning: a framework for interpreting what an agent has learned
  - I. Mishra, G. Dao and M. Lee.  *SSCI 2018*.  [[paper]](https://webpages.charlotte.edu/mlee173/pdfs/adprl18.pdf)
- Interestingness elements for explainable reinforcement learning: Understanding agents' capabilities and limitations
  - P. Sequeira and M. Gervasio. *AI 2020*.  [[paper]](https://arxiv.org/pdf/1912.09007)  [[code]](https://paperswithcode.com/paper/interestingness-elements-for-explainable)
- Explainable ai in deep reinforcement learning models for power system emergency control
  - K. Zhang, J. Zhang, P. Xu, T. Gao and D. Gao.  *TCSS 2021*.  [[paper]](https://ieeexplore.ieee.org/abstract/document/9506997)
- Edge: Explaining deep reinforcement learning policies
  - W. Guo, X. Wu, U. Khan and X. Xing.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/65c89f5a9501a04c073b354f03791b1f-Paper.pdf)  [[code]](https://github.com/henrygwb/edge)
- Collective explainable AI: Explaining cooperative strategies and agent contribution in multiagent reinforcement learning with shapley values
  - A. Heuillet, F. Couthouis and N. Díaz-Rodríguez.  *CIM 2022*  [[paper]](https://arxiv.org/pdf/2110.01307)  [[code]](https://github.com/fabien-couthouis/xai-in-rl)
- ProtoX: Explaining a Reinforcement Learning Agent via Prototyping
  - R. Ragodos, T. Wang, Q. Lin and X. Zhou.  *NeurIPS 2022*  [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/ae5bf4f35236240c9460e761c60fa53d-Paper-Conference.pdf)  [[code]](https://github.com/rrags/ProtoX)
- Towards interpretable deep reinforcement learning with human-friendly prototypes
  - EM. Kenny, M. Tucker and J. Shah.  *ICLR 2023*  [[paper]](https://openreview.net/pdf?id=hWwY_Jq0xsN)  [[code]](https://github.com/EoinKenny/Prototype-Wrapper-Network-ICLR23)


#### Current Observation

- Toward Interpretable Deep Reinforcement Learning with Linear Model U-Trees
  - G. Liu, O. Schulte, W. Zhu and Q. Li.  *ECML PKDD 2018*.  [[paper]](https://arxiv.org/pdf/1807.05887)  [[code]](https://github.com/Guiliang/uTree_mimic_mountain_car)
- Learn to interpret atari agents
  - Z. Yang, S. Bai, L. Zhang and P. Torr.  *arXiv 2018*. [[paper]](https://arxiv.org/pdf/1812.11276)  [[code]](https://github.com/yz93/Learn-to-Interpret-Atari-Agents)
- Visualizing and Understanding Atari Agents
  - S. Greydanus, A. Koul, J. Dodge and A. Fern.  *ICML 2018*  [[paper]](http://proceedings.mlr.press/v80/greydanus18a/greydanus18a.pdf)  [[code]](https://paperswithcode.com/paper/visualizing-and-understanding-atari-agents)
- Transparency and Explanation in Deep Reinforcement Learning Neural Networks
  - R. Iyer, Y. Li, H. Li, M. Lewis, R. Sundar, K. Sycara.  *AIES 2018*.  [[paper]](https://dl.acm.org/doi/pdf/10.1145/3278721.3278776)  [[code]](https://github.com/KDL-umass/saliency_maps)
- Rise: Randomized input sampling for explanation of black-box models
  - V. Petsiuk, A. Das and K. Saenko.  *arXiv 2018*.  [[paper]](https://arxiv.org/pdf/1806.07421)  [[code]](https://paperswithcode.com/paper/rise-randomized-input-sampling-for)
- Unsupervised video object segmentation for deep reinforcement learning
  - V. Goel, J. Weng and P. Poupart.  *NeurIPS 2018*.  [[paper]](https://proceedings.neurips.cc/paper/2018/file/96f2b50b5d3613adf9c27049b2a888c7-Paper.pdf)  [[code]](https://github.com/vik-goel/MOREL)
- DQNViz: A Visual Analytics Approach to Understand Deep Q-Networks
  - J. Wang, L. Gou, H. Shen and H. Yang.  *TVCG 2018*.  [[paper]](https://ieeexplore.ieee.org/abstract/document/8454905/)
- Alphastock: A buying-winners-and-selling-losers investment strategy using interpretable deep reinforcement attention networks
  - J. Wang, Y. Zhang, K. Tang, J. Wu and Z. Xiong.  *KDD 2019*.  [[paper]](https://arxiv.org/pdf/1908.02646)
- Social attention for autonomous decision-making in dense traffic
  - E. Leurent and J. Mercat.  *arXiv 2019*.  [[paper]](https://arxiv.org/pdf/1911.12250)  [[code]](https://eleurent.github.io/social-attention/)
- Towards better interpretability in deep q-networks
  - R. Annasamy and K. Sycara.  *AAAI 2019*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/4377/4255)  [[code]](https://github.com/maraghuram/I-DQN)
- Neuroevolution of self-interpretable agents
  - Y. Tang, D. Nguyen and D Ha.  *GECCO 2020*.  [[paper]](https://dl.acm.org/doi/pdf/10.1145/3377930.3389847)  [[code]](https://paperswithcode.com/paper/neuroevolution-of-self-interpretable-agents)
- The sensory neuron as a transformer: Permutation-invariant neural networks for reinforcement learning
  - Y. Tang and D. Ha.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/be3e9d3f7d70537357c67bb3f4086846-Paper.pdf)  [[code]](https://paperswithcode.com/paper/the-sensory-neuron-as-a-transformer)
- Deep reinforcement learning with stacked hierarchical attention for text-based games
  - Y. Xu, M. Fang, L. Chen, Y. Du, J. Zhou and C. Zhang.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/bf65417dcecc7f2b0006e1f5793b7143-Paper.pdf)  [[code]](https://github.com/YunqiuXu/SHA-KG)
- Xgail: Explainable generative adversarial imitation learning for explainable human decision analysis
  - M. Pan, W. Huang, Y. Li, X. Zhou and J. Luo.  *KDD 2020*.  [[paper]](https://dl.acm.org/doi/pdf/10.1145/3394486.3403186)  [[code]](https://github.com/paperpublicsource/xgail)
- Machine versus human attention in deep reinforcement learning tasks
  - S. Guo, R. Zhang, B. Liu, Y. Zhu, D. Ballard, M. Hayhoe and P. Stone.  *NeurIPS 2021*.  [[paper]](https://proceedings.neurips.cc/paper/2021/file/d58e2f077670f4de9cd7963c857f2534-Paper.pdf)
- Training characteristic functions with reinforcement learning: Xai-methods play connect four
  - S. Waldchen, F. Huber and S. Pokutta.  *ICML 2022*.  [[paper]](https://proceedings.mlr.press/v162/waldchen22a/waldchen22a.pdf)
- Look where you look! Saliency-guided Q-networks for generalization in visual Reinforcement Learning
  - D. Bertoin, A. Zouitine, M. Zouitine and E. Rachelson.  *NeurIPS 2022*.  [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/c5ee2a08fbe743b171b0b4b2bdfd6f86-Paper-Conference.pdf)
- Inherently explainable reinforcement learning in natural language
  - X. Peng, M. Riedl and P. Ammanabrolu.  *NeurIPS 2022*.  [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/672e44a114a41d5f34b97459877c083d-Paper-Conference.pdf)  [[code]](https://github.com/xiangyu-peng/HEX-RL)
- Explaining reinforcement learning with shapley values
  - D. Beechey, TMS. Smith and Ö. Şimşek  *ICML 2023*.  [[paper]](https://proceedings.mlr.press/v202/beechey23a/beechey23a.pdf) [[code]](https://github.com/bath-reinforcement-learning-lab/SVERL_icml_2023)
#### Future Prediction

- Contrastive explanations for reinforcement learning in terms of expected consequences
  - J. Waa, J. Diggelen, K. Bosch and M. Neerincx.  *arXiv 2018*.  [[paper]](https://arxiv.org/pdf/1807.08706)
- Semantic Predictive Control for Explainable and Efficient Policy Learning
  - X. Pan; X. Chen; Q. Cai; J. Canny and F. Yu.  *ICRA 2019*.  [[paper]](https://ieeexplore.ieee.org/abstract/document/8794437/)
- Safe Reinforcement Learning With Model Uncertainty Estimates
  - B. Lütjens, M. Everett and J. How.  *ICRA 2019*.  [[paper]](https://arxiv.org/pdf/1810.08700)
- What did you think would happen? explaining agent behaviour through intended outcomes
  - H. Yau, C. Russell and S. Hadfield.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/d5ab8dc7ef67ca92e41d730982c5c602-Paper.pdf)  [[code]](https://paperswithcode.com/paper/what-did-you-think-would-happen-explaining#code)
- Weakly-supervised reinforcement learning for controllable behavior
  - L. Lee, B. Eysenbach, R. Salakhutdinov, S. Gu and C. Finn.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/1bd69c7df3112fb9a584fbd9edfc6c90-Paper.pdf)


**[⬆ back to top](#table-of-contents)**

### Task Explaining

#### Whole Top-down Structure

- Hierarchical and Interpretable Skill Acquisition in Multi-task Reinforcement Learning
  - T. Shu, C. Xiong and R. Socher.  *ICLR 2018*.  [[paper]](https://arxiv.org/pdf/1712.07294)
- A Boolean task algebra for reinforcement learning
  - G. Nangue Tasse, S. James and B. Rosman.  *NeurIPS 2020*.  [[paper]](https://proceedings.neurips.cc/paper/2020/file/6ba3af5d7b2790e73f0de32e5c8c1798-Paper.pdf)  [[code]](https://github.com/geraudnt/boolean_composition)

#### Simple Task Division

- Language as an abstraction for hierarchical deep reinforcement learning
  - Y. Jiang, S. Gu, K. Murphy and C.Finn.  *NeurIPS 2019*.  [[paper]](https://proceedings.neurips.cc/paper/2019/file/0af787945872196b42c9f73ead2565c8-Paper.pdf)  [[code]](https://paperswithcode.com/paper/language-as-an-abstraction-for-hierarchical#code)
- SDRL: interpretable and data-efficient deep reinforcement learning leveraging symbolic planning
  - D. Lyu, F. Yang, B. Liu and S. Gustafson.  *AAAI 2019*.  [[paper]](https://ojs.aaai.org/index.php/AAAI/article/download/4153/4031)
- Dot-to-dot: Explainable hierarchical reinforcement learning for robotic manipulation
  - B. Beyret, A. Shafti, A. Faisal.  *IROS 2019*.  [[paper]](https://arxiv.org/pdf/1904.06703)
- Model primitives for hierarchical lifelong reinforcement learning
  - B. Wu, J. Gupta and M. Kochenderfer.  *AAMAS 2020*.  [[paper]](https://arxiv.org/pdf/1903.01567)  [[code]](https://github.com/sisl/MPHRL)
- Multi-task reinforcement learning with context-based representations
  - S. Sodhani, A. Zhang and J. Pineau.  *NeurIPS 2021*.  [[paper]](http://proceedings.mlr.press/v139/sodhani21a/sodhani21a.pdf)  [[code]](https://paperswithcode.com/paper/multi-task-reinforcement-learning-with#code)


**[⬆ back to top](#table-of-contents)**

## 🤖️ Human knowledge for RL paradigm

### Fuzzy Controller Representing Human Knowledge
- KoGuN: Accelerating Deep Reinforcement Learning via Integrating Human Suboptimal Knowledge
  - P. Zhang, J. Hao, W. Wang, H. Tang, Y. Ma, Y. Duan and Y. Zheng.  *arXiv 2020*.  [[paper]](https://arxiv.org/pdf/2002.07418)
- Fuzzy Action-Masked Reinforcement Learning Behavior Planning for Highly Automated Drivin
  - T. Rudolf, M. Gao, T. Schürmann, S. Schwab and S. Hohmann. *ICCAR*.  [[paper]](https://ieeexplore.ieee.org/abstract/document/9782671) 
- Efficient hierarchical policy network with fuzzy rules
  - W. Shi, Y. Feng, H. Huang, Z. Liu, J. Huang and G. Cheng. *IJMLC*. [[paper]](https://link.springer.com/article/10.1007/s13042-021-01417-2)

### Dense Reward on Human Command
- Using Natural Language for Reward Shaping in Reinforcement Learning
  - P. Goyal, S. Niekum and R. Mooney.  *arXiv 2019*.  [[paper]](https://arxiv.org/pdf/1903.02020)  [[code]](https://github.com/prasoongoyal/rl-learn)

### Learn Mattered Features from Human Interactions
- Textual Explanations for Self-Driving Vehicles
  - J. Kim, A. Rohrbach, T. Darrell, J. Canny and Z. Akata.  *ECCV 2018*.  [[paper]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Jinkyu_Kim_Textual_Explanations_for_ECCV_2018_paper.pdf)  [[code]](https://github.com/JinkyuKimUCB/explainable-deep-driving)
- Local explanations for reinforcement learning
  - R. Luss, A. Dhurandhar, M. Liu. *AAAI 2023*. [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/26081)
- Curricular Subgoals for Inverse Reinforcement Learning
  - S. Liu, Y. Qing, S. Xu, H. Wu, J. Zhang, J. Cong, T. Chen, Y. Liu and M. Song. *arXiv*.  [[paper]](https://arxiv.org/pdf/2306.08232.pdf)  [[code]](https://github.com/Plankson/CSIRL)

### Subtask Scheduling with Human Annotation
- Ask Your Humans: Using Human Instructions to Improve Generalization in Reinforcement Learning
  - V. Chen, A. Gupta, K. Marino.  *arXiv 2020*.  [[paper]](https://arxiv.org/pdf/2011.00517)  [[code]](https://github.com/valeriechen/ask-your-humans)
- LISA: Learning interpretable skill abstractions from language
  - D. Garg, S. Vaidyanath, K. Kim, J. Song and S. Ermon. *NeurIPS 2022*. [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/883105b282fe15275991b411e6b200c5-Paper-Conference.pdf)
- Towards Effective and Interpretable Human-Agent Collaboration in MOBA Games: A Communication Perspective
  - Y. Gao, F. Liu, L. Wang, Z. Lian, W. Wang, S. Li, X. Wang, X. Zeng, R. Wang, J. Wang, Q. Fu, W. Yang, L. Huang and W. Liu. *ICLR 2023*. [[paper]](https://arxiv.org/pdf/2304.11632.pdf) [[code]](https://sites.google.com/view/mcc-demo)
- Perceiving the world: Question-guided reinforcement learning for text-based games
  - Y. Xu, M. Fang, L. Chen, Y. Du, JT. Zhou and C. Zhang.  *ACL 2022*.  [[paper]](https://arxiv.org/pdf/2204.09597.pdf)  [[code]](https://github.com/YunqiuXu/QWA)


**[⬆ back to top](#table-of-contents)**

## 🏠 Explainable AI Library

As for completeness, we also list the library of explainable AI methods to tackle the balck box problem of AI methods. They can emhance the AI model with transparency and explainability.
| Explainable AI library                                       |                         GitHub Stars                         |
| ------------------------------------------------------------ | :----------------------------------------------------------: |
| [Aequitas](https://github.com/dssg/aequitas)                 | ![Star](https://img.shields.io/github/stars/dssg/aequitas) |
| [Alibi Explain](https://github.com/SeldonIO/alibi)           | ![Star](https://img.shields.io/github/stars/SeldonIO/alibi) |
| [Captum](https://github.com/pytorch/captum)                  | ![Star](https://img.shields.io/github/stars/pytorch/captum) |
| [DeepVis Toolbox](https://github.com/yosinski/deep-visualization-toolbox) | ![Star](https://img.shields.io/github/stars/yosinski/deep-visualization-toolbox) |
| [ELI5](https://github.com/TeamHG-Memex/eli5)                 | ![Star](https://img.shields.io/github/stars/TeamHG-Memex/eli5) |
| [InterpretML](https://github.com/interpretml/interpret/)     | ![Star](https://img.shields.io/github/stars/interpretml/interpret) |
| [IBM AI Explainability 360](https://github.com/Trusted-AI/AIX360) | ![Star](https://img.shields.io/github/stars/Trusted-AI/AIX360) |
| [iModels](https://github.com/csinva/imodels)                 | ![Star](https://img.shields.io/github/stars/csinva/imodels.svg) |
| [LIME](https://github.com/marcotcr/lime)                     | ![Star](https://img.shields.io/github/stars/marcotcr/lime) |
| [OmniXAI](https://github.com/salesforce/OmniXAI)             | ![Star](https://img.shields.io/github/stars/salesforce/OmniXAI)|
| [SHAP](https://github.com/slundberg/shap)                    | ![Star](https://img.shields.io/github/stars/slundberg/shap) |
| [Skater](https://github.com/oracle/Skater)                   | ![Star](https://img.shields.io/github/stars/oracle/Skater)|

<!-- ## Contributors

<a href="https://github.com/Plankson/awesome-explainable-reinforcement-learning/contributors">
  <img src="https://contrib.rocks/image?repo=plankson/awesome-explainable-reinforcement-learning" />
</a>
 -->
## Show your support

Please ⭐️ this repository if this project helped you!


## Starchart

[![Star History Chart](https://api.star-history.com/svg?repos=Plankson/awesome-explainable-reinforcement-learning&Date)](https://star-history.com/#Plankson/awesome-explainable-reinforcement-learning&Date)

**[⬆ back to top](#table-of-contents)**
