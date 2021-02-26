This repository lists papers on causality for natural language processing (NLP).


## Causality Basics 
### Talks/Tutorial/Overview
- (Vivid, beginner-friendly) Yoshua Bengio's Overview of Causality&NLP [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]
### Overview Papers
- (2021 Overview, Schoelkopf+) Towards Causal Representation Learning [[PDF](https://arxiv.org/pdf/2102.11107.pdf)]
- (2019 Overview, Schoelkopf) Causality for Machine Learning [[PDF](https://arxiv.org/pdf/1911.10500.pdf)]

## Causality Applied to NLP
- (NeurIPS 2020 Oral) Causal Mediation Analysis for Interpreting Neural NLP:
The Case of Gender Bias [[PDF](https://arxiv.org/pdf/2004.12265.pdf)]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Cause: input text, mediator: some neurons, effect: output prediction

- (ACL 2020) Text and Causal Inference: A Review of Using Text to Remove Confounding from Causal Estimates [[PDF](https://www.aclweb.org/anthology/2020.acl-main.474.pdf)]

- (UAI 2020) Adapting Text Embeddings for Causal Inference [[PDF](https://arxiv.org/pdf/1905.12741.pdf)]

- (arXiv 2020) Causal Effects of Linguistic Properties [[PDF](https://arxiv.org/pdf/2010.12919.pdf)]


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Cause: binary writer intent, confounder: other linguistic habits of the writer, mediator: text by the writer, effect: reader's response time

## Addressing "Confounders" in NLP
- (EMNLP 2019) Topics to Avoid: Demoting Latent Confounds in Text Classification [[PDF](https://arxiv.org/pdf/1909.00453.pdf)]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Cause: native language, confounder: topic, effect: text

- (NAACL 2018, Stanford) Deconfounded lexicon induction for interpretable social science [[PDF](https://www.aclweb.org/anthology/N18-1146.pdf)]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Cause: some keywords, confounder: , effect: output prediction

- Interpretable Neural Architectures for Attributing an Ad’s Performance to its Writing Style
### Non-NLP Causality tools that can be applied to deconfound
- (NIPS 2017, MPI, discover causal graphs behind data) Avoiding Discrimination through Causal Reasoning [[PDF](https://arxiv.org/pdf/1706.02744.pdf)]

## More Resources

### Books (for Systematic Learning)
- (For ML Audience) Elements of Causal Inference: [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]

- (Quick Primer by Judea Pearl) Causal Inference in Statistics: A Primer [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
- (Focus on SCM) Causality: Models, Reasoning, and Inference [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
- More reading recommendations: See this [blog](https://www.bradyneal.com/which-causal-inference-book).

## Contributions
All types of contributions to this paper list is welcome. Feel free to open a Pull Request.

Contact: [Zhijing Jin](zhijing-jin.com), PhD of Bernhard Schoelkopf at Max Planck Institute for Intelligent Systems, working on NLP & Causality.

