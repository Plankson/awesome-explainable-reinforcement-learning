# Awesome Explainable Reinforcement-Learning

A list of awesome paper and code resources on explainable reinforcement learning. Inspired by [Awesome-Visual-Transformer](https://github.com/dk-liang/Awesome-Visual-Transformer), [awesome-transfer-learning](https://github.com/artix41/awesome-transfer-learning), [awesome-self-supervised-learning](https://github.com/jason718/awesome-self-supervised-learning), [awesome-graph-self-supervised-learning](https://github.com/LirongWu/awesome-graph-self-supervised-learning) and [awesome-deep-vision](https://github.com/kjw0612/awesome-deep-vision).

## Table of Contents

- [Overview](#Overview)
- [Papers](#Papers)
  - [Survey](#Survey)
- 

## <h2 id="Overview"> Overview</h2>

We review current explainable reinforcement learning framework and explainability of human knowledge-based reinforcement learning framework. We creatively propose a new taxonomy for existing explainable reinforcement learning based on reinforcement learning paradigm. Specifically, we divide existing explainable reinforcement learning methods into four categories: model-explaining, reward-explaining, state-explaining, task-explaining as shown below:

<img src="Fig\Taxonomy.png" alt="1" style="zoom: 80%;" />

​	In the Figure above, $e_\pi$ and $e_g$ denotes for two aspects of explanations: inner logic inference of agent and goal influence in action-taking. $a_t,r_t,s_t$ refer to the action, reward and states at time $t$;  The red parts in these diagrams are the explainable parts.

- Model Explaining: trains the agent to be explainable by having understandable logic operation in its inner structure
- Reward Explaining: reconstructs reward function towards an explainable one $r'_t$  and makes it possible to see how the goal influences the agent
- State Explaining: adds a submodule for introspection to quantify the influences of different state features towards the decision-making as $w(s_t)$.
- Task Explaining: gets an architectural level explainability in complex environments by multilevel agents, the high-level agent schedule low-level agents by the subgoal signal $g_t$ which could be utilized for explanations.



## <h2 id="Papers">Papers</h2>

###  <h2 id="Survey">Survey</h2>

- Explainable Reinforcement Learning: A Survey
  - E. Puiutta and E. Veith.  *CD-MAKE 2020*. [[paper]](https://arxiv.org/pdf/2005.06247.pdf)
- A Survey on Interpretable Reinforcement Learning
  - C. Glanois, P. Weng, M. Zimmer, D. Li, T. Yang,  J. Hao and W. Liu.  *Arxiv 2021*. [[paper]](https://arxiv.org/pdf/2112.13112.pdf)
- Explainable Reinforcement Learning for Broad-XAI: A Conceptual Framework and Survey
  - R. Dazeley, P. Vamplew and F.Cruz. *Arxiv 2021*. [[paper]](https://arxiv.org/pdf/2108.09003)
- Explainable AI and Reinforcement Learning—A Systematic Review of Current Approaches and Trends
  - Lindsay Wells and Tomasz Bednarz.  *FRAI 2021*. [[paper]](https://www.frontiersin.org/articles/10.3389/frai.2021.550030/full)
- Explainability in deep reinforcement learning
  - A. Heuillet, F. Couthouis and N. Díaz-Rodríguez.  *KBS 2021*. [[paper]](https://www.sciencedirect.com/science/article/am/pii/S0950705120308145)
- Explainable Deep Reinforcement Learning: State of the Art and Challenges
  - G. Vouros.  *ACM 2022*.  [[paper]](https://scholar.archive.org/work/tpfqi5iggnhybfgz7u6qsiwm5i/access/wayback/https://dl.acm.org/doi/pdf/10.1145/3527448)

