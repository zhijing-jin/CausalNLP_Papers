This repository lists papers on causality for natural language processing (NLP). Welcome to be a collaborator, -- you can make an issue/pull request, and I can add you :).

### Contents
- [1. Causality Basics](#1-causality-basics)
- [2. Causality Applied to General NLP](#2-causality-applied-to-general-nlp)
- [3. Addressing "Confounders" in NLP](#3-addressing-confounders-in-nlp)
- [4. More Resources](#4-more-resources)
- [Contributions](#contributions)

## 1. Causality Basics 
### 1.1 Talks/Tutorial/Overview
1. (Vivid, beginner-friendly) Yoshua Bengio's Overview of Causality&NLP [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]
### 1.2 Overview Papers
1. (2021 Overview, Schoelkopf+) Towards Causal Representation Learning [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
1. (2019 Overview, Schoelkopf) Causality for Machine Learning [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

## 2. Causality Applied to General NLP
1. (NeurIPS 2020 Oral) Causal Mediation Analysis for Interpreting Neural NLP:
The Case of Gender Bias [[pdf](https://arxiv.org/pdf/2004.12265.pdf)]
[Summary] Cause: input text, mediator: some neurons, effect: output prediction

1. (ACL 2020) Text and Causal Inference: A Review of Using Text to Remove Confounding from Causal Estimates [[pdf](https://www.aclweb.org/anthology/2020.acl-main.474.pdf)]

1. (UAI 2020) Adapting Text Embeddings for Causal Inference [[pdf](https://arxiv.org/pdf/1905.12741.pdf)]

1. (arXiv 2020) Causal Effects of Linguistic Properties [[pdf](https://arxiv.org/pdf/2010.12919.pdf)]
[Summary] Cause: binary writer intent, confounder: other linguistic habits of the writer, mediator: text by the writer, effect: reader's response time

## 3. Addressing "Confounders" in NLP
1. (EMNLP 2019) Topics to Avoid: Demoting Latent Confounds in Text Classification [[pdf](https://arxiv.org/pdf/1909.00453.pdf)]
[Summary] Cause: native language, confounder: topic, effect: text

1. (NAACL 2018, Stanford) Deconfounded lexicon induction for interpretable social science [[pdf](https://www.aclweb.org/anthology/N18-1146.pdf)]
[Summary] Cause: some keywords, confounder: , effect: output prediction

1. Interpretable Neural Architectures for Attributing an Ad’s Performance to its Writing Style
### 3.1 Causality tools that can be applied to deconfound
1. (NIPS 2017, MPI, discover causal graphs behind data) Avoiding Discrimination through Causal Reasoning [[pdf](https://arxiv.org/pdf/1706.02744.pdf)]

## 4. More Resources

### Books (for Systematic Learning)
1. (For ML Audience) Elements of Causal Inference: [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]

1. (Quick Primer by Judea Pearl) Causal Inference in Statistics: A Primer [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
1. (Focus on SCM) Causality: Models, Reasoning, and Inference [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
- More reading recommendations: See this [blog](https://www.bradyneal.com/which-causal-inference-book).

## Contributions
All types of contributions to this paper list is welcome. Feel free to open a Pull Request.

Contact: [Zhijing Jin](zhijing-jin.com), PhD of Bernhard Schoelkopf at Max Planck Institute for Intelligent Systems, working on NLP & Causality.

