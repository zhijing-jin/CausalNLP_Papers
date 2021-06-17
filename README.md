# Causality for NLP Reading List

This repository lists papers on causality for natural language processing (NLP). 

**Contributor:** [Zhijing Jin](http://zhijing-jin.com).
Welcome to be a collaborator, -- you can make an issue/pull request, and I can add you :).

### Contents (Actively Updating)

- [1. Causality Basics](#1-causality-basics)
  - [1.1 Talks/Tutorial/etc](#11-Talkstutorialetc)
  - [1.2 Overview Papers](#12-overview-papers)
  - [1.3 Toolboxes](#13-toolboxes)
- [2. Causality Applied to General NLP](#2-causality-applied-to-general-nlp)
  - [2.1 Causal Relation Extraction](#21-causal-relation-extraction) 
- [3. Causality for Various Applications](#3-causality-for-various-applications)
  - [3.1 Persuasion](#31-persuation)
  - [3.2 Psychology and Behavior](#32-psychology-and-behavior)
  - [3.3 Economics](#33-economics)
  - [3.4 Healthcare](#34-healthcare)
  - [3.4 Judicial Decision](#35-judicial-decision)
  - [3.5 Marketing strategies and sales prediction](#36-marketing-strategies-and-sales-prediction)
- [4. Addressing "Confounders" in NLP](#4-addressing-confounders-in-nlp)
  - [4.1 Causality tools that can be applied to deconfound](#41-causality-tools-that-can-be-applied-to-deconfound)
- [5. More Resources](#5-more-resources)
  - [5.1 Causality Papers from Schoelkopf's Lab, MPI](#51-causality-papers-from-schoelkopfs-lab-mpi)
  - [5.2 Causality Papers from Bengio's Lab, MILA](#52-causality-papers-from-bengios-lab-mila)
    - [Motivational Position Papers](#motivational-position-papers)
    - [Applying Causality Knowledge for RL Interaction Design](#applying-causality-knowledge-for-rl-interaction-design)
    - [Applying causality to model design](#applying-causality-to-model-design)
    - [Causal induction from interventional data](#causal-induction-from-interventional-data)
    - [Grounded AI](#grounded-AI)
  - [5.3 Other Causality Papers (Potentially Applicable to NLP)](#53-other-causality-papers-potentially-applicable-to-nlp)
  - [5.4 Books (for Systematic Learning)](#54-books-for-systematic-learning)
  - [5.5 Online Courses](#55-online-courses)
  - [5.6 People Directory](#56-people-directory)
  - [5.7 Workshops](#57-workshops)
  - [5.8 Others](#58-others)
- [Contributions](#contributions)
- [How to Cite This Repo](#How-to-Cite-This-Repo)

## 1. Causality Basics

### 1.1 Talks/Tutorial/etc

Motivational reading:
1. (2002 AI Magazine) **Reasoning with Cause and Effect.** _Judea Pearl_. [[pdf](https://ftp.cs.ucla.edu/pub/stat_ser/r265-ai-mag.pdf)]
1. (Blog) **ML beyond Curve Fitting: An Intro to Causal Inference and do-Calculus.** _Ferenc Huszár_. [[blog](https://www.inference.vc/untitled/)]


Talks and tutorials:
1. (Videos course to introduce a series of concepts) **Introduction to Causal Inference** [[Video](https://www.youtube.com/c/BradyNealCausalInference)]
1. (Vivid, beginner-friendly) **Yoshua Bengio's Primer on the Future of Causality&NLP.** [[Video@ELLIS NLP Workshop](https://www.youtube.com/watch?v=u3IR6sSwwjg&list=PL5_PEnlMYYahS7HZ3rt8QTkeKlxuYhomD&index=4&ab_channel=ELLISNLP)]

1. (Global, weekly reading group) Online Causal Inference Seminar. Organized by Stanford, ETH, etc. [[speakers](https://sites.google.com/view/ocis/home#h.13whjoi1jght)] [[past recordings](https://sites.google.com/view/ocis/past-talks-and-recordings)] 

   Every Tuesdays at 8:30 am PT (11:30 am ET / 4:30 pm London / 5:30 pm Berlin).

Blogs:
1. **Causal Analysis in Theory and Practice.** Judea Pearl's [[blog](http://causality.cs.ucla.edu/blog/)]

### 1.2 Overview Papers

1. (2021 Overview, Schoelkopf+) **Towards Causal Representation Learning.** [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
1. (2019 Overview, Schoelkopf) **Causality for Machine Learning.** [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

### 1.3 Toolboxes

1. (2020) **DoWhy: An End-to-End Library for Causal Inference.** 
_Amit Sharma, Emre Kiciman_. [[GitHub](https://github.com/microsoft/dowhy)] [[pdf](https://arxiv.org/pdf/2011.04216.pdf)]
2. (2019) **Causal Discovery Toolbox in Python.** [[GitHub](https://github.com/FenTechSolutions/CausalDiscoveryToolbox)] [[pdf](https://arxiv.org/pdf/1903.02278.pdf)] 

## 2. Causality Applied to General NLP

1. **Discovery of Treatments from Text Corpora.** _Christian Fong, Justin Grimmer_. [[pdf](https://www.aclweb.org/anthology/P16-1151.pdf)]
1. **How to Make Causal Inferences Using Texts.** _Naoki Egami, Christian J. Fong, Justin Grimmer, Margaret E. Roberts, Brandon M. Stewart_. [[pdf](https://arxiv.org/pdf/1802.02163.pdf)]

3. (NeurIPS 2020 Spotlight) **Causal Mediation Analysis for Interpreting Neural NLP:
   The Case of Gender Bias.** _Jesse Vig, Sebastian Gehrmann, Yonatan Belinkov, Sharon Qian, Daniel Nevo, Simas Sakenis, Jason Huang, Yaron Singer, Stuart Shieber_. [[pdf](https://arxiv.org/pdf/2004.12265.pdf)]
   <br>[Summary] Cause: input text, mediator: some neurons, effect: output prediction

1. (ACL 2020) **Text and Causal Inference: A Review of Using Text to Remove Confounding from Causal Estimates.** _Katherine A. Keith, David Jensen, and Brendan O'Connor_. [[pdf](https://www.aclweb.org/anthology/2020.acl-main.474.pdf)]

1. (UAI 2020) **Adapting Text Embeddings for Causal Inference.** _Victor Veitch, Dhanya Sridhar, David M. Blei_. [[pdf](https://arxiv.org/pdf/1905.12741.pdf)]

1. (CSCW 2020) **Quantifying the Causal Effects of Conversational Tendencies.** _Justine Zhang, Sendhil Mullainathan, Cristian Danescu-Niculescu-Mizil_. [[pdf](https://arxiv.org/pdf/2009.03897.pdf)]

1. (arXiv 2020) **Causal Effects of Linguistic Properties.** _Reid Pryzant, Dallas Card, Dan Jurafsky, Victor Veitch, Dhanya Sridhar_. [[pdf](https://arxiv.org/pdf/2010.12919.pdf)] [[blog](http://ai.stanford.edu/blog/text-causal-inference/) and [github](https://github.com/rpryzant/causal_selection)]
   <br>[Summary] Cause: binary writer intent, confounder: other linguistic habits of the writer, mediator: text by the writer, effect: reader's response time
   
1. (arXiv 2020) **Decoupling entrainment from consistency using deep neural networks.** [[pdf](https://arxiv.org/pdf/2011.01860.pdf)]
   <br>[Note] Entrainment = speakers adapting to conversation partners so as to become more similar
   
1. (arXiv 2020) **CausaLM: Causal Model Explanation Through Counterfactual Language Models.** _Amir Feder, Nadav Oved, Uri Shalit and Roi Reichart_. [[pdf](https://arxiv.org/pdf/2005.13407.pdf)]

1. (arXiv 2021) **Generating Synthetic Text Data to Evaluate Causal Inference Methods.** _Zach Wood-Doughty, Ilya Shpitser, Mark Dredze_. [[pdf](https://arxiv.org/pdf/2102.05638.pdf)]

1. (ICLR 2020) **Learning the Difference that Makes a Difference with Counterfactually-Augmented Data.**
_Divyansh Kaushik, Eduard Hovy, Zachary C. Lipton_. [[pdf](https://arxiv.org/pdf/1909.12434.pdf)]

1. (ICLR 2021 Workshop) **A Causal Lens for Controllable Text Generation.** _Zhiting Hu, Li Erran Li_.
[[pdf](https://sites.google.com/connect.hku.hk/robustml-2021/accepted-papers/paper-089)]

1. **Generating Synthetic Text Data to Evaluate Causal Inference Methods.**
_Zach Wood-Doughty, Ilya Shpitser, Mark Dredze_.
[[pdf](https://arxiv.org/pdf/2102.05638.pdf)]

1. (2018 EMNLP) **Challenges of Using Text Classifiers for Causal Inference.**
_Zach Wood-Doughty, Ilya Shpitser, Mark Dredze_. [[pdf](https://arxiv.org/pdf/1810.00956.pdf)]

1. (2018 Political Analysis) **Matching with text data: An experimental evaluation of methods for matching documents and of measuring match quality.**
_Reagan Mozer, Luke Miratrix, Aaron Russell Kaufman, L Jason Anastasopoulos_. [[pdf](https://arxiv.org/pdf/1801.00644.pdf)]


1. (2017 EMNLP) **Detecting and Explaining Causes From Text For a Time Series Event.**
_Dongyeop Kang, Varun Gangal, Ang Lu, Zheng Chen, Eduard Hovy_.
[[pdf](https://arxiv.org/pdf/1707.08852.pdf)]
   <br>[Summary] Finding causes for the stock price time series.

1. (2016 JMLR) **Learning representations for counterfactual inference.**
_Fredrik Johansson, Uri Shalit, David Sontag_. [[pdf](http://proceedings.mlr.press/v48/johansson16.pdf)]


1. (2001 PAKDD) **Semantic Expectation-Based Causation Knowledge Extraction: A Study on Hong Kong Stock Movement Analysis.**
_Boon-Toh Low, Ki Chan, Lei-Lei Choi, Man-Yee Chin, Sin-Ling Lay_.
[[link](https://link.springer.com/chapter/10.1007/3-540-45357-1_15)]

### 2.1 Causal Relation Extraction
#### Surveys and Reviews
1. **CREST: A Causal Relation Schema for Text (A repo containing datasets for causal/counterfactual relation extraction)** _Pedram Hosseini_. [[GitHub](https://github.com/phosseini/CREST)]
   <br>[Summary] CausalRE datasets: SemEval 2007 Task 4 (114 causal sentences), SemEval 2021 Task 8 (1,331), EventCausality (485), Causal-TimeBank (318), EventStoryLine v1.5 (2,608), CaTeRS (308), BECauSE v2.1 (554), Choice of Plausible Alternatives (COPA) (1,000), The Penn Discourse Treebank (PDTB) 3.0 (7,991).

1. (2020 COLING) **A Review of Dataset and Labeling Methods for Causality Extraction.** _Jinghang Xu, Wanli Zuo, Shining Liang, Xianglin Zuo_. [[pdf](https://www.aclweb.org/anthology/2020.coling-main.133.pdf)]
   <br>[Summary] Very reader-friendly survey, including ideas such as Causal connectives (verb: cause, result; conjunction: because, so; preposition: for, because of; adverb: consequently; Verb Phrase: result in, lead to; Prepositional phrase: as a result of; Clause: that's why, so that); Causal concepts (sufficient, necessary, temporal); etc.
   
1. (2016 arXiv) **Automatic Extraction of Causal Relations from Natural Language Texts: A Comprehensive Survey.** _Nabiha Asghar_. [[GitHub](https://arxiv.org/pdf/1605.07895.pdf)]
   <br>[Summary] Automatic discovery of linguistic patterns expressing causal relations, such as 1995's work using patterns like "because [cause], [effect]", 2002's work using patterns like "NP1-CausativeVerb-NP2", later work using a Naive Bayes classifier, and many more.

1. (2018 CMU Thesis) **Annotating and Automatically Tagging Constructions of Causal Language.**
_Jesse Dunietz_. [[pdf](https://jessedunietz.com/assets/publications/thesis.pdf)] 

1. (2021 arXiv) **A Survey on Extraction of Causal Relations from Natural Language Text.**
_Jie Yang, Soyeon Caren Han, Josiah Poon_. [[pdf](https://arxiv.org/pdf/2101.06426.pdf)]

1. **Richer Event Description (RED) Annotation Guidelines.** _Martha Palmer, Will Styler, Kevin Crooks, Tim O'Gorman_.
[[GitHub](https://github.com/timjogorman/RicherEventDescription/blob/master/guidelines.md)]

1. (2020 Thesis) **Narrative Generation to Support Causal Exploration of Directed Graphs.** 
_Arjun Choudhry_. [[pdf](https://vtechworks.lib.vt.edu/bitstream/handle/10919/98670/Choudhry_A_T_2020.pdf?sequence=1&isAllowed=y)]
#### Method or Dataset Papers
Causal relation extraction from web data
1. (2019 EMNLP) **Weakly Supervised Multilingual Causality Extraction from Wikipedia.**
_Chikara Hashimoto_. 
[[pdf](https://www.aclweb.org/anthology/D19-1296.pdf)]
   <br>[Summary] Cross-verification between Wikipedia and Wikidata, e.g., "Protectionism causes Trade war"

1. (2016 ACL) **Identifying Causal Relations Using Parallel Wikipedia Articles.**
_Christopher Hidey, Kathy McKeown_.
[[pdf](https://www.aclweb.org/anthology/P16-1135.pdf)]
   <br>[Summary] Find linguistic markers like "because".

1. (2014 ACL) **Toward Future Scenario Generation: Extracting Event Causality Exploiting Semantic Relation, Context, and Association Features**
_Chikara Hashimoto, Kentaro Torisawa, Julien Kloetzer, Motoki Sano, István Varga, Jong-Hoon Oh, Yutaka Kidawara_.
[[pdf](https://www.aclweb.org/anthology/P14-1093.pdf)]

1. (2012 EMNLP) **Excitatory or Inhibitory: A New Semantic Orientation Extracts Contradiction and Causality from the Web.**
_Chikara Hashimoto, Kentaro Torisawa, Stijn De Saeger, Jong-Hoon Oh, Jun’ichi Kazama_.
[[pdf](https://www.aclweb.org/anthology/D12-1057.pdf)]
   <br>[Summary] Extracted one million contradiction pairs and 500,000 causality pairs.

1. (1998 Literary and Linguistic Computing) **Automatic extraction of cause-effect information from newspaper text without knowledge-based inferencing.** _Christopher Khoo, Jaklin Kornfilt, Sung Hyon Myaeng, Robert Oddy_.
[[pdf](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.727.5787&rep=rep1&type=pdf)]

1. (1991 Knowledge Acquisition) **Knowledge-based acquisition of causal relationships in text.**
_Randy M. Kaplan, Genevieve Berry-Rogghe_.


Causal relation extraction from curated datasets (relatively small):

1. (2019 NAACL) **Modeling Document-level Causal Structures for Event Causal Relation Identification.** _Lei Gao, Prafulla Kumar Choubey, Ruihong Huang_.
[[pdf](https://www.aclweb.org/anthology/N19-1179.pdf)]
   <br>[Summary] EventStoryLine corpus; method: Integer Linear Programming (ILP)

1. (2018 ACL) **Joint Reasoning for Temporal and Causal Relations.** _Qiang Ning, Zhili Feng, Hao Wu, Dan Roth_. [[pdf](https://www.aclweb.org/anthology/P18-1212.pdf)]
   <br>[Summary] Method: constrained conditional models (CCMs), n integer linear programming (ILP).

1. (2018 SIGdial) **Automatic Extraction of Causal Relations from Text using Linguistically Informed Deep Neural Networks.**
_Tirthankar Dasgupta, Rupsa Saha, Lipika Dey, Abir Naskar_.
[[pdf](https://www.aclweb.org/anthology/W18-5035.pdf)]


1. (2017 ACL Workshop) **The Event StoryLine Corpus: A New Benchmark for Causal and Temporal Relation Extraction.**
_Tommaso Caselli, Piek Vossen_. [[pdf](https://www.aclweb.org/anthology/W17-2711.pdf)]

1. (2017 ACL) **The BECauSE Corpus 2.0: Annotating Causality and Overlapping Relations.** 
_Jesse Dunietz, Lori Levin, Jaime Carbonell_.
[[pdf](https://www.aclweb.org/anthology/W17-0812/)]


1. (2016 ACL Workshop) **CaTeRS: Causal and Temporal Relation Scheme for Semantic Annotation of Event Structures.**
_Nasrin Mostafazadeh, Alyson Grealish, Nathanael Chambers, James Allen, Lucy Vanderwende_. [[pdf](https://www.aclweb.org/anthology/W16-1007.pdf)]

1. (2016 KR) **Commonsense Causal Reasoning between Short Texts.**
_Zhiyi Luo, Yuchen Sha, Kenny Q. Zhu, Seung-Won Hwang, Zhongyuan Wang_. [[pdf](https://www.aaai.org/ocs/index.php/KR/KR16/paper/view/12818/12498)]
   <br>[Summary] Contains a list of causal cue verbs.

1. (2015 ACL Workshop) **Annotating Causal Language Using Corpus Lexicography of Constructions.**
_Jesse Dunietz, Lori Levin, Jaime Carbonell_.
[[pdf](https://www.aclweb.org/anthology/W15-1622.pdf)]
   <br>[Summary] Quite important. This paper teaches the ontology for causality annotation, e.g., Degrees of Causation (cause, enable, prevent), types of causation (consequence, motivation, purpose), instance (causal connective, cause, effect), linguistic type (causality with no lexical trigger, causality with connectives, temporal language).

1. (2014 EACL) **Annotating Causality in the TempEval-3 Corpus.**
_Paramita Mirza, Rachele Sprugnoli, Sara Tonelli, Manuela Speranza_.
[[pdf](https://www.aclweb.org/anthology/W14-0702.pdf)]
   <br>[Summary] Containing some illustrative examples on page 3.

3. (2011 ACL) **Minimally Supervised Event Causality Identification.**
_Quang Do, Yee Seng Chan, Dan Roth_. [[pdf](https://www.aclweb.org/anthology/D11-1027.pdf)]
   <br>[Summary] Uses PMI, IDF, etc.

1. (2009 SemEval) **SemEval-2010 Task 8: Multi-Way Classification of Semantic Relations between Pairs of Nominals**
_Iris Hendrickx, Su Nam Kim, Zornitsa Kozareva, Preslav Nakov, Diarmuid Ó Séaghdha, Sebastian Padó, Marco Pennacchiotti, Lorenza Romano, Stan Szpakowicz_.
[[pdf](https://www.aclweb.org/anthology/S10-1006.pdf)]

1. (2008 LREC) **Building a Corpus of Temporal-Causal Structure.** _Steven Bethard, William Corvey, Sara Klingenstein, James H. Martin_. [[pdf](http://www.lrec-conf.org/proceedings/lrec2008/pdf/229_paper.pdf)]
   <br>[Summary] Combining causal and temporal relation extraction, such as "Fuel tanks had [EVENT leaked] and [EVENT contaminated] the soil." <EVENT_leaked, causes, EVENT_contaminated>. Small dataset with 271 causal relations, and 329 BEFORE/AFTER relations.

1. (2008 LREC) **Causal Relation Extraction.**
_Eduardo Blanco, Nuria Castell, Dan Moldovan_.
[[pdf](http://www.lrec-conf.org/proceedings/lrec2008/pdf/87_paper.pdf)]

1. (2007 SemEval) **SemEval-2007 Task 04: Classification of Semantic Relations between Nominals.**
_Roxana Girju, Preslav Nakov, Vivi Nastase, Stan Szpakowicz, Peter Turney, Deniz Yuret_.
[[pdf](https://www.aclweb.org/anthology/S07-1003.pdf)]

1. (2006 IPM) **Incremental cue phrase learning and bootstrapping method for causality extraction using cue phrase and word pair probabilities.** _Du-Seong Chang, Key-Sun Choi_. [[pdf](https://dl.acm.org/doi/abs/10.1016/j.ipm.2005.04.004)] 

1. (2004 ICNLP) **Causal Relation Extraction Using Cue Phrase and Lexical Pair Probabilities.** _Du-Seong Chang, Key-Sun Choi_. [[pdf](http://semanticweb.kaist.ac.kr/home/images/a/af/Causal_Relation_Extraction_Using_Cue_Phrases_and_Lexical_Pair_Probabilities.pdf)]


1. (2003 ACL Workshop) **Automatic detection of causal relations for question answering.** _Roxana Girju_. [[pdf](https://www.aclweb.org/anthology/W03-1210.pdf)]

1. (2002 AAAI) **Text Mining for Causal Relations.** _Roxana Girju, Dan Moldovan_. [[pdf](https://www.aaai.org/Papers/FLAIRS/2002/FLAIRS02-071.pdf)]

1. (2000 ACL) **Extracting Causal Knowledge from a Medical Database Using Graphical Patterns.**
_Christopher S. G. Khoo, Syin Chan, Yun Niu_.
[[pdf](https://www.aclweb.org/anthology/P00-1043.pdf)]

1. (1997) **Coatis, an nlp system to locate expressions of actions connected by causality links.** _Daniela Garcia_. [[link](https://link.springer.com/chapter/10.1007/BFb0026799)]

1. (1995 PhD Thesis) **Automatic identification of causal relations in text and their use for improving precision in information retrieval.**
_Christopher Khoo_.
[[pdf](https://scholar.google.com/scholar_url?url=https://repository.arizona.edu/bitstream/handle/10150/105106/chris_khoo.PhD_thesis.pdf%3Fsequence%3D1&hl=de&sa=T&oi=gsb-gga&ct=res&cd=0&d=8432224869863885584&ei=g9ymYMOVMMPtmQH3_qPYDg&scisig=AAGBfm07wHjoKM8Q_-LQaYK8Ejq1J2LR0Q)]


#### Some useful tools:

Helping to identify causal verbs, and connectives:

1. (2005 PhD Thesis) **VerbNet: A broad-coverage, comprehensive verb lexicon.** _Karin Kipper Schuler_.
[[pdf](https://verbs.colorado.edu/~kipper/Papers/dissertation.pdf)]

1. (2009 ACL) **Using Syntax to Disambiguate Explicit Discourse Connectives in Text.** _Emily Pitler, Ani Nenkova_. [[pdf](https://www.aclweb.org/anthology/P09-2004.pdf)]


Helping to annotate data efficiently and affordably:

1. (2017 SIGMOD) **Snorkel: Fast Training Set Generation for Information Extraction.** _Alexander J. Ratner, Stephen H. Bach, Henry R. Ehrenberg, Chris Ré_. [[pdf](https://ajratner.github.io/assets/papers/ratner-sigmoddemo17.pdf)]

Helping to analyze the semantics of causal events:

1. (1998 COLING) **The Berkeley FrameNet Project.** _Collin F. Baker, Charles J. Fillmore, John B. Lowe_. [[pdf](https://www.aclweb.org/anthology/C98-1013.pdf)]

1. AMR parsing

1. (2016 ACL Workshop) **The Storyline Annotation and Representation Scheme (StaR): A Proposal.** _Tommaso Caselli, Piek Vossen_. [[pdf](https://www.aclweb.org/anthology/W16-5708.pdf)]

1. (2014 Report) **Guidelines for ECB+ Annotation of Events and their Coreference.** _Agata Cybulska, Piek Vossen_.
[[pdf](http://www.newsreader-project.eu/files/2013/01/NWR-2014-1.pdf)]

### 3.2 Causal Commonsense Reasoning and Generation
1. (2020 EMNLP) **GLUCOSE: GeneraLized and COntextualized Story Explanations.** _Nasrin Mostafazadeh, Aditya Kalyanpur, Lori Moon, David Buchanan, Lauren Berkowitz, Or Biran, Jennifer Chu-Carroll_.
[[pdf](https://arxiv.org/pdf/2009.07758.pdf)]
1. (2019 EMNLP) **Counterfactual Story Reasoning and Generation.**
_Lianhui Qin, Antoine Bosselut, Ari Holtzman, Chandra Bhagavatula, Elizabeth Clark, Yejin Choi_. [[pdf](https://arxiv.org/pdf/1909.04076.pdf)]
1. (2020 IJCAI) **Guided Generation of Cause and Effect.** _Zhongyang Li, Xiao Ding, Ting Liu, J. Edward Hu, Benjamin Van Durme_.
[[pdf](https://www.ijcai.org/Proceedings/2020/0502.pdf)] [[video](https://www.ijcai.org/proceedings/2020/video/24610)]
   <br>[Summary] 314 million automatically extracted cause and effects.

## 3. Causality for Various Applications
### 3.1 Persuasion
1. (arXiv 2020) **Influence via Ethos: On the Persuasive Power of Reputation in Deliberation Online.** _Emaad Manzoor, George H. Chen, Dokyun Lee, Michael D. Smith_. [[pdf](https://arxiv.org/pdf/2006.00707.pdf)]
   <br>[Summary] Cause: reputation, effect: persuation in debates.

1. **Estimating Causal Effects of Tone in Online Debates.**
_Dhanya Sridhar and Lise Getoor_. [[pdf](https://arxiv.org/pdf/1906.04177.pdf)]

### 3.2 Psychology and Behavior
1. **The effect of wording on message propagation: Topic- and author-controlled natural experiments on Twitter.** _Chenhao Tan, Lillian Lee, Bo Pang_. [[pdf](https://www.aclweb.org/anthology/P14-1017.pdf)] 
3. (CHI 2016) **Discovering shifts to suicidal ideation from mental health content in social media.** _Munmun De Choudhury, Emre Kiciman, Mark Dredze, Glen Coppersmith, Mrinal Kumar_. [[pdf](https://dl.acm.org/doi/pdf/10.1145/2858036.2858207?casa_token=ZJKLrg8LAOsAAAAA%3Aecs8HsunRyeUeD_De6Dx15_nPRZ1-mmjiXfAEXLpr25wwz6ywzQcJuZqWjJQIyibEGxZTOkULd1h)]
   <br>[Summary] Method: propensity score matching. Cause: linguistic and social interaction based measures on Reddit text, effect: suicidal attempt.
2. (CWSM 2017) **The Language of Social Support in Social Media and its Effect on Suicidal Ideation Risk.** _Munmun De Choudhury, Emre Kıcıman_. [[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5565730/pdf/nihms891351.pdf)]
   <br>[Summary] Cause: linguistic clues of Reddit comments, effect: suicidal attempt.
   
1. (Political Behavior, 2017) **Tweetment Effects on the Tweeted: Experimentally Reducing Racist Harassment.** _Kevin Munger_. [[pdf](https://link.springer.com/content/pdf/10.1007/s11109-016-9373-5.pdf)]   

1. (ICWSM 2017) **Estimating the Effect Of Exercising On Users’ Online Behavior.**
_Seyed Amin Mirlohi Falavarjani, Hawre Hosseini, Zeinab Noorian, Ebrahim Bagheri_.
[[pdf](https://ojs.aaai.org/index.php/ICWSM/article/view/14975/14825)]
   <br>[Summary] Cause: offline activities from Foursquare posts (e.g., check-ins at a gym, effect: user interests from topics of their Twitter posts. Discovery: shift in interest reduces significantly after users start exercising.
   
1. (CSCW 2017) **Distilling the outcomes of personal experiences: A propensity-scored analysis of social media.** _Alexandra Olteanu, Onur Varol, Emre Kiciman_. [[pdf](https://dl.acm.org/doi/pdf/10.1145/2998181.2998353?casa_token=U8iCSHz-uGUAAAAA:i9qcF0UCEH-lYKhTE9aA5RNMxFlvqfPW0tiHtUsh_lkmdV1F1O9ko9jPIl_nb8Cx5Rbtf4nn5JGq)]

1. (ICWSM 2018) **Using longitudinal social media analysis to understand the effects of early college alcohol use.**
_Emre Kiciman, Scott Counts, Melissa Gasser_. [[pdf](http://kiciman.org/wp-content/uploads/2018/10/college_alcohol_tweets_icwsm18e.pdf)]

1. (ICML 2018) **Estimating causal effects of exercise from mood logging data.**
_Dhanya Sridhar, Aaron Springer, Victoria Hollis, Steve Whittaker, Lise Getoor_.
   <br>[Summary] Cause: daily activities, effect: wellness markers (e.g., mood) on EmotiCal, confounder: Text of mood triggers. Confounding adjustment method: Propensity score matching

1. (ICWSM 2019) **A social media study on the effects of psychiatric medication use.** _Koustuv Saha, Benjamin Sugar, John Torous, Bruno Abrahao, Emre Kıcıman, Munmun De Choudhury_. [[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7152507/pdf/nihms-1578147.pdf)]
   <br>[Summary] Cause: psychiatric drugs, confounder: previous Twitter posts, effect: psychopathology (incl. mood, cognition, depression, anxiety, psychosis, and suicidal ideation). Method: stratified propensity score matching.

1. (Psychological Science 2019) **Increasing vegetable intake by emphasizing tasty and enjoyable attributes: A randomized controlled multisite intervention for taste-focused labeling.** _
Bradley Turnwald, Jaclyn Bertoldo, Margaret Perry, Peggy Policastro, Maureen Timmons, Christopher Bosso, Priscilla Connors, Robert Valgenti, Lindsey Pine, Ghislaine Challamel, Christopher Gardner, Alia Crum_. [pdf](https://journals.sagepub.com/doi/pdf/10.1177/0956797619872191)
   <br>[Summary] Cause: taste-focused lables, or health-focused labels, effect: vegetable intake. Method: RCT.

1. (ICWSM 2021) **The Effect of Moderation on Online Mental Health Conversations.** _
David Wadden, Tal August, Qisheng Li, Tim Althoff_. [pdf](https://arxiv.org/pdf/2005.09225.pdf)
   <br>[Summary] Cause: moderation in online mental health conversations, effect: psychological improvements. Method: natural experiment (comparing the data right before moderators are introduced to a platform and right after).



### 3.3 Economics
1. (arXiv 2017) **A deep causal inference approach to measuring the effects of forming group loans in online non-profit microfinance platform.**
_Thai T Pham and Yuanyuan Shen_. [[pdf](https://arxiv.org/pdf/1706.02795.pdf)]

1. (2020 Journal of Economic Surveys) **Econometrics Meets Sentiment: An Overview of Methodology and Applications.** 
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

1. (eCOM@SIGIR 2017) **Predicting Sales from the Language of Product Descriptions.** _Reid Pryzant, Young-Joo Chung, Dan Jurafsky_ [[pdf](http://ceur-ws.org/Vol-2311/paper_3.pdf)]
   <br>[Summary] Cause: product description (e.g., writing styles and word usages), confounder: brand loyalty and price strategies, effect: sales. Method: adversarial training.
   
## 4. Addressing "Confounders" in NLP

1. (EMNLP 2019) **Topics to Avoid: Demoting Latent Confounds in Text Classification.** _Sachin Kumar, Shuly Wintner, Noah A. Smith, Yulia Tsvetkov_. [[pdf](https://arxiv.org/pdf/1909.00453.pdf)]
   <br>[Summary] Cause: native language, confounder: topic, effect: text

1. (NAACL 2018, Stanford) **Deconfounded lexicon induction for interpretable social science.** _Reid Pryzant, Kelly Shen, Dan Jurafsky, Stefan Wagner_. [[pdf](https://www.aclweb.org/anthology/N18-1146.pdf)]
   <br>[Summary] Cause: some keywords, confounder: , effect: output prediction


1. (EMNLP 2020) **Unsupervised Discovery of Implicit Gender Bias.** _Anjalie Field, Yulia Tsvetkov_. [[pdf](https://www.aclweb.org/anthology/2020.emnlp-main.44.pdf)]
   <br>[Summary] Method: propensity matching and adversarial learning.

1. (AJPS 2020) **Adjusting for confounding with text matching.**
_Margaret E Roberts, Brandon M Stewart, and Richard A Nielsen_. [[pdf](http://www.mit.edu/~rnielsen/textmatching.pdf)]

1. (arXiv 2020) **Adjusting for Confounders with Text: Challenges and an Empirical Evaluation Framework for Causal Inference.** _Galen Weld, Peter West, Maria Glenski, David Arbour, Ryan Rossi, Tim Althoff_. [[pdf](https://arxiv.org/pdf/2009.09961.pdf)]


### 4.1 Causality tools that can be applied to deconfound

1. (NIPS 2017, MPI, discover causal graphs behind data) **Avoiding Discrimination through Causal Reasoning.** _Niki Kilbertus, Mateo Rojas-Carulla, Giambattista Parascandolo, Moritz Hardt, Dominik Janzing, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1706.02744.pdf)]

## 5. More Resources

### 5.1 Causality Papers from Schoelkopf's Lab, MPI

#### Overview

1. (2021 Overview) **Towards Causal Representation Learning.** [[pdf](https://arxiv.org/pdf/2102.11107.pdf)]
1. (2019 Overview) **Causality for Machine Learning.** [[pdf](https://arxiv.org/pdf/1911.10500.pdf)]

#### Independent Causal Mechanisms
1. (2012 ICML) **On Causal and Anticausal Learning.** 
_Bernhard Schölkopf, Dominik Janzing, Jonas Peters, Eleni Sgouritsa, Kun Zhang, Joris Mooij_.
[[pdf](https://icml.cc/2012/papers/625.pdf)]
2. (2018 NeurIPS workshop) **Generalization in anti-causal learning.**
_Niki Kilbertus, Giambattista Parascandolo, Bernhard Schölkopf_.
[[pdf](https://arxiv.org/pdf/1812.00524.pdf)]

1. (UAI 2020) **Semi-supervised learning, causality and the conditional cluster assumption.**
_Julius von Kügelgen, Alexander Mey, Marco Loog, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1905.12081.pdf)]

#### Causal discovery

1. **Causal Discovery from Heterogeneous/Nonstationary Data with Independent Changes.** _Biwei Huang, Kun Zhang, Jiji Zhang, Joseph Ramsey, Ruben Sanchez-Romero, Clark Glymour, Bernhard Schölkopf_. [[pdf](https://arxiv.org/pdf/1903.01672.pdf)]


### 5.2 Causality Papers from Bengio's Lab, MILA

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

Quote from [a blog](https://medium.com/@wcarvalho92/success-vs-failure-generalization-vs-stereotyping-40de0713ab5d): "Causality is the idea that you can model something with an abstraction of the real-world process that generated it. When you use compositionality and learning-to-learn to break down objects into their parts and relations, modeling the object as a creation of these parts can be seen as modeling them in a causal way."

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



### 5.3 Other Causality Papers (Potentially Applicable to NLP)
1. (PSB 2020 Oral) **Robustly Extracting Medical Knowledge from EHRs: A Case Study of Learning a Health Knowledge Graph.** _Irene Y. Chen, Monica Agrawal, Steven Horng, David Sontag_. [[pdf](https://arxiv.org/pdf/1910.01116.pdf)]

1. (2021 AAAI; AI Safety, RL with causality) **Agent Incentives: A Causal Perspective.** _Tom Everitt, Ryan Carey, Eric Langlois, Pedro A Ortega, Shane Legg_.
[[pdf](https://arxiv.org/pdf/2102.01685.pdf)]

1. (2019 IJCAI AI Safety Workshop) **Modeling AGI Safety Frameworks with Causal Influence Diagrams.** _Tom Everitt, Ramana Kumar, Victoria Krakovna, Shane Legg_ ([Causal Incentives Working Group](https://causalincentives.com/)).
[[pdf](https://arxiv.org/pdf/1906.08663.pdf)]

#### Some tools that might be useful for disentanglement
1. (2009) **Tensor Decompositions and Applications.** _Tamara Kolda, Brett Bader_. [[pdf](https://www.kolda.net/publication/TensorReview.pdf)]

### 5.4 Books (for Systematic Learning)

1. (For ML Audience) **Elements of Causal Inference.** _Jonas Peters, Dominik Janzing and Bernhard Schölkopf_. [[Book, 2017](https://library.oapen.org/bitstream/handle/20.500.12657/26040/11283.pdf?sequence=1)]
1. (Quick Primer by Judea Pearl) **Causal Inference in Statistics: A Primer.** _Judea Pearl_. [[Book, 2016](http://bayes.cs.ucla.edu/PRIMER/)]
1. (Focus on SCM) **Causality: Models, Reasoning, and Inference.** _Judea Pearl_. [[Book, 2009](https://www.amazon.de/Causality-Reasoning-Inference-Judea-Pearl/dp/0521773628)]
1. More book recommendations: See Brady Neal's [blog](https://www.bradyneal.com/which-causal-inference-book), and this [pointer](https://sites.google.com/view/causality-reading-group/introduction) to causality books for beginner/intermediate/advanced.
1. A long paper&book list including multiple categories of causality papers: [[spreadsheet](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=0)]

### 5.5 Online Courses

1. **Graphical Models and Causality.** _[Isabelle Guyon](http://www.clopinet.com/isabelle) (ETH)_. [[course website](http://clopinet.com/isabelle/Projects/ETH/Causality_Reading_Group.html)]
1. **Applied Causality (Spring 2019).** _David Blei (Columbia University)_. [[course reading list](http://www.cs.columbia.edu/~blei/seminar/2019-applied-causality/index.html)]

1. (Reading group) **Causality Reading Club@Amsterdam ML Lab.** _Prof. Joris Mooij_. [[past readings](https://amlab.science.uva.nl/meetings/causality-reading-club/)]

### 5.6 People Directory

(Credits to [Causal Resources](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=1999914756).)

- **Judea Pearl** (UCLA), US.
- **Bernhard Schölkopf** (MPI Tübingen), Tübingen, Germany. [[group intro](http://webdav.tuebingen.mpg.de/causality/)]
- **Dominik Janzing** (MPI Tübingen), Tübingen, Germany.
- **Ulrike von Luxburg** (MPI Tübingen), Tübingen, Germany.
- **Joris Mooij** (University of Amsterdam; former: MPI Tübingen), Netherlands. [[home page](https://staff.fnwi.uva.nl/j.m.mooij/)]
- **Jonas Peters** (Copenhagen University; former: MPI Tübingen), Denmark. [[home page](http://web.math.ku.dk/~peters/)]
- **Peter Bühlmann** (ETH), Switzerland.
- **Marloes Maathuis** (ETH), Switzerland. [[video](https://www.youtube.com/watch?v=Q_2cgCeAjpo)]
- **Ilya Shpitser** (JHU; former: UCLA with Judea Pearl), US. [[home page](https://www.cs.jhu.edu/faculty/ilya-shpitser-3/)]
- **Kun Zhang** (CMU; former: MPI Tübingen), Pittsburg, US. 
- **Peter Spirtes** (CMU Philosophy), Pittsburgh, US.
- **Elias Bareinboim** (Columbia), US. [[home page](https://causalai.net/)]
- **Andrew Gelman** (Columbia; former: UCLA with Judea Pearl), US. [[video](https://www.youtube.com/watch?time_continue=25&v=cuE9eHSbjNI&app=desktop)]
- **Stephan Hartmann** (LMU), Munich, Germany.
- **Kosuke Imai** (Harvard; former: Princeton), US. 
- **Ferederick Eberhardt** (Caltech; former: CMU), US.
- **Cheng Soon Ong** (Data61; former: MPI Tübingen), Canberra, Australia.

### 5.7 Workshops

Please see this [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1byIwl_hI-kVtxyTsNcNd6SQRQXJ3CO4xZszDIgFMtIM/edit#gid=416373885) for a list of causality workshops (2016 - now). 

### 5.8 Others

- Job postings for causality researchers: [[website](https://sites.google.com/view/ocis/opportunities-in-causal-inference)]
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
