This repository lists papers on causality for natural language processing (NLP). Welcome to be a collaborator, -- you can make an issue/pull request, and I can add you :).

### Contents (Actively Updating)
- [1. Causality Basics](#1-causality-basics)
  - [1.1 Talks/Tutorial/etc](#11-talkstuturaletc)
  - [1.2 Overview Papers](#12-overview-papers)
- [2. Causality Applied to General NLP](#2-causality-applied-to-general-nlp)
- [3. Addressing "Confounders" in NLP](#3-addressing-confounders-in-nlp)
  - [3.1 Causality tools that can be applied to deconfound](#31-causality-tools-that-can-be-applied-to-deconfound)
- [4. More Resources](#4-more-resources)
  - [4.1 Causality Papers from Schoelkopf's Lab, MPI](#41-causality-papers-from-schoelkopfs-lab-mpi)
  - [4.2 Causality Papers from Bengio's Lab, MILA](#42-causality-papers-from-bengios-lab-mila)
  - [4.3 Books (for Systematic Learning)](#43-books-for-systematic-learning)
- [Contributions](#contributions)

## 1. Causality Basics 
### 1.1 Talks/Tutorial/etc
1. (Vivid, beginner-friendly) **Yoshua Bengio's Primer on the Future of Causality&NLP.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]
### 1.2 Overview Papers
1. (2021 Overview, Schoelkopf+) **Towards Causal Representation Learning.** [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
1. (2019 Overview, Schoelkopf) **Causality for Machine Learning.** [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

## 2. Causality Applied to General NLP
1. (NeurIPS 2020 Spotlight) **Causal Mediation Analysis for Interpreting Neural NLP:
The Case of Gender Bias.** _Jesse Vig, Sebastian Gehrmann, Yonatan Belinkov, Sharon Qian, Daniel Nevo, Simas Sakenis, Jason Huang, Yaron Singer, Stuart Shieber_. [[pdf](https://arxiv.org/pdf/2004.12265.pdf)]
<br>[Summary] Cause: input text, mediator: some neurons, effect: output prediction

1. (ACL 2020) **Text and Causal Inference: A Review of Using Text to Remove Confounding from Causal Estimates.** _Katherine A. Keith, David Jensen, and Brendan O'Connor_. [[pdf](https://www.aclweb.org/anthology/2020.acl-main.474.pdf)]

1. (UAI 2020) **Adapting Text Embeddings for Causal Inference.** _Victor Veitch, Dhanya Sridhar, David M. Blei_. [[pdf](https://arxiv.org/pdf/1905.12741.pdf)]

1. (arXiv 2020) **Causal Effects of Linguistic Properties.** _Reid Pryzant, Dallas Card, Dan Jurafsky, Victor Veitch, Dhanya Sridhar_. [[pdf](https://arxiv.org/pdf/2010.12919.pdf)]
<br>[Summary] Cause: binary writer intent, confounder: other linguistic habits of the writer, mediator: text by the writer, effect: reader's response time

## 3. Addressing "Confounders" in NLP
1. (EMNLP 2019) **Topics to Avoid: Demoting Latent Confounds in Text Classification.** _Sachin Kumar, Shuly Wintner, Noah A. Smith, Yulia Tsvetkov_. [[pdf](https://arxiv.org/pdf/1909.00453.pdf)]
<br>[Summary] Cause: native language, confounder: topic, effect: text

1. (NAACL 2018, Stanford) **Deconfounded lexicon induction for interpretable social science.** _Reid Pryzant, Kelly Shen, Dan Jurafsky, Stefan Wagner_. [[pdf](https://www.aclweb.org/anthology/N18-1146.pdf)]
<br>[Summary] Cause: some keywords, confounder: , effect: output prediction

1. Interpretable Neural Architectures for Attributing an Ad’s Performance to its Writing Style
### 3.1 Causality tools that can be applied to deconfound
1. (NIPS 2017, MPI, discover causal graphs behind data) **Avoiding Discrimination through Causal Reasoning.** _Niki Kilbertus, Mateo Rojas-Carulla, Giambattista Parascandolo, Moritz Hardt, Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1706.02744.pdf)]

## 4. More Resources
### 4.1 Causality Papers from Schoelkopf's Lab, MPI
#### Overview
1. (2021 Overview) **Towards Causal Representation Learning.** [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
1. (2019 Overview) **Causality for Machine Learning.** [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

#### Causal discovery
1. **Causal Discovery from Heterogeneous/Nonstationary Data with Independent Changes.** _Biwei Huang, Kun Zhang, Jiji Zhang, Joseph Ramsey, Ruben Sanchez-Romero, Clark Glymour, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1903.01672.pdf)]


### 4.2 Causality Papers from Bengio's Lab, MILA
1. (Summary) **Yoshua Bengio's Summary Talk.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]

#### Motivational Position Papers
1. (Position Paper, arXiv 2020) **Inductive Biases for Deep Learning of Higher-Level Cognition.** _Anirudh Goyal, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/2011.15091.pdf)]
<br>[Summary] We need inductive bias for real understanding and generalization => such as decomposing world knowledge into right causal pieces

1. (Motivational, position paper, arXiv 2017) **The Consciousness Prior.** _Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1709.08568.pdf)]

#### Applying Causality Knowledge for RL Interaction Design
1. (arXiv 2020) **Visual Concept Reasoning Networks.** _Taesup Kim, Sungwoong Kim, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/2008.11783.pdf)]
<br> [Summary] Modularized visual concept reasoning by split-transform-attend-interact-modulate-merge modules

1. (RLDM 2017) **Independently Controllable Features.**
_Emmanuel Bengio, Valentin Thomas, Joelle Pineau, Doina Precup, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1703.07718.pdf)]

1. (arXiv 2017) **Independently Controllable Factors.** _Valentin Thomas, Jules Pondard, Emmanuel Bengio, Marc Sarfati, Philippe Beaudoin, Marie-Jean Meurs, Joelle Pineau, Doina Precup, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1708.01289.pdf)]
<br> [Summary] The representations of (1) abstract action, and (2) abstract variables, should be learned together, because the action is about controlling variables. A way to disentangle abstractions from images & videos when we have an agent which can interact with the environment. The right abstractions have the right factors. I.e., there exists a policy and a learnable feature for each such aspect of the environment.

#### Applying causality to model design
1. **Recurrent Independent Mechanisms.** _Anirudh Goyal, Alex Lamb, Jordan Hoffmann, Shagun Sodhani, Sergey Levine, Yoshua Bengio, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1909.10893.pdf)]
<br>[Summary] Divides the overall model into k small subsystems (or modules), Each small module is recurrent

1. **Object Files and Schemata: Factorizing Declarative and Procedural Knowledge in Dynamical Systems.** _Anirudh Goyal, Alex Lamb, Phanideep Gampa, Philippe Beaudoin, Sergey Levine, Charles Blundell, Yoshua Bengio, Michael Mozer_. [[pdf](https://arxiv.org/pdf/2006.16225.pdf)]
<br>[Summary] Modularity when designing the model

#### Causal induction from interventional data
[Background] Changes in distribution is caused by intervention on few causes/mechanisms (in extension of Independent Mechanisms by [[Schoelkopf+ 2012](https://icml.cc/2012/papers/625.pdf)])

1. (arXiv 2019) **Learning Neural Causal Models from unknown Interventions.** _Nan Rosemary Ke, Olexa Bilaniuk, Anirudh Goyal, Stefan Bauer, Hugo Larochelle, Bernhard Schölkopf, Michael C. Mozer, Chris Pal, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1910.01075.pdf)]
<br>[Summary] Aim: make use of the combination of observational and interventional data, Method: continuous optimization and neural networks, Extended setting: when the identity of the intervened upon variable is unknown

1. (NeurIPS 2020 Spotlight) **Differentiable Causal Discovery from Interventional Data.** _Philippe Brouillard, Sébastien Lachapelle, Alexandre Lacoste, Simon Lacoste-Julien, Alexandre Drouin_. [[pdf](https://arxiv.org/pdf/2007.01754.pdf)] [[review](https://papers.nips.cc/paper/2020/file/f8b7aa3a0d349d9562b424160ad18612-Review.html)]
<br>[Summary] Closely related to [Ke+ 2019](https://arxiv.org/pdf/1910.01075.pdf), Method: continuous-constrained framework + normalizing flows

1. (ICLR 2019) **Learning Dynamics Model in Reinforcement Learning by Incorporating the Long Term Future.** _Nan Rosemary Ke, Amanpreet Singh, Ahmed Touati, Anirudh Goyal, Yoshua Bengio, Devi Parikh, Dhruv Batra_.
[[pdf](https://arxiv.org/pdf/1903.01599.pdf)]

1. (ICLR 2020) **A Meta-Transfer Objective for Learning to Disentangle Causal Mechanisms.** _Yoshua Bengio, Tristan Deleu, Nasim Rahaman, Rosemary Ke, Sébastien Lachapelle, Olexa Bilaniuk, Anirudh Goyal, Christopher Pal_. [[pdf](https://arxiv.org/pdf/1901.10912.pdf)]

#### Grounded AI
1. (ICLR 2021) **CausalWorld: A Robotic Manipulation Benchmark for Causal Structure and Transfer Learning.** _Ossama Ahmed, Frederik Träuble, Anirudh Goyal, Alexander Neitz, Yoshua Bengio, Bernhard Schölkopf, Manuel Wüthrich, Stefan Bauer_. [[pdf](https://arxiv.org/pdf/2010.04296.pdf)]
<br>[Summary] An RL dataset to model do-interventions and discover causality

1. (ICLR 2019) **BabyAI: A Platform to Study the Sample Efficiency of Grounded Language Learning.** _Maxime Chevalier-Boisvert, Dzmitry Bahdanau, Salem Lahlou, Lucas Willems, Chitwan Saharia, Thien Huu Nguyen, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1810.08272.pdf)]
<br>[Summary] (not yet causal) synthetic language acquisition, A simulation platform, to do language instructions with a simulated human in the loop, Allows curriculum learning for 19 levels






### 4.3 Books (for Systematic Learning)
1. (For ML Audience) **Elements of Causal Inference.** _Jonas Peters, Dominik Janzing and Bernhard Schölkopf_. [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]

1. (Quick Primer by Judea Pearl) **Causal Inference in Statistics: A Primer.** _Judea Pearl_. [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
1. (Focus on SCM) **Causality: Models, Reasoning, and Inference.** _Judea Pearl_. [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
- More reading recommendations: See Brady Neal's [blog](https://www.bradyneal.com/which-causal-inference-book).

## Contributions
All types of contributions to this paper list is welcome. Feel free to open a Pull Request.

Contact: [Zhijing Jin](zhijing-jin.com), PhD of Bernhard Schoelkopf at Max Planck Institute for Intelligent Systems, working on NLP & Causality.

