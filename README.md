# Causality for NLP Reading List

This repository lists papers on causality for natural language processing (NLP). 

**Contributor:** [Zhijing Jin](http://zhijing-jin.com).
Welcome to be a collaborator, -- you can make an issue/pull request, and I can add you :).

### Contents (Actively Updating)

- [1. Causality Basics](#1-causality-basics)
  - [1.1 Talks/Tutorial/etc](#11-talks-tutorial-etc)
  - [1.2 Overview Papers](#12-overview-papers)
  - [1.3 Toolboxes](#13-toolboxes)
- [2. Causality Applied to General NLP](#2-causality-applied-to-general-nlp)
  - [2.1 Overview](#21-overview)
  - [2.2 Causal Reasoning](#22-causal-reasoning)
  - [2.3 Interpretability by Causal Methods](#23-interpretability-by-causal-methods)
  - [2.4 Text Features in Causal Graphs (for Social Science, Psychology, etc.)](#24-text-features-in-causal-graphs-for-social-science-psychology-etc)
  - [2.5 Causality to Bring Insights to NLP Modeling (for Robustness, Domain Adaptation, etc)](#25-causality-to-bring-insights-to-nlp-modeling-for-robustness-domain-adaptation-etc)
  - [2.6 Causal Relation Extraction](#26-causal-relation-extraction)
- [3. Causality for Various Applications](#3-causality-for-various-applications)
  - [3.1 Persuasion](#31-persuation)
  - [3.2 Psychology and Behavior](#32-psychology-and-behavior)
  - [3.3 Economics](#33-economics)
  - [3.4 Healthcare](#34-healthcare)
  - [3.4 Judicial Decision](#35-judicial-decision)
  - [3.5 Marketing strategies and sales prediction](#36-marketing-strategies-and-sales-prediction)
- [4. More Resources](#4-more-resources)
  - [4.1 Causality Papers from Schoelkopf's Lab, MPI](#41-causality-papers-from-schoelkopfs-lab-mpi)
    - [4.1.0 Overview](#410-overview)
    - [4.1.1 Learning Causal "Units" and Mechanisms (i.e., Causal Representation Learning)](#411-learning-causal-units-and-mechanisms-ie-causal-representation-learning)
    - [4.1.2 Robustness and Invariance (incl. Semi-Supervised Learning, Covariate Shift, Transfer Learning)](#411-learning-causal-units-and-mechanisms-ie-causal-representation-learning)
    - [4.1.3 Causal Discovery](#411-learning-causal-units-and-mechanisms-ie-causal-representation-learning)
    - [4.1.4 Causal Effect Estimation](#414-causal-effect-estimation)
    - [4.1.5 Foundational work (theory, ICA, etc.)](#415-foundational-work-theory-ica-etc)
  - [4.2 Causality Papers from Bengio's Lab, MILA](#42-causality-papers-from-bengios-lab-mila)
    - [Motivational Position Papers](#motivational-position-papers)
    - [Applying Causality Knowledge for RL Interaction Design](#applying-causality-knowledge-for-rl-interaction-design)
    - [Applying causality to model design](#applying-causality-to-model-design)
    - [Causal induction from interventional data](#causal-induction-from-interventional-data)
    - [Grounded AI](#grounded-AI)
  - [4.3 Other Causality Papers (Potentially Applicable to NLP)](#43-other-causality-papers-potentially-applicable-to-nlp)
  - [4.4 Books (for Systematic Learning)](#44-books-for-systematic-learning)
  - [4.5 Online Courses](#45-online-courses)
  - [4.6 People Directory](#46-people-directory)
  - [4.7 Workshops](#47-workshops)
  - [4.8 Others](#48-others)
- [Contributions](#contributions)
- [How to Cite This Repo](#How-to-Cite-This-Repo)

## 1. Causality Basics

### 1.1 Talks, Tutorial, etc

Talks and Tutorials:

1. (CausalNLP) **Bernhard's Talk on Towards Causal NLP.** [[Video@EMNLP 2021 Workshop](https://www.youtube.com/watch?v=Zwt1jJxVSvg&list=PLtVBX_ld338UTeq9LphgjCfMpM2EcSbEs&index=1)]
2. (Vivid, beginner-friendly) **Yoshua Bengio's Primer on the Future of Causality&NLP.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]

Seminars:


1. (Global, weekly reading group) **Online Causal Inference Seminar.** Organized by Stanford, ETH, etc. [[speakers](https://sites.google.com/view/ocis/home#h.13whjoi1jght)] [[past recordings](https://sites.google.com/view/ocis/past-talks-and-recordings)] 

   Every Tuesdays at 8:30 am PT (11:30 am ET / 4:30 pm London / 5:30 pm Berlin).
1. (Current) **Causal Seminar@Harvard Data Science Institute.** [[talks](https://datascience.harvard.edu/event-category/causal-inference/)]
1. (2021, Recordings available) **Beyond i.i.d. learning:
   Causality, dynamics, and interactions.** ETH Seminar by Prof Michael Muehlebach, Bernhard Schölkopf, Andreas Krause. [[past recordings](https://beyond-iid-learning.xyz/lectures/)]

Motivational Materials:

1. (2002 AI Magazine) **Reasoning with Cause and Effect.** _Judea Pearl_. [[pdf](https://ftp.cs.ucla.edu/pub/stat_ser/r265-ai-mag.pdf)]
2. (Blog) **ML beyond Curve Fitting: An Intro to Causal Inference and do-Calculus.** _Ferenc Huszár_. [[blog](https://www.inference.vc/untitled/)]
3. (Blog) **Causal Analysis in Theory and Practice.** Judea Pearl's [[blog](http://causality.cs.ucla.edu/blog/)]
4. (Videos course to introduce a series of concepts) **Introduction to Causal Inference** [[Video](https://www.youtube.com/c/BradyNealCausalInference)]

### 1.2 Overview Papers

1. (2021 IEEE, Overview by Schoelkopf+) **Towards Causal Representation Learning.** _Bernhard Schölkopf, Francesco Locatello, Stefan Bauer, Nan Rosemary Ke, Nal Kalchbrenner, Anirudh Goyal, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/2102.11107.pdf)] 
2. (2021 Survey) **Causal Inference in Natural Language Processing: Estimation, Prediction, Interpretation and Beyond.** _Amir Feder, Katherine A. Keith, Emaad Manzoor, Reid Pryzant, Dhanya Sridhar, Zach Wood-Doughty, Jacob Eisenstein, Justin Grimmer, Roi Reichart, Margaret E. Roberts, Brandon M. Stewart, Victor Veitch, Diyi Yang_. [[pdf](https://arxiv.org/pdf/2109.00725.pdf)]
3. (2019 Overview, Schoelkopf) **Causality for Machine Learning.** _Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]
4. (2018 ACM CSUR) **A Survey of Learning Causality with Data: Problems and Methods.** _Ruocheng Guo, Lu Cheng, Jundong Li, P. Richard Hahn, Huan Liu_. [[pdf](https://arxiv.org/pdf/1809.09337.pdf)]
5. (2015 Political Analysis) **The Statistics of Causal Inference: A View from Political Methodology.** *Luke Keele*. [[pdf](https://hrr.w.uib.no/files/2019/01/Keele_2015_causal.pdf)]



### 1.3 Toolboxes

#### Causal Discovery

1. (2021) **causal-learn (Python package for causal discovery).** _Carnegie Mellon University_. [[GitHub](https://github.com/cmu-phil/causal-learn)] [[documentation](https://causal-learn.readthedocs.io/en/latest/)] 
2. (2019) **Causal Discovery Toolbox in Python.** [[GitHub](https://github.com/FenTechSolutions/CausalDiscoveryToolbox)] [[pdf](https://arxiv.org/pdf/1903.02278.pdf)] 
3. **Causal discovery tools.** _University of Pittsburgh/Carnegie Mellon University Center for Causal Discovery_. [[link](https://www.ccd.pitt.edu/tools/)]
   <br>e.g., Tretrad, [py-causal](https://bd2kccd.github.io/docs/py-causal/) 

#### Causal Effect Estimation

1. (2020) **DoWhy: An End-to-End Library for Causal Inference.** _Amit Sharma, Emre Kiciman_. [[GitHub](https://github.com/microsoft/dowhy)] [[pdf](https://arxiv.org/pdf/2011.04216.pdf)]
2. (2023) **Ananke: A module for causal inference.** *Jaron J. R. Lee, Rohit Bhattacharya, Razieh Nabi, Ilya Shpitser*. [[link](https://ananke.readthedocs.io/en/latest/#)] [[pdf](https://arxiv.org/pdf/2301.11477)]
3. (2020) **CausalML: Python Package for Causal Machine Learning.** [[GitHub](https://github.com/uber/causalml)] [[pdf](https://arxiv.org/pdf/2002.11631.pdf)]

#### Papers that give a taxonomy of methods

1. (2021, Survey on continuous optimization for causal discovery) **D’ya like DAGs? A Survey on Structure Learning and Causal Discovery.** _Matthew J. Vowels, Necati Cihan Camgoz, Richard Bowden_. [[pdf](https://arxiv.org/pdf/2103.02582.pdf)]
2. (2018 ACM CSUR) **A Survey of Learning Causality with Data: Problems and Methods.** _Ruocheng Guo, Lu Cheng, Jundong Li, P. Richard Hahn, Huan Liu_. [[pdf](https://arxiv.org/pdf/1809.09337.pdf)]
3. (2018, National Science Review) **Learning causality and causality-related learning: some recent progress.** _Kun Zhang, Bernhard Schölkopf, Peter Spirtes, Clark Glymour_. [[pdf](https://academic.oup.com/nsr/article/5/1/26/4638533)]
4. (2016) **Causal discovery and inference: Concepts and recent methodological advances.** [[pdf](https://link.springer.com/content/pdf/10.1186/s40535-016-0018-x.pdf)]
5. (2019 Front. Genet.) **Review of Causal Discovery Methods Based on Graphical Models.** _Clark Glymour, Kun Zhang, Peter Spirtes_. [[pdf](https://www.frontiersin.org/articles/10.3389/fgene.2019.00524/full)]

## 2. Causality Applied to General NLP

### 2.1 Overview

1. (2024 arXiv) **Large Language Models and Causal Inference in Collaboration: A Comprehensive Survey.**
   _Xiaoyu Liu, Paiheng Xu, Junda Wu, Jiaxin Yuan, Yifan Yang, Yuhang Zhou, Fuxiao Liu, Tianrui Guan, Haoliang Wang, 
   Tong Yu, Julian McAuley, Wei Ai, Furong Huang_.
   [[pdf](https://arxiv.org/pdf/2403.09606)]
2. (2022 TACL) **Causal Inference in Natural Language Processing: Estimation, Prediction, Interpretation and Beyond.**
   _Amir Feder, Katherine A. Keith, Emaad Manzoor, Reid Pryzant, Dhanya Sridhar, Zach Wood-Doughty, Jacob Eisenstein, 
   Justin Grimmer, Roi Reichart, Margaret E. Roberts, Brandon M. Stewart, Victor Veitch, Diyi Yang_.
   [[pdf](https://arxiv.org/abs/2109.00725)]
3. (2024 arXiv) **The Odyssey of Commonsense Causality: From Foundational Benchmarks to Cutting-Edge Reasoning.**
   *Shaobo Cui, Zhijing Jin, Bernhard Schölkopf, Boi Faltings*.
   [[pdf](https://arxiv.org/pdf/2406.19307)]

### 2.2 Causal Reasoning



#### 2.2.1 Formal Causal Reasoning

##### Whether LLMs can do causal reasoning with established solutions

1. (2023 NeurIPS) **CLadder: Assessing Causal Reasoning in Language Models.**
   _Zhijing Jin*, Yuen Chen*, Felix Leeb*, Luigi Gresele*, Ojasv Kamal, Zhiheng LYU, Kevin Blin, Fernando Gonzalez Adauto, Max Kleiman-Weiner, Mrinmaya Sachan, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/pdf/2312.04350)]

2. (2024 ICLR) **Can Large Language Models Infer Causation from Correlation?**
   _Zhijing Jin*, Jiarui Liu*, Zhiheng Lyu, Spencer Poff, Mrinmaya Sachan, Rada Mihalcea, Mona Diab†, Bernhard Schölkopf†_.
   [[pdf](https://arxiv.org/pdf/2306.05836)]

3. (2023 TMLR) **Causal Parrots: Large Language Models May Talk Causality But Are Not Causal.**
   _Matej Zečević, Moritz Willig, Devendra Singh Dhami, Kristian Kersting_.
   [[pdf](https://arxiv.org/pdf/2308.13067)]

4. (2024 TMLR) **Causal Reasoning and Large Language Models: Opening a New Frontier for Causality.**
   _Emre Kıcıman, Robert Ness, Amit Sharma, Chenhao Tan_.
   [[pdf](https://arxiv.org/pdf/2305.00050)]

5. (2024 ACL Findings) **Are LLMs Capable of Data-based Statistical and Causal Reasoning? Benchmarking Advanced 
   Quantitative Reasoning with Data.**
   _Xiao Liu, Zirui Wu, Xueqing Wu, Pan Lu, Kai-Wei Chang, Yansong Feng_.
   [[pdf](https://arxiv.org/pdf/2402.17644)]

6. (2024 arXiv) **LLMs Are Prone to Fallacies in Causal Inference.**

   *Nitish Joshi, Abulhair Saparov, Yixin Wang, He He*.

   [[pdf](https://arxiv.org/pdf/2406.12158)]

7. (2024 arXiv) **CLEAR: Can Language Models Really Understand Causal Graphs?**
   _Sirui Chen, Mengying Xu, Kun Wang, Xingyu Zeng, Rui Zhao, Shengjie Zhao, Chaochao Lu_. 
   [[pdf](https://arxiv.org/pdf/2406.16605)]

8. (2024 arXiv) **Evaluating Interventional Reasoning Capabilities of Large Language Models.**
   _Tejas Kasetty, Divyat Mahajan, Gintare Karolina Dziugaite, Alexandre Drouin, Dhanya Sridhar_.
   [[pdf](https://arxiv.org/pdf/2404.05545)]

##### LLMs to Help Causal Effect Estimation

1. (2024 arXiv) **End-To-End Causal Effect Estimation from Unstructured Natural Language Data.**
   _Nikita Dhawan, Leonardo Cotta, Karen Ullrich, Rahul G. Krishnan, Chris J. Maddison_.
   [[pdf](https://arxiv.org/pdf/2407.07018)]

##### LLMs to Help Causal Relation Discovery

1. (2023 SPIGM Workshop at ICML) **Causal Discovery with Language Models as Imperfect Experts.**
   _Stephanie Long, Alexandre Piché, Valentina Zantedeschi, Tibor Schuster, Alexandre Drouin_.
   [[pdf](https://arxiv.org/pdf/2307.02390)]
2. (2024 arXiv) **Efficient Causal Graph Discovery Using Large Language Models.**
   _Thomas Jiralerspong, Xiaoyin Chen, Yash More, Vedant Shah, Yoshua Bengio_.
   [[pdf](https://arxiv.org/pdf/2402.01207)]
3. (2023 arxiv) **From Query Tools to Causal Architects: Harnessing Large Language Models for Advanced Causal Discovery from Data.**
    _Taiyu Ban, Lyvzhou Chen, Xiangyu Wang, Huanhuan Chen_.
    [[pdf](https://arxiv.org/abs/2306.16902)]
4. (2024 arviv) **ALCM: Autonomous LLM-Augmented Causal Discovery Framework.**
    _Elahe Khatibi, Mahyar Abbasian, Zhongqi Yang, Iman Azimi, Amir M. Rahmani_.
    [[pdf](https://arxiv.org/abs/2405.01744)]
5. (2024 arxiv) **Large Language Models are Effective Priors for Causal Graph Discovery.**
    _Victor-Alexandru Darvariu, Stephen Hailes, Mirco Musolesi_.
    [[pdf](https://arxiv.org/abs/2405.13551)]
6. (2024 arxiv) **Multi-Agent Causal Discovery Using Large Language Models.**
    _Hao Duong Le, Xin Xia, Zhang Chen_.
    [[pdf](https://arxiv.org/abs/2407.15073)]
7. (2024 arxiv) **Bridging Causal Discovery and Large Language Models: A Comprehensive Survey of Integrative Approaches and Future Directions.**
    _Guangya Wan, Yuqi Wu, Mengxuan Hu, Zhixuan Chu, Sheng Li_.
    [[pdf](https://arxiv.org/abs/2402.11068)]
8. (2024 arxiv) **Large Language Models for Constrained-Based Causal Discovery.**
    _Kai-Hendrik Cohrs, Gherardo Varando, Emiliano Diaz, Vasileios Sitokonstantinou, Gustau Camps-Valls_.
    [[pdf](https://arxiv.org/abs/2406.07378)]
9. (2024 arxiv) **Causal Graph Discovery with Retrieval-Augmented Generation based Large Language Models.**
    _Yuzhe Zhang, Yipeng Zhang, Yidong Gan, Lina Yao, Chen Wang_.
    [[pdf](https://arxiv.org/abs/2402.15301)]
10. (2024 SSRN) **Towards Automating Causal Discovery in Financial Markets and Beyond.**
    _Alik Sokolov, Fabrizzio Sabelli, Behzad Azadie faraz, Wuding Li, Luis Seco_.
    [[pdf](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4679414)]
11. (2024 COLM) **LLM4Causal: Democratized Causal Tools for Everyone via Large Language Model.**
    _Haitao Jiang, Lin Ge, Yuhe Gao, Jianian Wang, Rui Song_.
    [[pdf](https://openreview.net/attachment?id=H1Edd5d2JP&name=pdf)]
12. (2024 arxiv) **Knowledge Graph Structure as Prompt: Improving Small Language Models Capabilities for Knowledge-based Causal Discovery.**
    _Yuni Susanti, Michael Färber_.
    [[pdf](https://arxiv.org/abs/2407.18752)]
13. (2024 ACL) **Open Event Causality Extraction by the Assistance of LLM in Task Annotation, Dataset, and Method.**
    _Kun Luo, Tong Zhou, Yubo Chen, Jun Zhao, Kang Liu_.
    [[pdf](https://aclanthology.org/2024.neusymbridge-1.4/)]
14. (2023 arxiv) **Causal Discovery with Language Models as Imperfect Experts.**
    _Stephanie Long, Alexandre Piché, Valentina Zantedeschi, Tibor Schuster, Alexandre Drouin_.
    [[pdf](https://arxiv.org/abs/2307.02390)]
15. (2024 ACL) **Identifying while Learning for Document Event Causality Identification.**
    _Cheng Liu, Wei Xiang, Bang Wang_.
    [[pdf](https://arxiv.org/abs/2405.20608)]
#### 2.2.2 Commonsense/Empirical Causal Reasoning

1. (2024 arXiv) **The Odyssey of Commonsense Causality: From Foundational Benchmarks to Cutting-Edge Reasoning.**
   *Shaobo Cui, Zhijing Jin, Bernhard Schölkopf, Boi Faltings*.
   [[pdf](https://arxiv.org/pdf/2406.19307)]
2. (2022 arXiv) **Causal Inference Principles for Reasoning about Commonsense Causality.**
   _Jiayao Zhang, Hongming Zhang, Dan Roth, Weijie J. Su_.
   [[pdf](https://arxiv.org/pdf/2202.00436.pdf)]
3. (2021 ACL Findings) **Empowering Language Understanding with Counterfactual Reasoning.** _Fuli Feng, Jizhi Zhang, Xiangnan He, Hanwang Zhang, Tat-Seng Chua_. [[pdf](https://arxiv.org/pdf/2106.03046.pdf)]
4. (2021 ARR) **e-CARE: a New Dataset for Exploring Explainable Causal Reasoning.** _Anonymous_. [[pdf](https://openreview.net/pdf?id=48T0DriwGcv)]
5. (2020 EMNLP) **GLUCOSE: GeneraLized and COntextualized Story Explanations.** _Nasrin Mostafazadeh, Aditya Kalyanpur, Lori Moon, David Buchanan, Lauren Berkowitz, Or Biran, Jennifer Chu-Carroll_.
   [[pdf](https://arxiv.org/pdf/2009.07758.pdf)]
6. (2019 EMNLP) **Counterfactual Story Reasoning and Generation.**
   _Lianhui Qin, Antoine Bosselut, Ari Holtzman, Chandra Bhagavatula, Elizabeth Clark, Yejin Choi_. [[pdf](https://arxiv.org/pdf/1909.04076.pdf)]
7. (2020 IJCAI) **Guided Generation of Cause and Effect.** _Zhongyang Li, Xiao Ding, Ting Liu, J. Edward Hu, Benjamin Van Durme_.
   [[pdf](https://www.ijcai.org/Proceedings/2020/0502.pdf)] [[video](https://www.ijcai.org/proceedings/2020/video/24610)]
   <br>[Summary] 314 million automatically extracted cause and effects.

#### 2.2.3 Both Types of Causal Reasoning

1. (2024 AAAI Workshop) **A Critical Review of Causal Reasoning Benchmarks for Large Language Models**. 

   *Linying Yang, Vik Shirvaikar, Oscar Clivio, Fabian Falck.* 

   [[pdf](https://arxiv.org/pdf/2407.08029)]

2. (2024 arXiv) **C2P: Featuring Large Language Models with Causal Reasoning.** 

   *Abdolmahdi Bagheri, Matin Alinejad, Kevin Bello, Alireza Akhondi-Asl*.

   [[pdf](https://arxiv.org/pdf/2407.18069)]




### 2.3 Interpretability by Causal Methods

1. (2023 ACL) **A Causal Framework to Quantify the Robustness of Mathematical Reasoning in Language Models.**
   _Alessandro Stolfo*, Zhijing Jin*, Kumar Shridhar, Bernhard Schoelkopf, Mrinmaya Sachan_.
   [[pdf](https://arxiv.org/pdf/2210.12023.pdf)]

2. (2022 ACL Findings) **Interpreting the Robustness of Neural NLP Models to Textual Perturbations.**
   _Yunxiang Zhang, Liangming Pan, Samson Tan, Min-Yen Kan_. [[pdf](https://arxiv.org/pdf/2110.07159.pdf)]
3. (2020 NeurIPS Spotlight) **Causal Mediation Analysis for Interpreting Neural NLP:
   The Case of Gender Bias.** _Jesse Vig, Sebastian Gehrmann, Yonatan Belinkov, Sharon Qian, Daniel Nevo, Simas Sakenis, Jason Huang, Yaron Singer, Stuart Shieber_. [[pdf](https://arxiv.org/pdf/2004.12265.pdf)]
   <br>[Summary] Cause: input text, mediator: some neurons, effect: output prediction

4. (2021 NeurIPS) **Causal Abstractions of Neural Networks.**
   _Atticus Geiger, Hanson Lu, Thomas Icard, Christopher Potts_. [[pdf](https://arxiv.org/pdf/2106.02997.pdf)]
5. (2021 arXiv) **Probing Classifiers: Promises, Shortcomings, and Advances.** _Yonatan Belinkov_. [[pdf](https://arxiv.org/pdf/2102.12452.pdf)]
6. (2021 ACL) **Causal Analysis of Syntactic Agreement Mechanisms in Neural Language Models.**
   _Matthew Finlayson, Aaron Mueller, Sebastian Gehrmann, Stuart Shieber, Tal Linzen, Yonatan Belinkov_. [[pdf](https://arxiv.org/pdf/2106.06087.pdf)]
7. (2021 CoNLL) **Counterfactual Interventions Reveal the Causal Effect of Relative Clause Representations on Agreement Prediction.**
   _Shauli Ravfogel, Grusha Prasad, Tal Linzen, Yoav Goldberg_.
   [[pdf](https://arxiv.org/pdf/2105.06965.pdf)]
8. (2021 arXiv) **Causal Distillation for Language Models.**
   _Zhengxuan Wu, Atticus Geiger, Josh Rozner, Elisa Kreiss, Hanson Lu, Thomas Icard, Christopher Potts, Noah D. Goodman_. [[pdf](https://arxiv.org/pdf/2112.02505.pdf)]
9. (2021 arXiv) **Inducing Causal Structure for Interpretable Neural Networks.**
   _Atticus Geiger, Zhengxuan Wu, Hanson Lu, Josh Rozner, Elisa Kreiss, Thomas Icard, Noah D. Goodman, Christopher Potts_. [[pdf](https://arxiv.org/pdf/2112.00826.pdf)] [[slides](https://web.stanford.edu/~cgpotts/talks/potts-mcgill2022-slides.pdf)]

10. (2020 CL) **CausaLM: Causal Model Explanation Through Counterfactual Language Models.**
    _Amir Feder, Nadav Oved, Uri Shalit, Roi Reichart_. [[pdf](https://arxiv.org/pdf/2005.13407.pdf)]

11. (2020 TACL) **Amnesic Probing: Behavioral Explanation with Amnesic Counterfactuals.** _Yanai Elazar, Shauli Ravfogel, Alon Jacovi, Yoav Goldberg_. [[pdf](https://arxiv.org/pdf/2006.00995.pdf)]

12. (2020 ICLR) **Learning the Difference that Makes a Difference with Counterfactually-Augmented Data.**
    _Divyansh Kaushik, Eduard Hovy, Zachary C. Lipton_. [[pdf](https://arxiv.org/pdf/1909.12434.pdf)]

### 2.4 Text Features in Causal Graphs (for Social Science, Psychology, etc.)

1. (2021 EMNLP Findings) **Mining the Cause of Political Decision-Making from Social Media: A Case Study of COVID-19 Policies across the US States**
   _Zhijing Jin, Zeyu Peng, Tejas Vaidhya, Bernhard Schoelkopf, Rada Mihalcea_. [[pdf](https://drive.google.com/file/d/1Y2Wcn8D9sBcSi4Or0cR7gxA2jZ5jUUQE/view?usp=sharing)] [[talk](https://drive.google.com/file/d/1Qs80sva7HvKFLu_T25r3BvGdIvzdJJ5l/)]

2. (2021 arXiv) **Generating Synthetic Text Data to Evaluate Causal Inference Methods.** _Zach Wood-Doughty, Ilya Shpitser, Mark Dredze_. [[pdf](https://arxiv.org/pdf/2102.05638.pdf)]

3. (2020 ACL) **Text and Causal Inference: A Review of Using Text to Remove Confounding from Causal Estimates.** _Katherine A. Keith, David Jensen, and Brendan O'Connor_. [[pdf](https://www.aclweb.org/anthology/2020.acl-main.474.pdf)]

4. (2020 UAI) **Adapting Text Embeddings for Causal Inference.** _Victor Veitch, Dhanya Sridhar, David M. Blei_. [[pdf](https://arxiv.org/pdf/1905.12741.pdf)]

5. (2020 AJPS) **Adjusting for confounding with text matching.**
   _Margaret E Roberts, Brandon M Stewart, and Richard A Nielsen_. [[pdf](http://www.mit.edu/~rnielsen/textmatching.pdf)]

6. (2020 arXiv) **Adjusting for Confounders with Text: Challenges and an Empirical Evaluation Framework for Causal Inference.** _Galen Weld, Peter West, Maria Glenski, David Arbour, Ryan Rossi, Tim Althoff_. [[pdf](https://arxiv.org/pdf/2009.09961.pdf)]

7. (2020 CSCW) **Quantifying the Causal Effects of Conversational Tendencies.** _Justine Zhang, Sendhil Mullainathan, Cristian Danescu-Niculescu-Mizil_. [[pdf](https://arxiv.org/pdf/2009.03897.pdf)]

8. (2020 arXiv) **Causal Effects of Linguistic Properties.** _Reid Pryzant, Dallas Card, Dan Jurafsky, Victor Veitch, Dhanya Sridhar_. [[pdf](https://arxiv.org/pdf/2010.12919.pdf)] [[blog](http://ai.stanford.edu/blog/text-causal-inference/) and [github](https://github.com/rpryzant/causal_selection)]
   <br>[Summary] Cause: binary writer intent, confounder: other linguistic habits of the writer, mediator: text by the writer, effect: reader's response time

9. (2020 arXiv) **Decoupling entrainment from consistency using deep neural networks.** [[pdf](https://arxiv.org/pdf/2011.01860.pdf)]
   <br>[Note] Entrainment = speakers adapting to conversation partners so as to become more similar

10. (2018 EMNLP) **Challenges of Using Text Classifiers for Causal Inference.**
    _Zach Wood-Doughty, Ilya Shpitser, Mark Dredze_. [[pdf](https://arxiv.org/pdf/1810.00956.pdf)]

11. (2018 Political Analysis) **Matching with text data: An experimental evaluation of methods for matching documents and of measuring match quality.**
    _Reagan Mozer, Luke Miratrix, Aaron Russell Kaufman, L Jason Anastasopoulos_. [[pdf](https://arxiv.org/pdf/1801.00644.pdf)]

12. (2018 arXiv) **How to Make Causal Inferences Using Texts.** _Naoki Egami, Christian J. Fong, Justin Grimmer, Margaret E. Roberts, Brandon M. Stewart_. [[pdf](https://arxiv.org/pdf/1802.02163.pdf)]

13. (2017 EMNLP) **Detecting and Explaining Causes From Text For a Time Series Event.**
    _Dongyeop Kang, Varun Gangal, Ang Lu, Zheng Chen, Eduard Hovy_.
    [[pdf](https://arxiv.org/pdf/1707.08852.pdf)]
    <br>[Summary] Finding causes for the stock price time series.

14. (2016 ACL) **Discovery of Treatments from Text Corpora.** _Christian Fong, Justin Grimmer_. [[pdf](https://www.aclweb.org/anthology/P16-1151.pdf)]
15. (2016 JMLR) **Learning representations for counterfactual inference.**
    _Fredrik Johansson, Uri Shalit, David Sontag_. [[pdf](http://proceedings.mlr.press/v48/johansson16.pdf)]


### 2.5 Causality to Bring Insights to NLP Modeling (for Robustness, Domain Adaptation, etc)

1. (2023 ICML) **Towards Trustworthy Explanation: On Causal Rationalization.**
   _Wenbo Zhang, Tong Wu, Yunlong Wang, Yong Cai, Hengrui Cai_.[[pdf](https://arxiv.org/abs/2306.14115)]

2. (2023) **Towards Trustworthy and Aligned Machine Learning: A Data-centric Survey with Causality Perspectives.**
   _Haoyang Liu, Maheep Chaudhary, Haohan Wang_.
   [[pdf](https://arxiv.org/pdf/2307.16851.pdf)]

3. (2021 EMNLP Oral) **Causal Direction of Data Collection Matters: Implications of Causal and Anticausal Learning for NLP.**
   _Zhijing Jin*, Julius von Kügelgen*, Jingwei Ni, Tejas Vaidhya, Ayush Kaushal, Mrinmaya Sachan, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/2110.03618)] [[talk](https://drive.google.com/file/d/19dFDslovDFzBgkXN5lKrgV9xP8kWrB5e/)]

4. (2021 arXiv) **Counterfactual Invariance to Spurious Correlations: Why and How to Pass Stress Tests.** _Victor Veitch, Alexander D'Amour, Steve Yadlowsky, Jacob Eisenstein_. [[pdf](https://arxiv.org/pdf/2106.00545.pdf)]

5. (2021 CVPR) **Counterfactual VQA: A Cause-Effect Look at Language Bias.** _Yulei Niu, Kaihua Tang, Hanwang Zhang, Zhiwu Lu, Xian-Sheng Hua, Ji-Rong Wen_. [[pdf](https://arxiv.org/pdf/2006.04315.pdf)]
6. (2021 ICLR Workshop) **A Causal Lens for Controllable Text Generation.** _Zhiting Hu, Li Erran Li_.
   [[pdf](https://sites.google.com/connect.hku.hk/robustml-2021/accepted-papers/paper-089)]

7. (2021 EMNLP) **Uncovering Main Causalities for Long-tailed Information Extraction.** _Guoshun Nan, Jiaqi Zeng, Rui Qiao, Zhijiang Guo, Wei Lu_. [[pdf](https://arxiv.org/pdf/2109.05213.pdf)]
8. (2021 ACL findings) **Discovering Topics in Long-tailed Corpora with Causal Intervention.** _Xiaobao Wu, Chunping Li, Yishu Miao_. [[pdf](https://aclanthology.org/2021.findings-acl.15.pdf)]
9. (2020 EMNLP) **Unsupervised Discovery of Implicit Gender Bias.** _Anjalie Field, Yulia Tsvetkov_. [[pdf](https://www.aclweb.org/anthology/2020.emnlp-main.44.pdf)]
   <br>[Summary] Method: propensity matching and adversarial learning.
10. (2020 EMNLP) **Counterfactual Generator: A Weakly-Supervised Method for Named Entity Recognition.**
    _Xiangji Zeng, Yunliang Li, Yuchen Zhai, Yin Zhang_. [[pdf](https://aclanthology.org/2020.emnlp-main.590.pdf)]
11. (2020 EMNLP) **De-Biased Court’s View Generation with Causality.** _Yiquan Wu, Kun Kuang, Yating Zhang, Xiaozhong Liu, Changlong Sun, Jun Xiao, Yueting Zhuang, Luo Si, Fei Wu_. [[pdf](https://aclanthology.org/2020.emnlp-main.56.pdf)]
12. (2020 EMNLP Findings) **Identifying Spurious Correlations for Robust Text Classification.** _Zhao Wang, Aron Culotta_. [[pdf](https://aclanthology.org/2020.findings-emnlp.308.pdf)]
13. (2020 EMNLP) **Counterfactual Off-Policy Training for Neural Dialogue Generation.** _Qingfu Zhu, Weinan Zhang, Ting Liu, William Yang Wang_. [[pdf](https://aclanthology.org/2020.emnlp-main.276)]
14. (2019 EMNLP) **Topics to Avoid: Demoting Latent Confounds in Text Classification.** _Sachin Kumar, Shuly Wintner, Noah A. Smith, Yulia Tsvetkov_. [[pdf](https://arxiv.org/pdf/1909.00453.pdf)]
    <br>[Summary] Cause: native language, confounder: topic, effect: text

15. (2018 NAACL, Stanford) **Deconfounded lexicon induction for interpretable social science.** _Reid Pryzant, Kelly Shen, Dan Jurafsky, Stefan Wagner_. [[pdf](https://www.aclweb.org/anthology/N18-1146.pdf)]
    <br>[Summary] Cause: some keywords, effect: output prediction

#### Related NLP Papers


##### Data augmentation

1. (2021 NAACL) **Counterfactual Data Augmentation for Neural Machine Translation.** _Qi Liu, Matt Kusner, Phil Blunsom_. [[pdf](https://www.aclweb.org/anthology/2021.naacl-main.18.pdf)]
   <br>[Summary] First do phrase alignment between source and target sentences, and then only change some phrases in the source sentence, expecting the target sentence also only changes by that key phrase. Not much usage of causality.

2. (2019 ACL) **Counterfactual Data Augmentation for Mitigating Gender Stereotypes in Languages with Rich Morphology.** _Ran Zmigrod, Sabrina J. Mielke, Hanna Wallach, Ryan Cotterell_. [[pdf](https://www.aclweb.org/anthology/P19-1161.pdf)]
   <br>[Summary] Change female words to male words in languages with rich morphology and inflections. Not much usage of causality.

##### Compositionality and Neuro-Symbolic Approaches

1. (2022 arXiv) **Compositionality as Lexical Symmetry.**
   _Ekin Akyürek, Jacob Andreas_. [[pdf](https://arxiv.org/pdf/2201.12926.pdf)]
2. (2021 NeurIPS) **Improving Coherence and Consistency in Neural
   Sequence Models with Dual-System,
   Neuro-Symbolic Reasoning.**
   _Maxwell Nye, Michael Henry Tessler, Joshua B. Tenenbaum, Brenden M. Lake_.
   [[pdf](https://proceedings.neurips.cc/paper/2021/file/d3e2e8f631bd9336ed25b8162aef8782-Paper.pdf)]

#### Related Non-NLP Papers

1. (2021 arXiv) **Desiderata for Representation Learning: A Causal Perspective.** _Yixin Wang, Michael I. Jordan_. [[pdf](https://arxiv.org/pdf/2109.03795.pdf)]
   <br>[Summary] The causal predictors of a task should be both necessary and sufficient factors.

##### Causality tools that can be applied to deconfound

1. (2017 NIPS, MPI, discover causal graphs behind data) **Avoiding Discrimination through Causal Reasoning.** _Niki Kilbertus, Mateo Rojas-Carulla, Giambattista Parascandolo, Moritz Hardt, Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1706.02744.pdf)]


##### Related CV papers on counterfactual generation:

1. (2021 ICLR) **Counterfactual Generative Networks.** _Axel Sauer, Andreas Geiger_. [[pdf](https://openreview.net/pdf?id=BXewfAYMmJw)]

### 2.6 Causal Relation Extraction

#### Surveys and Reviews

1. **CREST: A Causal Relation Schema for Text (A repo containing datasets for causal/counterfactual relation extraction)** _Pedram Hosseini_. [[GitHub](https://github.com/phosseini/CREST)]
   <br>[Summary] CausalRE datasets: SemEval 2007 Task 4 (114 causal sentences), SemEval 2021 Task 8 (1,331), EventCausality (485), Causal-TimeBank (318), EventStoryLine v1.5 (2,608), CaTeRS (308), BECauSE v2.1 (554), Choice of Plausible Alternatives (COPA) (1,000), The Penn Discourse Treebank (PDTB) 3.0 (7,991).

2. (2020 COLING) **A Review of Dataset and Labeling Methods for Causality Extraction.** _Jinghang Xu, Wanli Zuo, Shining Liang, Xianglin Zuo_. [[pdf](https://www.aclweb.org/anthology/2020.coling-main.133.pdf)]
   <br>[Summary] Very reader-friendly survey, including ideas such as Causal connectives (verb: cause, result; conjunction: because, so; preposition: for, because of; adverb: consequently; Verb Phrase: result in, lead to; Prepositional phrase: as a result of; Clause: that's why, so that); Causal concepts (sufficient, necessary, temporal); etc.

3. (2016 arXiv) **Automatic Extraction of Causal Relations from Natural Language Texts: A Comprehensive Survey.** _Nabiha Asghar_. [[GitHub](https://arxiv.org/pdf/1605.07895.pdf)]
   <br>[Summary] Automatic discovery of linguistic patterns expressing causal relations, such as 1995's work using patterns like "because [cause], [effect]", 2002's work using patterns like "NP1-CausativeVerb-NP2", later work using a Naive Bayes classifier, and many more.

4. (2018 CMU Thesis) **Annotating and Automatically Tagging Constructions of Causal Language.**
   _Jesse Dunietz_. [[pdf](https://jessedunietz.com/assets/publications/thesis.pdf)] 

5. (2021 arXiv) **A Survey on Extraction of Causal Relations from Natural Language Text.**
   _Jie Yang, Soyeon Caren Han, Josiah Poon_. [[pdf](https://arxiv.org/pdf/2101.06426.pdf)]

6. **Richer Event Description (RED) Annotation Guidelines.** _Martha Palmer, Will Styler, Kevin Crooks, Tim O'Gorman_.
   [[GitHub](https://github.com/timjogorman/RicherEventDescription/blob/master/guidelines.md)]

7. (2020 Thesis) **Narrative Generation to Support Causal Exploration of Directed Graphs.** 
   _Arjun Choudhry_. [[pdf](https://vtechworks.lib.vt.edu/bitstream/handle/10919/98670/Choudhry_A_T_2020.pdf?sequence=1&isAllowed=y)]

#### Method or Dataset Papers

##### Causal relation extraction from web data

1. (2019 EMNLP) **Weakly Supervised Multilingual Causality Extraction from Wikipedia.**
   _Chikara Hashimoto_. 
   [[pdf](https://www.aclweb.org/anthology/D19-1296.pdf)]
   <br>[Summary] Cross-verification between Wikipedia and Wikidata, e.g., "Protectionism causes Trade war"

2. (2016 ACL) **Identifying Causal Relations Using Parallel Wikipedia Articles.**
   _Christopher Hidey, Kathy McKeown_.
   [[pdf](https://www.aclweb.org/anthology/P16-1135.pdf)]
   <br>[Summary] Find linguistic markers like "because".

3. (2014 ACL) **Toward Future Scenario Generation: Extracting Event Causality Exploiting Semantic Relation, Context, and Association Features**
   _Chikara Hashimoto, Kentaro Torisawa, Julien Kloetzer, Motoki Sano, István Varga, Jong-Hoon Oh, Yutaka Kidawara_.
   [[pdf](https://www.aclweb.org/anthology/P14-1093.pdf)]

4. (2012 EMNLP) **Excitatory or Inhibitory: A New Semantic Orientation Extracts Contradiction and Causality from the Web.**
   _Chikara Hashimoto, Kentaro Torisawa, Stijn De Saeger, Jong-Hoon Oh, Jun’ichi Kazama_.
   [[pdf](https://www.aclweb.org/anthology/D12-1057.pdf)]
   <br>[Summary] Extracted one million contradiction pairs and 500,000 causality pairs.


1. (1998 Literary and Linguistic Computing) **Automatic extraction of cause-effect information from newspaper text without knowledge-based inferencing.** _Christopher Khoo, Jaklin Kornfilt, Sung Hyon Myaeng, Robert Oddy_.
   [[pdf](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.727.5787&rep=rep1&type=pdf)]

2. (1991 Knowledge Acquisition) **Knowledge-based acquisition of causal relationships in text.**
   _Randy M. Kaplan, Genevieve Berry-Rogghe_.


##### Causal relation extraction from curated datasets (relatively small):

1. (2021 Neurocomputing) **Causality Extraction based on Self-attentive BiLSTM-CRF with Transferred Embeddings.**_Zhaoning Li, Qi Li, Xiaotian Zou, Jiangtao Ren_. [[GitHub](https://github.com/Das-Boot/scite)]

2. (2021 NAACL) **Everything Has a Cause: Leveraging Causal Inference in Legal Text Analysis**
   _Xiao Liu, Da Yin, Yansong Feng, Yuting Wu, Dongyan Zhao_. [[pdf](https://www.aclweb.org/anthology/2021.naacl-main.155.pdf)]

3. (2021 NAACL) **Graph Convolutional Networks for Event Causality Identification with Rich Document-level Structures.**
   _Minh Tran Phu and Thien Huu Nguyen_ [[pdf](https://www.aclweb.org/anthology/2021.naacl-main.273.pdf)]

4. (2020 EMNLP) **XCOPA: A Multilingual Dataset for Causal Commonsense Reasoning.** _Edoardo Maria Ponti, Goran Glavaš, Olga Majewska, Qianchu Liu, Ivan Vulić, Anna Korhonen_. [[pdf](https://arxiv.org/pdf/2005.00333.pdf)]

5. (2020 EMNLP) **Causal Inference of Script Knowledge.** _Noah Weber, Rachel Rudinger, Benjamin Van Durme_. [[pdf](https://aclanthology.org/2020.emnlp-main.612.pdf)]
6. (2019 NAACL) **Modeling Document-level Causal Structures for Event Causal Relation Identification.** _Lei Gao, Prafulla Kumar Choubey, Ruihong Huang_.
   [[pdf](https://www.aclweb.org/anthology/N19-1179.pdf)]
   <br>[Summary] EventStoryLine corpus; method: Integer Linear Programming (ILP)

7. (2018 ACL) **Joint Reasoning for Temporal and Causal Relations.** _Qiang Ning, Zhili Feng, Hao Wu, Dan Roth_. [[pdf](https://www.aclweb.org/anthology/P18-1212.pdf)]
   <br>[Summary] Method: constrained conditional models (CCMs), n integer linear programming (ILP).

8. (2018 SIGdial) **Automatic Extraction of Causal Relations from Text using Linguistically Informed Deep Neural Networks.**
   _Tirthankar Dasgupta, Rupsa Saha, Lipika Dey, Abir Naskar_.
   [[pdf](https://www.aclweb.org/anthology/W18-5035.pdf)]


1. (2017 ACL Workshop) **The Event StoryLine Corpus: A New Benchmark for Causal and Temporal Relation Extraction.**
   _Tommaso Caselli, Piek Vossen_. [[pdf](https://www.aclweb.org/anthology/W17-2711.pdf)]

2. (2017 ACL) **The BECauSE Corpus 2.0: Annotating Causality and Overlapping Relations.** 
   _Jesse Dunietz, Lori Levin, Jaime Carbonell_.
   [[pdf](https://www.aclweb.org/anthology/W17-0812/)]


1. (2016 ACL Workshop) **CaTeRS: Causal and Temporal Relation Scheme for Semantic Annotation of Event Structures.**
   _Nasrin Mostafazadeh, Alyson Grealish, Nathanael Chambers, James Allen, Lucy Vanderwende_. [[pdf](https://www.aclweb.org/anthology/W16-1007.pdf)]

2. (2016 KR) **Commonsense Causal Reasoning between Short Texts.**
   _Zhiyi Luo, Yuchen Sha, Kenny Q. Zhu, Seung-Won Hwang, Zhongyuan Wang_. [[pdf](https://www.aaai.org/ocs/index.php/KR/KR16/paper/view/12818/12498)]
   <br>[Summary] Contains a list of causal cue verbs.


1. (2015 ACL Workshop) **Annotating Causal Language Using Corpus Lexicography of Constructions.**
   _Jesse Dunietz, Lori Levin, Jaime Carbonell_.
   [[pdf](https://www.aclweb.org/anthology/W15-1622.pdf)]
   <br>[Summary] Quite important. This paper teaches the ontology for causality annotation, e.g., Degrees of Causation (cause, enable, prevent), types of causation (consequence, motivation, purpose), instance (causal connective, cause, effect), linguistic type (causality with no lexical trigger, causality with connectives, temporal language).

2. (2014 EACL) **Annotating Causality in the TempEval-3 Corpus.**
   _Paramita Mirza, Rachele Sprugnoli, Sara Tonelli, Manuela Speranza_.
   [[pdf](https://www.aclweb.org/anthology/W14-0702.pdf)]
   <br>[Summary] Containing some illustrative examples on page 3.

3. (2011 ACL) **Minimally Supervised Event Causality Identification.**
   _Quang Do, Yee Seng Chan, Dan Roth_. [[pdf](https://www.aclweb.org/anthology/D11-1027.pdf)]
   <br>[Summary] Uses PMI, IDF, etc.

4. (2009 SemEval) **SemEval-2010 Task 8: Multi-Way Classification of Semantic Relations between Pairs of Nominals**
   _Iris Hendrickx, Su Nam Kim, Zornitsa Kozareva, Preslav Nakov, Diarmuid Ó Séaghdha, Sebastian Padó, Marco Pennacchiotti, Lorenza Romano, Stan Szpakowicz_.
   [[pdf](https://www.aclweb.org/anthology/S10-1006.pdf)]

5. (2008 LREC) **Building a Corpus of Temporal-Causal Structure.** _Steven Bethard, William Corvey, Sara Klingenstein, James H. Martin_. [[pdf](http://www.lrec-conf.org/proceedings/lrec2008/pdf/229_paper.pdf)]
   <br>[Summary] Combining causal and temporal relation extraction, such as "Fuel tanks had [EVENT leaked] and [EVENT contaminated] the soil." <EVENT_leaked, causes, EVENT_contaminated>. Small dataset with 271 causal relations, and 329 BEFORE/AFTER relations.

6. (2008 LREC) **Causal Relation Extraction.**
   _Eduardo Blanco, Nuria Castell, Dan Moldovan_.
   [[pdf](http://www.lrec-conf.org/proceedings/lrec2008/pdf/87_paper.pdf)]

7. (2007 SemEval) **SemEval-2007 Task 04: Classification of Semantic Relations between Nominals.**
   _Roxana Girju, Preslav Nakov, Vivi Nastase, Stan Szpakowicz, Peter Turney, Deniz Yuret_.
   [[pdf](https://www.aclweb.org/anthology/S07-1003.pdf)]

8. (2006 IPM) **Incremental cue phrase learning and bootstrapping method for causality extraction using cue phrase and word pair probabilities.** _Du-Seong Chang, Key-Sun Choi_. [[pdf](https://dl.acm.org/doi/abs/10.1016/j.ipm.2005.04.004)] 

9. (2004 ICNLP) **Causal Relation Extraction Using Cue Phrase and Lexical Pair Probabilities.** _Du-Seong Chang, Key-Sun Choi_. [[pdf](http://semanticweb.kaist.ac.kr/home/images/a/af/Causal_Relation_Extraction_Using_Cue_Phrases_and_Lexical_Pair_Probabilities.pdf)]


1. (2003 ACL Workshop) **Automatic detection of causal relations for question answering.** _Roxana Girju_. [[pdf](https://www.aclweb.org/anthology/W03-1210.pdf)]

2. (2002 AAAI) **Text Mining for Causal Relations.** _Roxana Girju, Dan Moldovan_. [[pdf](https://www.aaai.org/Papers/FLAIRS/2002/FLAIRS02-071.pdf)]


1. (2001 PAKDD) **Semantic Expectation-Based Causation Knowledge Extraction: A Study on Hong Kong Stock Movement Analysis.**
   _Boon-Toh Low, Ki Chan, Lei-Lei Choi, Man-Yee Chin, Sin-Ling Lay_.
   [[link](https://link.springer.com/chapter/10.1007/3-540-45357-1_15)]

2. (2000 ACL) **Extracting Causal Knowledge from a Medical Database Using Graphical Patterns.**
   _Christopher S. G. Khoo, Syin Chan, Yun Niu_.
   [[pdf](https://www.aclweb.org/anthology/P00-1043.pdf)]

3. (1997) **Coatis, an nlp system to locate expressions of actions connected by causality links.** _Daniela Garcia_. [[link](https://link.springer.com/chapter/10.1007/BFb0026799)]

4. (1995 PhD Thesis) **Automatic identification of causal relations in text and their use for improving precision in information retrieval.**
   _Christopher Khoo_.
   [[pdf](https://scholar.google.com/scholar_url?url=https://repository.arizona.edu/bitstream/handle/10150/105106/chris_khoo.PhD_thesis.pdf%3Fsequence%3D1&hl=de&sa=T&oi=gsb-gga&ct=res&cd=0&d=8432224869863885584&ei=g9ymYMOVMMPtmQH3_qPYDg&scisig=AAGBfm07wHjoKM8Q_-LQaYK8Ejq1J2LR0Q)]


#### Some useful tools:

Helping to identify causal verbs, and connectives:

1. (2005 PhD Thesis) **VerbNet: A broad-coverage, comprehensive verb lexicon.** _Karin Kipper Schuler_.
   [[pdf](https://verbs.colorado.edu/~kipper/Papers/dissertation.pdf)]

2. (2009 ACL) **Using Syntax to Disambiguate Explicit Discourse Connectives in Text.** _Emily Pitler, Ani Nenkova_. [[pdf](https://www.aclweb.org/anthology/P09-2004.pdf)]


Helping to annotate data efficiently and affordably:

1. (2017 SIGMOD) **Snorkel: Fast Training Set Generation for Information Extraction.** _Alexander J. Ratner, Stephen H. Bach, Henry R. Ehrenberg, Chris Ré_. [[pdf](https://ajratner.github.io/assets/papers/ratner-sigmoddemo17.pdf)]

Helping to analyze the semantics of causal events:

1. (1998 COLING) **The Berkeley FrameNet Project.** _Collin F. Baker, Charles J. Fillmore, John B. Lowe_. [[pdf](https://www.aclweb.org/anthology/C98-1013.pdf)]

2. AMR parsing

3. (2016 ACL Workshop) **The Storyline Annotation and Representation Scheme (StaR): A Proposal.** _Tommaso Caselli, Piek Vossen_. [[pdf](https://www.aclweb.org/anthology/W16-5708.pdf)]

4. (2014 Report) **Guidelines for ECB+ Annotation of Events and their Coreference.** _Agata Cybulska, Piek Vossen_.
   [[pdf](http://www.newsreader-project.eu/files/2013/01/NWR-2014-1.pdf)]

## 3. Causality for Various Applications

### 3.1 Persuasion

1. (2020 arXiv) **Influence via Ethos: On the Persuasive Power of Reputation in Deliberation Online.** _Emaad Manzoor, George H. Chen, Dokyun Lee, Michael D. Smith_. [[pdf](https://arxiv.org/pdf/2006.00707.pdf)]
   <br>[Summary] Cause: reputation, effect: persuation in debates.

2. **Estimating Causal Effects of Tone in Online Debates.**
   _Dhanya Sridhar and Lise Getoor_. [[pdf](https://arxiv.org/pdf/1906.04177.pdf)]

### 3.2 Psychology and Behavior

1. **The effect of wording on message propagation: Topic- and author-controlled natural experiments on Twitter.** _Chenhao Tan, Lillian Lee, Bo Pang_. [[pdf](https://www.aclweb.org/anthology/P14-1017.pdf)] 
2. (CHI 2016) **Discovering shifts to suicidal ideation from mental health content in social media.** _Munmun De Choudhury, Emre Kiciman, Mark Dredze, Glen Coppersmith, Mrinal Kumar_. [[pdf](https://dl.acm.org/doi/pdf/10.1145/2858036.2858207?casa_token=ZJKLrg8LAOsAAAAA%3Aecs8HsunRyeUeD_De6Dx15_nPRZ1-mmjiXfAEXLpr25wwz6ywzQcJuZqWjJQIyibEGxZTOkULd1h)]
   <br>[Summary] Method: propensity score matching. Cause: linguistic and social interaction based measures on Reddit text, effect: suicidal attempt.
3. (2017 CWSM) **The Language of Social Support in Social Media and its Effect on Suicidal Ideation Risk.** _Munmun De Choudhury, Emre Kıcıman_. [[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5565730/pdf/nihms891351.pdf)]
   <br>[Summary] Cause: linguistic clues of Reddit comments, effect: suicidal attempt.

4. (Political Behavior, 2017) **Tweetment Effects on the Tweeted: Experimentally Reducing Racist Harassment.** _Kevin Munger_. [[pdf](https://link.springer.com/content/pdf/10.1007/s11109-016-9373-5.pdf)]   

5. (2017 ICWSM) **Estimating the Effect Of Exercising On Users’ Online Behavior.**
   _Seyed Amin Mirlohi Falavarjani, Hawre Hosseini, Zeinab Noorian, Ebrahim Bagheri_.
   [[pdf](https://ojs.aaai.org/index.php/ICWSM/article/view/14975/14825)]
   <br>[Summary] Cause: offline activities from Foursquare posts (e.g., check-ins at a gym, effect: user interests from topics of their Twitter posts. Discovery: shift in interest reduces significantly after users start exercising.

6. (2017 CSCW) **Distilling the outcomes of personal experiences: A propensity-scored analysis of social media.** _Alexandra Olteanu, Onur Varol, Emre Kiciman_. [[pdf](https://dl.acm.org/doi/pdf/10.1145/2998181.2998353?casa_token=U8iCSHz-uGUAAAAA:i9qcF0UCEH-lYKhTE9aA5RNMxFlvqfPW0tiHtUsh_lkmdV1F1O9ko9jPIl_nb8Cx5Rbtf4nn5JGq)]

7. (2018 ICWSM) **Using longitudinal social media analysis to understand the effects of early college alcohol use.**
   _Emre Kiciman, Scott Counts, Melissa Gasser_. [[pdf](http://kiciman.org/wp-content/uploads/2018/10/college_alcohol_tweets_icwsm18e.pdf)]

8. (2018 ICML) **Estimating causal effects of exercise from mood logging data.**
   _Dhanya Sridhar, Aaron Springer, Victoria Hollis, Steve Whittaker, Lise Getoor_.
   <br>[Summary] Cause: daily activities, effect: wellness markers (e.g., mood) on EmotiCal, confounder: Text of mood triggers. Confounding adjustment method: Propensity score matching

9. (2019 ICWSM) **A social media study on the effects of psychiatric medication use.** _Koustuv Saha, Benjamin Sugar, John Torous, Bruno Abrahao, Emre Kıcıman, Munmun De Choudhury_. [[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7152507/pdf/nihms-1578147.pdf)]
   <br>[Summary] Cause: psychiatric drugs, confounder: previous Twitter posts, effect: psychopathology (incl. mood, cognition, depression, anxiety, psychosis, and suicidal ideation). Method: stratified propensity score matching.

10. (Psychological Science 2019) **Increasing vegetable intake by emphasizing tasty and enjoyable attributes: A randomized controlled multisite intervention for taste-focused labeling.** _
    Bradley Turnwald, Jaclyn Bertoldo, Margaret Perry, Peggy Policastro, Maureen Timmons, Christopher Bosso, Priscilla Connors, Robert Valgenti, Lindsey Pine, Ghislaine Challamel, Christopher Gardner, Alia Crum_. [pdf](https://journals.sagepub.com/doi/pdf/10.1177/0956797619872191)
    <br>[Summary] Cause: taste-focused lables, or health-focused labels, effect: vegetable intake. Method: RCT.

11. (2021 ICWSM) **The Effect of Moderation on Online Mental Health Conversations.** _
    David Wadden, Tal August, Qisheng Li, Tim Althoff_. [pdf](https://arxiv.org/pdf/2005.09225.pdf)
    <br>[Summary] Cause: moderation in online mental health conversations, effect: psychological improvements. Method: natural experiment (comparing the data right before moderators are introduced to a platform and right after).



### 3.3 Economics

1. (2017 arXiv) **A deep causal inference approach to measuring the effects of forming group loans in online non-profit microfinance platform.**
   _Thai T Pham and Yuanyuan Shen_. [[pdf](https://arxiv.org/pdf/1706.02795.pdf)]

2. (2020 Journal of Economic Surveys) **Econometrics Meets Sentiment: An Overview of Methodology and Applications.** 
   _Andres Algaba, David Ardia, Keven Bluteau, Samuel Borms, and Kris Boudt_.
   <br>[Summary] Use sentiment as a parameter or a variable to model econometric variables.

### 3.4 Healthcare

1. **Measuring semantic similarity of clinical trial outcomes using deep pre-trained language representations.**
   _Anna Koroleva, Sanjay Kamath, Patrick Paroubek_. [[pdf](https://www.sciencedirect.com/science/article/pii/S2590177X19300575)]

### 3.5 Judicial Decision

1. (SSRN 2015) **How Judicial Identity Changes the Text of Legal Rulings**
   Michael Gill and Andrew Hall
   <br>[Summary] Cause: male or female/white of PoC judge. Method: RCT. [[pdf](https://poseidon01.ssrn.com/delivery.php?ID=952112098007006068097068030025100024031086037020053013069083081065096025112124105087055031099031027019034093127090116094014000033047002081054085089100116124096000121088020035013095127084107003013090092027067114011113122085113122096083067080012083116104&EXT=pdf&INDEX=TRUE)]

### 3.6 Marketing strategies and sales prediction

1. **Interpretable Neural Architectures for Attributing an Ad’s Performance to its Writing Style.** _Reid Pryzant, Sugato Basu, Kazoo Sone_. [[pdf](https://www.aclweb.org/anthology/W18-5415.pdf)]

2. (eCOM@SIGIR 2017) **Predicting Sales from the Language of Product Descriptions.** _Reid Pryzant, Young-Joo Chung, Dan Jurafsky_ [[pdf](http://ceur-ws.org/Vol-2311/paper_3.pdf)]
   <br>[Summary] Cause: product description (e.g., writing styles and word usages), confounder: brand loyalty and price strategies, effect: sales. Method: adversarial training.

## 4. More Resources

### 4.1 Causality Papers from Schoelkopf's Lab, MPI

#### 4.1.0 Overview

1. (2018 ICLR) **Learning Causal Mechanisms (ICLR invited talk).** [[talk](https://www.youtube.com/watch?v=4qc28RA7HLQ)]
2. (2021 Overview) **Towards Causal Representation Learning.** [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
3. (2019 Overview) **Causality for Machine Learning.** [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

#### 4.1.1 Learning Causal "Units" and Mechanisms (i.e., Causal Representation Learning)

1. (2022 ICLR) **The Role of Pretrained Representations for the OOD Generalization of RL Agents.**
   _Frederik Träuble, Andrea Dittadi, Manuel Wuthrich, Felix Widmaier, Peter Vincent Gehler, Ole Winther, Francesco Locatello, Olivier Bachem, Bernhard Schölkopf, Stefan Bauer_. [[pdf](https://openreview.net/pdf?id=8eb12UQYxrG)]

2. (2021 ICML) **On disentangled representations learned from correlated data.**
   _Frederik Träuble, Elliot Creager, Niki Kilbertus, Francesco Locatello, Andrea Dittadi, Anirudh Goyal, Bernhard Schölkopf, Stefan Bauer_. [[pdf](http://proceedings.mlr.press/v139/trauble21a/trauble21a.pdf)]

3. (2021 NeurIPS) **Self-supervised learning with data augmentations provably isolates content from style.**
   _Julius Von Kügelgen, Yash Sharma, Luigi Gresele, Wieland Brendel, Bernhard Schölkopf, Michel Besserve, Francesco Locatello_. [[pdf](https://proceedings.neurips.cc/paper/2021/file/8929c70f8d710e412d38da624b21c3c8-Paper.pdf)]

4. (2021 ICML) **Causal curiosity: Rl agents discovering self-supervised experiments for causal representation learning.**
   _Sumedh A Sontakke, Arash Mehrjou, Laurent Itti, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/pdf/2010.03110.pdf)]

5. (2021 ICLR) **Invariant Causal Representation Learning for Out-of-Distribution Generalization.**
   _Chaochao Lu, Yuhuai Wu, José Miguel Hernández-Lobato, Bernhard Schölkopf_. [[pdf](https://openreview.net/pdf?id=-e4EXDWXnSn)]

6. (2021 ICLR) **Learning explanations that are hard to vary.**
   _Giambattista Parascandolo, Alexander Neitz, Antonio Orvieto, Luigi Gresele, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/2009.00329.pdf)]

7. (2021 AAAI) **A theory of independent mechanisms for extrapolation in generative models.**
   _Michel Besserve, Rémy Sun, Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/2004.00184.pdf)]

8. (2020 NeurIPS) **Object-Centric Learning with Slot Attention.**
   _Francesco Locatello, Dirk Weissenborn, Thomas Unterthiner, Aravindh Mahendran, Georg Heigold, Jakob Uszkoreit, Alexey Dosovitskiy, Thomas Kipf_. [[pdf](https://arxiv.org/pdf/2006.15055.pdf)]

9. (2020 ICML) **Weakly-supervised disentanglement without compromises.**
   _Francesco Locatello, Ben Poole, Gunnar Rätsch, Bernhard Schölkopf, Olivier Bachem, Michael Tschannen_. [[pdf](http://proceedings.mlr.press/v119/locatello20a/locatello20a.pdf)]

10. (2019 ICML, Best Paper) **Challenging common assumptions in the unsupervised learning of disentangled representations.**
    _Francesco Locatello, Stefan Bauer, Mario Lucic, Gunnar Rätsch, Sylvain Gelly, Bernhard Schölkopf, Olivier Bachem_.
    [[pdf](http://proceedings.mlr.press/v97/locatello19a/locatello19a.pdf)]

11. (2019 arXiv) **Disentangling factors of variation using few labels.**
    _Francesco Locatello, Michael Tschannen, Stefan Bauer, Gunnar Rätsch, Bernhard Schölkopf, Olivier Bachem_. [[pdf](https://arxiv.org/pdf/1905.01258.pdf)]

12. (2019 arXiv) **Recurrent independent mechanisms.**
    _Anirudh Goyal, Alex Lamb, Jordan Hoffmann, Shagun Sodhani, Sergey Levine, Yoshua Bengio, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1909.10893.pdf)]

13. (2018 ICML) **Learning independent causal mechanisms.**
    _Giambattista Parascandolo, Niki Kilbertus, Mateo Rojas-Carulla, Bernhard Schölkopf_. [[pdf](http://proceedings.mlr.press/v80/parascandolo18a/parascandolo18a.pdf)]

14. (2018 NeurIPS) **Adaptive skip intervals: Temporal abstraction for recurrent dynamical models.**
    _Alexander Neitz, Giambattista Parascandolo, Stefan Bauer, Bernhard Schölkopf_. [[pdf](https://proceedings.neurips.cc/paper/2018/file/0f0ee3310223fe38a989b2c818709393-Paper.pdf)]

15. (2018 arXiv) **Counterfactuals uncover the modular structure of deep generative models.**
    _Michel Besserve, Arash Mehrjou, Rémy Sun, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1812.03253.pdf)]

16. (2017 CVPR) **Discovering causal signals in images.**
    _David Lopez-Paz, Robert Nishihara, Soumith Chintala, Bernhard Scholkopf, Léon Bottou_.
    [[pdf](https://openaccess.thecvf.com/content_cvpr_2017/papers/Lopez-Paz_Discovering_Causal_Signals_CVPR_2017_paper.pdf)]

17. (2017 NeurIPS) **Avoiding Discrimination through Causal Reasoning.**
    _Niki Kilbertus, Mateo Rojas-Carulla, Giambattista Parascandolo, Moritz Hardt, Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://proceedings.neurips.cc/paper/2017/file/f5f8590cd58a54e94377e6ae2eded4d9-Paper.pdf)]

#### 4.1.2 Robustness and Invariance (incl. Semi-Supervised Learning, Covariate Shift, Transfer Learning)

1. (2021 ICLR) **Source-free adaptation to measurement shift via bottom-up feature restoration.**
   _Cian Eastwood, Ian Mason, Christopher KI Williams, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/abs/2107.05446.pdf)]

2. (2016 ICML) **Domain adaptation with conditional transferable components.**
   _Mingming Gong, Kun Zhang, Tongliang Liu, Dacheng Tao, Clark Glymour, Bernhard Schölkopf_.
   [[pdf](http://proceedings.mlr.press/v48/gong16.pdf)]

3. (2021 EMNLP oral) **Causal Direction of Data Collection Matters: Implications of Causal and Anticausal Learning for NLP.**
   _Zhijing Jin, Julius von Kügelgen, Jingwei Ni, Tejas Vaidhya, Ayush Kaushal, Mrinmaya Sachan, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/pdf/2110.03618.pdf)]

4. (2020 UAI) **Semi-supervised learning, causality, and the conditional cluster assumption.**
   _Julius Kügelgen, Alexander Mey, Marco Loog, Bernhard Schölkopf_.
   [[pdf](http://proceedings.mlr.press/v124/kugelgen20a/kugelgen20a.pdf)]

5. (2018 JMLR) **Invariant models for causal transfer learning.**
   _Mateo Rojas-Carulla, Bernhard Schölkopf, Richard Turner, Jonas Peters_.
   [[pdf](https://www.jmlr.org/papers/volume19/16-432/16-432.pdf)]

6. (2018 NeurIPS workshop) **Generalization in anti-causal learning.**
   _Niki Kilbertus, Giambattista Parascandolo, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/pdf/1812.00524.pdf)]

7. (2012 ICML) **On Causal and Anticausal Learning.** 
   _Bernhard Schölkopf, Dominik Janzing, Jonas Peters, Eleni Sgouritsa, Kun Zhang, Joris Mooij_.
   [[pdf](https://icml.cc/2012/papers/625.pdf)]


#### 4.1.3 Causal Discovery

1. (2021 NeurIPS) **DiBS: Differentiable Bayesian Structure Learning.**
   _Lars Lorch, Jonas Rothfuss, Bernhard Schölkopf, Andreas Krause_.
   [[pdf](https://arxiv.org/pdf/2105.11839.pdf)]

2. (2021 ICML) **Necessary and sufficient conditions for causal feature selection in time series with latent common causes.**
   _Atalanti A Mastakouri, Bernhard Schölkopf, Dominik Janzing_.
   [[pdf](http://proceedings.mlr.press/v139/mastakouri21a/mastakouri21a.pdf)]

3. (2020 JMLR) **Causal Discovery from Heterogeneous/Nonstationary Data..**
   _Biwei Huang, Kun Zhang, Jiji Zhang, Joseph D Ramsey, Ruben Sanchez-Romero, Clark Glymour, Bernhard Schölkopf_.
   [[pdf](https://www.jmlr.org/papers/volume21/19-232/19-232.pdf)]

4. (2019 Nature communications) **Inferring causation from time series in Earth system sciences.**
   _Jakob Runge, Sebastian Bathiany, Erik Bollt, Gustau Camps-Valls, Dim Coumou, Ethan Deyle, Clark Glymour, Marlene Kretschmer, Miguel D Mahecha, Jordi Muñoz-Marí, Egbert H van Nes, Jonas Peters, Rick Quax, Markus Reichstein, Marten Scheffer, Bernhard Schölkopf, Peter Spirtes, George Sugihara, Jie Sun, Kun Zhang, Jakob Zscheischler_.
   [[pdf](https://www.nature.com/articles/s41467-019-10105-3.pdf)]

5. (2017 UAI) **Causal discovery from temporally aggregated time series.**
   _Mingming Gong, Kun Zhang, Bernhard Schölkopf, Clark Glymour, Dacheng Tao_.
   [[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5995575/pdf/nihms904883.pdf)]

6. (2016 JMLR) **Distinguishing cause from effect using observational data: methods and benchmarks.**
   _Joris M Mooij, Jonas Peters, Dominik Janzing, Jakob Zscheischler, Bernhard Schölkopf_.
   [[pdf](https://jmlr.org/papers/volume17/14-518/14-518.pdf)]

7. (2016 UAI) **On the Identifiability and Estimation of Functional Causal Models in the Presence of Outcome-Dependent Selection..**
   _Kun Zhang, Jiji Zhang, Biwei Huang, Bernhard Schölkopf, Clark Glymour_.
   [[pdf](http://auai.org/uai2016/proceedings/papers/305.pdf)]

8. (2016 PNAS) **Methods for causal inference from gene perturbation experiments and validation.**
   _Nicolai Meinshausen, Alain Hauser, Joris M. Mooij, Jonas Peters, Philip Versteeg, and Peter Bühlmann_.
   [[pdf](https://www.pnas.org/content/pnas/113/27/7361.full.pdf)]

9. (2016 ICML) **The arrow of time in multivariate time series.**
   _Stefan Bauer, Bernhard Schölkopf, Jonas Peters_.
   [[pdf](http://proceedings.mlr.press/v48/bauer16.pdf)]

10. (2014 UAI) **Inferring latent structures via information inequalities.**
    _Rafael Chaves, Lukas Luft, Thiago O Maciel, David Gross, Dominik Janzing, Bernhard Schölkopf_.
    [[pdf](https://arxiv.org/pdf/1407.2256.pdf)]

11. (2015 Journal of the Royal Statistical Society) **Causal inference using invariant prediction: identification and confidence intervals.**
    _Jonas Peters, Peter Bühlmann, Nicolai Meinshausen_.
    [[pdf](https://arxiv.org/pdf/1501.01332.pdf)]

12. (2008IEEE) **Causal inference using the algorithmic Markov condition.** _Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/0804.3678.pdf)]

#### 4.1.4 Causal Effect Estimation

1. (2016 PASA) **A causal, data-driven approach to modeling the Kepler d.**ata
   _Dun Wang, David W Hogg, Daniel Foreman-Mackey, Bernhard Schölkopf_.
   [[pdf](https://arxiv.org/pdf/1508.01853.pdf)]

2. (2016 PNAS) **Modeling confounding by half-sibling regression.**
   _Bernhard Schölkopf, David W Hogg, Dun Wang, Daniel Foreman-Mackey, Dominik Janzing, Carl-Johann Simon-Gabriel, Jonas Peters_.
   [[pdf](https://www.pnas.org/content/pnas/113/27/7391.full.pdf)]

3. (2021 ICML) **Conditional distributional treatment effect with kernel conditional mean embeddings and U-statistic regression
   Junhyung Park, Uri Shalit, Bernhard Schölkopf, Krikamol Muandet
   http://proceedings.mlr.press/v139/park21c/park21c.pdf

4. (2020 NeurIPS) **Dual Instrumental Variable Regression.**
   _Krikamol Muandet, Arash Mehrjou, Si Kai Lee, Anant Raj_.
   [[pdf](https://proceedings.neurips.cc/paper/2020/file/1c383cd30b7c298ab50293adfecb7b18-Paper.pdf)]

5. (2021 ICML Spotlight) **Proximal Causal Learning with Kernels: Two-Stage Estimation and Moment Restriction.**
   _Afsaneh Mastouri, Yuchen Zhu, Limor Gultchin, Anna Korba, Ricardo Silva, Matt J. Kusner, Arthur Gretton, Krikamol Muandet_.
   [[pdf](https://icml.cc/virtual/2021/spotlight/9926)]

6. (2021 JMLR) **Counterfactual Mean Embeddings.**
   _Krikamol Muandet, Motonobu Kanagawa, Sorawit Saengkyongam, Sanparith Marukatat_.
   [[pdf](https://jmlr.csail.mit.edu/papers/volume22/20-185/20-185.pdf)]

#### 4.1.5 Foundational work (theory, ICA, etc.)

Topics: thermodynamic arrow of time, modeling hierarchy (ODEs, macro variables, temporal abstractions), links to ICA.

1. (2021 NeurIPS) Independent mechanism analysis, a new concept?
   _Luigi Gresele, Julius Von Kügelgen, Vincent Stimper, Bernhard Schölkopf, Michel Besserve_. [[pdf]()]

2. (2020 UAI) The incomplete rosetta stone problem: Identifiability results for multi-view nonlinear ICA
   _Luigi Gresele, Paul K Rubenstein, Arash Mehrjou, Francesco Locatello, Bernhard Schölkopf_. [[pdf]()]

3. (2017 arXiv) Causal consistency of structural equation models
   _Paul K Rubenstein, Sebastian Weichwald, Stephan Bongers, Joris M Mooij, Dominik Janzing, Moritz Grosse-Wentrup, Bernhard Schölkopf_. [[pdf]()]

4. (2016 arXiv) From deterministic ODEs to dynamic structural causal models
   _Paul K Rubenstein, Stephan Bongers, Bernhard Schölkopf, Joris M Mooij_. [[pdf]()]

5. (2016 New Journal of Physics) Algorithmic independence of initial condition and dynamical law in thermodynamics and causal inference
   _Dominik Janzing, Rafael Chaves, Bernhard Schölkopf_. [[pdf]()]

6. (2017 Book by MIT Press) Elements of causal inference: foundations and learning algorithms
   _Jonas Peters, Dominik Janzing, Bernhard Schölkopf_. [[pdf]()]



### 4.2 Causality Papers from Bengio's Lab, MILA

1. (Summary) **Yoshua Bengio's Summary Talk.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]

#### Motivational Position Papers

1. (2020 Position Paper, arXiv) **Inductive Biases for Deep Learning of Higher-Level Cognition.** _Anirudh Goyal, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/2011.15091.pdf)]
   <br>[Summary] We need inductive bias for real understanding and generalization => such as decomposing world knowledge into right causal pieces

2. (Motivational, position paper, arXiv 2017) **The Consciousness Prior.** _Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1709.08568.pdf)]

#### Applying Causality Knowledge for RL Interaction Design

1. (2020 arXiv) **Visual Concept Reasoning Networks.** _Taesup Kim, Sungwoong Kim, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/2008.11783.pdf)]
   <br> [Summary] Modularized visual concept reasoning by split-transform-attend-interact-modulate-merge modules

2. (RLDM 2017) **Independently Controllable Features.**
   _Emmanuel Bengio, Valentin Thomas, Joelle Pineau, Doina Precup, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1703.07718.pdf)]

3. (2017 arXiv) **Independently Controllable Factors.** _Valentin Thomas, Jules Pondard, Emmanuel Bengio, Marc Sarfati, Philippe Beaudoin, Marie-Jean Meurs, Joelle Pineau, Doina Precup, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1708.01289.pdf)]
   <br> [Summary] The representations of (1) abstract action, and (2) abstract variables, should be learned together, because the action is about controlling variables. A way to disentangle abstractions from images & videos when we have an agent which can interact with the environment. The right abstractions have the right factors. I.e., there exists a policy and a learnable feature for each such aspect of the environment.

#### Applying causality to model design

Quote from [a blog](https://medium.com/@wcarvalho92/success-vs-failure-generalization-vs-stereotyping-40de0713ab5d): "Causality is the idea that you can model something with an abstraction of the real-world process that generated it. When you use compositionality and learning-to-learn to break down objects into their parts and relations, modeling the object as a creation of these parts can be seen as modeling them in a causal way."

1. **Recurrent Independent Mechanisms.** _Anirudh Goyal, Alex Lamb, Jordan Hoffmann, Shagun Sodhani, Sergey Levine, Yoshua Bengio, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1909.10893.pdf)]
   <br>[Summary] Divides the overall model into k small subsystems (or modules), Each small module is recurrent

2. **Object Files and Schemata: Factorizing Declarative and Procedural Knowledge in Dynamical Systems.** _Anirudh Goyal, Alex Lamb, Phanideep Gampa, Philippe Beaudoin, Sergey Levine, Charles Blundell, Yoshua Bengio, Michael Mozer_. [[pdf](https://arxiv.org/pdf/2006.16225.pdf)]
   <br>[Summary] Modularity when designing the model

#### Causal induction from interventional data

[Background] Changes in distribution is caused by intervention on few causes/mechanisms (in extension of Independent Mechanisms by [[Schoelkopf+ 2012](https://icml.cc/2012/papers/625.pdf)])

1. (2019 arXiv) **Learning Neural Causal Models from unknown Interventions.** _Nan Rosemary Ke, Olexa Bilaniuk, Anirudh Goyal, Stefan Bauer, Hugo Larochelle, Bernhard Schölkopf, Michael C. Mozer, Chris Pal, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1910.01075.pdf)]
   <br>[Summary] Aim: make use of the combination of observational and interventional data, Method: continuous optimization and neural networks, Extended setting: when the identity of the intervened upon variable is unknown

2. (NeurIPS 2020 Spotlight) **Differentiable Causal Discovery from Interventional Data.** _Philippe Brouillard, Sébastien Lachapelle, Alexandre Lacoste, Simon Lacoste-Julien, Alexandre Drouin_. [[pdf](https://arxiv.org/pdf/2007.01754.pdf)] [[review](https://papers.nips.cc/paper/2020/file/f8b7aa3a0d349d9562b424160ad18612-Review.html)]
   <br>[Summary] Closely related to [Ke+ 2019](https://arxiv.org/pdf/1910.01075.pdf), Method: continuous-constrained framework + normalizing flows

3. (2019 ICLR) **Learning Dynamics Model in Reinforcement Learning by Incorporating the Long Term Future.** _Nan Rosemary Ke, Amanpreet Singh, Ahmed Touati, Anirudh Goyal, Yoshua Bengio, Devi Parikh, Dhruv Batra_.
   [[pdf](https://arxiv.org/pdf/1903.01599.pdf)]

4. (2020 ICLR) **A Meta-Transfer Objective for Learning to Disentangle Causal Mechanisms.** _Yoshua Bengio, Tristan Deleu, Nasim Rahaman, Rosemary Ke, Sébastien Lachapelle, Olexa Bilaniuk, Anirudh Goyal, Christopher Pal_. [[pdf](https://arxiv.org/pdf/1901.10912.pdf)]

#### Grounded AI

1. (2021 ICLR) **CausalWorld: A Robotic Manipulation Benchmark for Causal Structure and Transfer Learning.** _Ossama Ahmed, Frederik Träuble, Anirudh Goyal, Alexander Neitz, Yoshua Bengio, Bernhard Schölkopf, Manuel Wüthrich, Stefan Bauer_. [[pdf](https://arxiv.org/pdf/2010.04296.pdf)]
   <br>[Summary] An RL dataset to model do-interventions and discover causality

2. (2019 ICLR) **BabyAI: A Platform to Study the Sample Efficiency of Grounded Language Learning.** _Maxime Chevalier-Boisvert, Dzmitry Bahdanau, Salem Lahlou, Lucas Willems, Chitwan Saharia, Thien Huu Nguyen, Yoshua Bengio_. [[pdf](https://arxiv.org/pdf/1810.08272.pdf)]
   <br>[Summary] (not yet causal) synthetic language acquisition, A simulation platform, to do language instructions with a simulated human in the loop, Allows curriculum learning for 19 levels



### 4.3 Other Causality Papers (Potentially Applicable to NLP)

#### Repos

1. [[Awesome-Causality-in-CV](https://github.com/rguo12/awesome-causality-algorithms)]

#### Invariance-Based Causal Discovery (for Robustness)

1. (2016, Journal of the Royal Statistical Society) **Causal inference using invariant prediction: identification and confidence intervals.**
   _Jonas Peters, Peter Bühlmann, Nicolai Meinshausen_. [[pdf](https://arxiv.org/pdf/1501.01332.pdf)]
2. (2018 Journal of Causal Inference) **Invariant Causal Prediction for Nonlinear Models.** _Christina Heinze-Deml*, Jonas Peters, and Nicolai Meinshausen_. [[pdf](https://www.degruyter.com/document/doi/10.1515/jci-2017-0016/html)]
3. (2019) **Invariant Risk Minimization.**
   _Martin Arjovsky, Léon Bottou, Ishaan Gulrajani, David Lopez-Paz_. [[pdf](https://arxiv.org/pdf/1907.02893.pdf)]
4. (2020) **Nonlinear Invariant Risk Minimization: A Causal Approach.**
   _Chaochao Lu, Yuhuai Wu, Jośe Miguel Hernández-Lobato, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/2102.12353.pdf)]

#### Interventional Robustness

1. (2018 IEEE Data Science Workshop) **Causality from a Distributional Robustness Point of View.** _Nicolai Meinshausen_. [[pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8439889)]

2. (2018) **Anchor regression: heterogeneous data meet causality.**
   _Dominik Rothenhäusler, Nicolai Meinshausen, Peter Bühlmann and Jonas Peters_. [[pdf](https://arxiv.org/pdf/1801.06229.pdf)]

#### Causality from Cognitive Science Point of View

1. (2002 NIPS) **Theory-Based Causal Inference.**
   _Joshua B. Tenenbaum & Thomas L. Griffiths_. [[pdf](https://papers.nips.cc/paper/2002/file/e77dbaf6759253c7c6d0efc5690369c7-Paper.pdf)]
   <br>[Summary] Modeling human's learning of causality as Bayesian computations over a hypothesis space of causal graphical model.

#### Others

1. (PSB 2020 Oral) **Robustly Extracting Medical Knowledge from EHRs: A Case Study of Learning a Health Knowledge Graph.** _Irene Y. Chen, Monica Agrawal, Steven Horng, David Sontag_. [[pdf](https://arxiv.org/pdf/1910.01116.pdf)]

2. (2021 AAAI; AI Safety, RL with causality) **Agent Incentives: A Causal Perspective.** _Tom Everitt, Ryan Carey, Eric Langlois, Pedro A Ortega, Shane Legg_.
   [[pdf](https://arxiv.org/pdf/2102.01685.pdf)]

3. (2019 IJCAI AI Safety Workshop) **Modeling AGI Safety Frameworks with Causal Influence Diagrams.** _Tom Everitt, Ramana Kumar, Victoria Krakovna, Shane Legg_ ([Causal Incentives Working Group](https://causalincentives.com/)).
   [[pdf](https://arxiv.org/pdf/1906.08663.pdf)]

4. (2018 IEEE workshop; robustness under domain shifts) **Causality from a Distributional Robustness Point of View.** _Nicolai Meinshausen_. [[pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8439889&casa_token=TqNXF6HAKDIAAAAA:U2ti2LifcIXZ4tyElAFyahiSDEAvXWxGbNLbU0NVxcvedqWKFUMuMOL8faO_yRX3mPqW_lky&tag=1)] 

#### Some tools that might be useful for disentanglement

1. (2009) **Tensor Decompositions and Applications.** _Tamara Kolda, Brett Bader_. [[pdf](https://www.kolda.net/publication/TensorReview.pdf)]

### 4.4 Books (for Systematic Learning)

1. (For ML Audience) **Elements of Causal Inference.** _Jonas Peters, Dominik Janzing and Bernhard Schölkopf_. [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]
2. (Quick Primer by Judea Pearl) **Causal Inference in Statistics: A Primer.** _Judea Pearl_. [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
3. (Focus on SCM) **Causality: Models, Reasoning, and Inference.** _Judea Pearl_. [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
4. (For statistics people on causal inference) **Causation, Prediction and Search.** _Peter Spirtes_. [[Book, 2001](https://mitpress.mit.edu/books/causation-prediction-and-search-second-edition)]
5. More book recommendations: See Brady Neal's [blog](https://www.bradyneal.com/which-causal-inference-book), and this [pointer](https://sites.google.com/view/causality-reading-group/introduction) to causality books for beginner/intermediate/advanced.
6. **Causal Inference for The Brave and True.** [[website](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)]
7. A long paper&book list including multiple categories of causality papers: [[spreadsheet](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=0)]

### 4.5 Online Courses

1. **Graphical Models and Causality.** _[Isabelle Guyon](http://www.clopinet.com/isabelle) (ETH)_. [[course website](http://clopinet.com/isabelle/Projects/ETH/Causality_Reading_Group.html)]
2. **Applied Causality (Spring 2019).** _David Blei (Columbia University)_. [[course reading list](http://www.cs.columbia.edu/~blei/seminar/2019-applied-causality/index.html)]
3. **A Week Long Course on Causal Modeling and Discovery.** (Center for Causal Discovery, 2016) [[videos](https://www.ccd.pitt.edu/video-tutorials/)]
4. (Reading group) **Causality Reading Club@Amsterdam ML Lab.** _Prof. Joris Mooij_. [[past readings](https://amlab.science.uva.nl/meetings/causality-reading-club/)]

### 4.6 People Directory

(Credits to [Causal Resources](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=1999914756).)

- **Judea Pearl** (UCLA), US.
- **Bernhard Schölkopf** (MPI Tübingen), Tübingen, Germany. [[group intro](http://webdav.tuebingen.mpg.de/causality/)]
- **Dominik Janzing** (Amazon Tübingen; former: MPI Tübingen), Tübingen, Germany.
- **Joris Mooij** (University of Amsterdam; former: MPI Tübingen), Netherlands. [[home page](https://staff.fnwi.uva.nl/j.m.mooij/)]
- **Jonas Peters** (Copenhagen University; former: MPI Tübingen), Denmark. [[home page](http://web.math.ku.dk/~peters/)]
- **Peter Bühlmann** (ETH), Switzerland.
- **Marloes Maathuis** (ETH), Switzerland. [[video](https://www.youtube.com/watch?v=Q_2cgCeAjpo)]
- **Nicolai Meinshausen** (ETH), Switzerland. E.g., Anchor regression.
- **Negar Kiyavash** (EPFL), Switzerland. E.g., causal structure learning.
- **Kun Zhang** (CMU; former: MPI Tübingen), US. 
- **Peter Spirtes** (CMU Philosophy), US.
- **Cosma Shalizi** (CMU), US.
- **David Sontag** (MIT), US.
- **Caroline Uhler** (MIT), US.
- **Victor Chernozhukov** (MIT), US.
- **Elias Bareinboim** (Columbia), US. [[home page](https://causalai.net/)]
- **Andrew Gelman** (Columbia; former: UCLA with Judea Pearl), US. [[video](https://www.youtube.com/watch?time_continue=25&v=cuE9eHSbjNI&app=desktop)]
- **Ilya Shpitser** (JHU; former: UCLA with Judea Pearl), US. [[home page](https://www.cs.jhu.edu/faculty/ilya-shpitser-3/)]
- **Kosuke Imai** (Harvard; former: Princeton), US. 
- **James Robins** (Harvard), US.
- **Ferederick Eberhardt** (Caltech; former: CMU), US.
- **David Heckerman** (Amazon), US.
- **Leon Bottou** (Facebook AI), US.
- **Thomas Richardson** (UW), US.
- **Stephan Hartmann** (LMU), Munich, Germany.
- **Cheng Soon Ong** (Data61; former: MPI Tübingen), Canberra, Australia.
- You can also track the [organizers](https://www.cclear.cc/OrganizingCommittee), [area chairs](https://www.cclear.cc/AreaChairs), and [advisory board](https://www.cclear.cc/AdvisoryBoard) of the CLeaR conference, as well as attendees of causal inference seminars/workshops such as [2021 Frontiers of Causal Inference in Data Science](https://www.cceb.med.upenn.edu/cci/frontiers-causal-inference-data-science-perspectives-leaders-tech-and-academia-may-28-2021).

### 4.7 Workshops

Please see this [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=416373885) for a list of causality workshops (2016 - now). 

### 4.8 Others

- Job postings for causality researchers: [[website](https://sites.google.com/view/ocis/opportunities-and-resources)]
- [*Causality notes*](https://docs.google.com/document/d/1nsN7KMAWhxENpSIxzBwcPaflPKra-1gr9TdPqXjLmb8/edit) by Tailin Wu

## Contributions

All types of contributions to this paper list is welcome. Feel free to open a Pull Request.

Contact: [Zhijing Jin](zhijing-jin.com), PhD of Bernhard Schoelkopf at Max Planck Institute for Intelligent Systems, working on NLP & Causality.

## How to Cite This Repo

```bibtex
@misc{causality2021jin,
  author = {Zhijing Jin},
  title = {Causality for NLP Reading List},
  year = {2021},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/zhijing-jin/Causality4NLP_Papers}}
}
```
