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
1. (Vivid, beginner-friendly) **Yoshua Bengio's Overview of Causality&NLP.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]
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

### 4.2 Causality Papers from Bengio's Lab, MILA


### 4.3 Books (for Systematic Learning)
1. (For ML Audience) **Elements of Causal Inference.** _Jonas Peters, Dominik Janzing and Bernhard Schölkopf_. [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]

1. (Quick Primer by Judea Pearl) **Causal Inference in Statistics: A Primer.** _Judea Pearl_. [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
1. (Focus on SCM) **Causality: Models, Reasoning, and Inference.** _Judea Pearl_. [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
- More reading recommendations: See Brady Neal's [blog](https://www.bradyneal.com/which-causal-inference-book).

## Contributions
All types of contributions to this paper list is welcome. Feel free to open a Pull Request.

Contact:.** [Zhijing Jin](zhijing-jin.com), PhD of Bernhard Schoelkopf at Max Planck Institute for Intelligent Systems, working on NLP & Causality.

