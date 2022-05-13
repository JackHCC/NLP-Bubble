# NLP-Bubble
🖨 Natural Language Processing Learning Blog，a Study Bubble to recording learning.

![](image/logo/NLP-Bubble-banner.png)

💡 NLP Learning Record 💡



## Lessons/Books

- [Statistical Learning Method v1](https://blog.creativecc.cn/posts/Lesson-Statistical-Learning-Method.html)

- [CS224N Natural Language Processing 2022](https://github.com/JackHCC/Awesome-DL-Models/tree/master/Docx/CS224N)
- [CS224W Machine Learning with Graphs 2021](https://blog.creativecc.cn/posts/Lesson-CS224W-Machine-Learning-with-Graphs.html)



## Papers

- [Arxiv NLP Reporter](https://github.com/JackHCC/Arxiv-NLP-Reporter)
  - [Web Reader](https://blog.creativecc.cn/Arxiv-NLP-Reporter/)

- Reading Web

  - [ACL anthology](https://www.aclweb.org/anthology/)
  - [NeurIPS](https://papers.nips.cc) , ICML, ICLR

  - [online preprint servers](https://arxiv.org)



## DataSet

### Classes

- Linguistic Data Consortium
  - [Linguistic Data Consortium (upenn.edu)](https://catalog.ldc.upenn.edu/)
  - [Linguistics (stanford.edu)](https://linguistics.stanford.edu/resources/resources-corpora)
- Machine translation
  - [Statistical Machine Translation (statmt.org)](https://statmt.org/)
- Dependency parsing: Universal Dependencies
  - [Universal Dependencies](https://universaldependencies.org/)

### Other

- Awesome
  - [NLPDataSet](https://github.com/liucongg/NLPDataSet)
  - [nlp-datasets](https://github.com/niderhoff/nlp-datasets)

- Platform
  - [千言：中文开源数据集合](https://www.luge.ai/)
  - [Papers With Code](https://paperswithcode.com/datasets)
  - Kaggle 
  - [GLUE](https://gluebenchmark.com/tasks)


- Blogs
  - [Datasets for Natural Language Processing](https://machinelearningmastery.com/datasets-natural-language-processing/)
  - [Sentiment Analysis](https://nlp.stanford.edu/sentiment/)
  - [The bAbI](https://research.facebook.com/downloads/babi/)



## NLP Task

思维导图：

![](../../../Blog/JackCC.Blog/hexo_blog/source/images/lesson/NLP_Task.png)

常见的32项NLP任务以及对应的评测数据、评测指标、目前的SOTA结果（2020.05）以及对应的Paper与Code.

| 任务                                           | 描述                | corpus/dataset                       | 评价指标                                   | SOTA                                       | Papers                                                       | Code                                                         |
| ---------------------------------------------- | ------------------- | ------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Chunking                                       | 组块分析            | Penn Treebank                        | F1                                         | 95.77                                      | [A Joint Many-Task Model: Growing a Neural Network for Multiple NLP Tasks](https://arxiv.org/pdf/1611.01587v5.pdf) | [Link](https://github.com/hassyGo/charNgram2vec)             |
| Common sense reasoning                         | 常识推理            | Event2Mind                           | cross-entropy                              | 4.22                                       | [Event2Mind: Commonsense Inference on Events, Intents, and Reactions](https://www.dialog-21.ru/media/5090/fenogenovaasplusetal-010.pdf) | [Link](https://github.com/Alenush/russian_event2mind)        |
| Parsing                                        | 句法分析            | Penn Treebank                        | F1                                         | 95.13                                      | [Constituency Parsing with a Self-Attentive Encoder](https://arxiv.org/pdf/1805.01052v1.pdf) | [Link](https://github.com/nikitakit/self-attentive-parser)   |
| Coreference resolution                         | 指代消解            | CoNLL 2012                           | average F1                                 | 73                                         | [Higher-order Coreference Resolution with Coarse-to-fine Inference](https://arxiv.org/pdf/1804.05392v1.pdf) | [Link](https://github.com/kentonl/e2e-coref)                 |
| Dependency parsing                             | 依存句法分析        | Penn Treebank                        | POS<br/>UAS<br/>LAS                        | 97.3<br/>95.44<br/>93.76                   | [Deep Biaffine Attention for Neural Dependency Parsing](https://arxiv.org/pdf/1611.01734v3.pdf) | [Link](https://github.com/PaddlePaddle/PaddleNLP/tree/develop/examples/dependency_parsing/ddparser) |
| Task-Oriented Dialogue/Intent Detection        | 任务型对话/意图识别 | ATIS/Snips                           | accuracy                                   | 94.1  97.0                                 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](https://aclanthology.org/N18-2118.pdf) | [Link](https://github.com/MiuLab/SlotGated-SLU)              |
| Task-Oriented Dialogue/Slot Filling            | 任务型对话/槽填充   | ATIS/Snips                           | F1                                         | 95.2<br/>88.8                              | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](https://aclanthology.org/N18-2118.pdf) | [Link](https://github.com/MiuLab/SlotGated-SLU)              |
| Task-Oriented Dialogue/Dialogue State Tracking | 任务型对话/状态追踪 | DSTC2                                | Area<br/>Food<br/>Price<br/>Joint          | 90<br/>84<br/>92<br/>72                    | [Dialogue Learning with Human Teaching and Feedback in End-to-End Trainable Task-Oriented Dialogue Systems](https://arxiv.org/pdf/1804.06512v1.pdf) | [Link](https://github.com/google-research-datasets/simulated-dialogue) |
| Domain adaptation                              | 领域适配            | Multi-Domain Sentiment Dataset       | average <br/>accuracy                      | 79.15                                      | [Strong Baselines for Neural Semi-supervised Learning under Domain Shift](https://arxiv.org/pdf/1804.09530v1.pdf) | [Link](https://github.com/bplank/semi-supervised-baselines)  |
| Entity Linking                                 | 实体链接            | AIDA CoNLL-YAGO                      | Micro-F1-strong<br/>Macro-F1-strong        | 86.6 <br/>89.4                             | [End-to-End Neural Entity Linking](https://arxiv.org/pdf/1808.07699v2.pdf) | [Link](https://github.com/dalab/end2end_neural_el)           |
| Information Extraction                         | 信息抽取            | ReVerb45K                            | Precision<br/>Recall<br/>F1                | 62.7<br/>84.4<br/>81.9                     | [CESI: Canonicalizing Open Knowledge Bases using Embeddings and Side Information](https://arxiv.org/pdf/1902.00172v1.pdf) | [Link](https://github.com/malllabiisc/cesi)                  |
| Grammatical Error Correction                   | 语法错误纠正        | JFLEG                                | GLEU                                       | 61.5                                       | [Near Human-Level Performance in Grammatical Error Correction with Hybrid Machine Translation](https://arxiv.org/pdf/1804.05945v1.pdf) | Link                                                         |
| Language modeling                              | 语言模型            | Penn Treebank                        | Validation perplexity<br/> Test perplexity | 48.33<br/>47.69                            | [Breaking the Softmax Bottleneck: A High-Rank RNN Language Model](https://arxiv.org/pdf/1711.03953v4.pdf) | [Link](https://github.com/zihangdai/mos)                     |
| Lexical Normalization                          | 词汇规范化          | LexNorm2015                          | F1<br/>Precision<br/>Recall                | 86.39 <br/>93.53 <br/>80.26                | [MoNoise: Modeling Noise Using a Modular Normalization System](https://arxiv.org/pdf/1710.03476v1.pdf) | [Link](https://bitbucket.org/robvanderg/monoise)             |
| Machine translation                            | 机器翻译            | WMT 2014 EN-DE                       | BLEU                                       | 35.0                                       | [Understanding Back-Translation at Scale](https://arxiv.org/pdf/1808.09381v2.pdf) | [Link](https://github.com/pytorch/fairseq)                   |
| Multimodal Emotion Recognition                 | 多模态情感识别      | IEMOCAP                              | Accuracy                                   | 76.5                                       | [Multimodal Sentiment Analysis using Hierarchical Fusion with Context Modeling](https://arxiv.org/pdf/1806.06228v1.pdf) | [Link](https://github.com/SenticNet/hfusion)                 |
| Multimodal Metaphor Recognition                | 多模态隐喻识别      | verb-noun pairs adjective-noun pairs | F1                                         | 0.75<br/>0.79                              | [Black Holes and White Rabbits: Metaphor Identification with Visual Features](https://aclanthology.org/N16-1020.pdf) | Link                                                         |
| Multimodal Sentiment Analysis                  | 多模态情感分析      | MOSI                                 | Accuracy                                   | 80.3                                       | [Context-Dependent Sentiment Analysis in User-Generated Videos](https://aclanthology.org/P17-1081.pdf) | [Link](https://github.com/senticnet/sc-lstm)                 |
| Named entity recognition                       | 命名实体识别        | CoNLL 2003                           | F1                                         | 93.09                                      | [Contextual String Embeddings for Sequence Labeling](https://aclanthology.org/C18-1139.pdf) | [Link](https://github.com/zalandoresearch/flair)             |
| Natural language inference                     | 自然语言推理        | SciTail                              | Accuracy                                   | 88.3                                       | [Improving Language Understanding by Generative Pre-Training](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf) | [Link](https://github.com/huggingface/transformers)          |
| Part-of-speech tagging                         | 词性标注            | Penn Treebank                        | Accuracy                                   | 97.96                                      | [Morphosyntactic Tagging with a Meta-BiLSTM Model over Context Sensitive Token Encodings](https://arxiv.org/pdf/1805.08237v1.pdf) | [Link](https://github.com/google/meta_tagger)                |
| Question answering                             | 问答                | CliCR                                | F1                                         | 33.9                                       | [CliCR: A Dataset of Clinical Case Reports for Machine Reading Comprehension](https://arxiv.org/pdf/1803.09720v1.pdf) | [Link](https://github.com/clips/clicr)                       |
| Word segmentation                              | 分词                | VLSP 2013                            | F1                                         | 97.90                                      | [A Fast and Accurate Vietnamese Word Segmenter](https://arxiv.org/pdf/1709.06307v2.pdf) | [Link](https://github.com/datquocnguyen/RDRsegmenter)        |
| Word Sense Disambiguation                      | 词义消歧            | SemEval 2015                         | F1                                         | 67.1                                       | [Word Sense Disambiguation: A Unified Evaluation Framework and Empirical Comparison](https://aclanthology.org/E17-1010.pdf) | Link                                                         |
| Text classification                            | 文本分类            | AG News                              | Error rate                                 | 5.01                                       | [Universal Language Model Fine-tuning for Text Classification](https://arxiv.org/pdf/1801.06146v5.pdf) | [Link](https://github.com/fastai/fastai)                     |
| Summarization                                  | 摘要                | Gigaword                             | ROUGE-1<br/>ROUGE-2<br/>ROUGE-L            | 37.04<br/>19.03<br/>34.46                  | [Retrieve, Rerank and Rewrite: Soft Template Based Neural Summarization](https://aclanthology.org/P18-1015.pdf) | Link                                                         |
| Sentiment analysis                             | 情感分析            | IMDb                                 | Accuracy                                   | 95.4                                       | [Universal Language Model Fine-tuning for Text Classification](https://arxiv.org/pdf/1801.06146v5.pdf) | [Link](https://github.com/fastai/fastai)                     |
| Semantic role labeling                         | 语义角色标注        | OntoNotes                            | F1                                         | 85.5                                       | [Jointly Predicting Predicates and Arguments in Neural Semantic Role Labeling](https://arxiv.org/pdf/1805.04787v2.pdf) | [Link](https://github.com/luheng/lsgn)                       |
| Semantic parsing                               | 语义解析            | LDC2014T12                           | F1 Newswire<br/>F1 Full                    | 0.71<br/>0.66                              | [AMR Parsing with an Incremental Joint Model](https://arxiv.org/pdf/1909.04303v2.pdf) | [Link](https://github.com/jcyk/AMR-parser)                   |
| Semantic textual similarity                    | 语义文本相似度      | SentEval                             | MRPC<br/>SICK-R<br/>SICK-E<br/>STS         | 78.6/84.4<br/>0.888<br/>87.8<br/>78.9/78.6 | [Learning General Purpose Distributed Sentence Representations via Large Scale Multi-task Learning](https://arxiv.org/pdf/1804.00079v1.pdf) | [Link](https://github.com/facebookresearch/SentEval)         |
| Relationship Extraction                        | 关系抽取            | New York Times Corpus                | P@10%<br/>P@30%                            | 73.6<br/>59.5                              | [RESIDE: Improving Distantly-Supervised Neural Relation Extraction using Side Information](https://arxiv.org/pdf/1812.04361v2.pdf) | [Link](https://github.com/malllabiisc/RESIDE)                |
| Relation Prediction                            | 关系预测            | WN18RR                               | H@10<br/>H@1<br/>MRR                       | 59.02<br/>45.37<br/>49.83                  | [Predicting Semantic Relations using Global Graph Properties](https://arxiv.org/pdf/1808.08644v1.pdf) | [Link](https://github.com/yuvalpinter/m3gm)                  |



## Resource

- [NLP-Interview-Notes](https://github.com/km1994/NLP-Interview-Notes)
- [Recommendation-Advertisement-Search](https://github.com/km1994/recommendation_advertisement_search)
- [NLPer-Arsenal](https://github.com/TingFree/NLPer-Arsenal)
- [AI-Surveys](https://github.com/KaiyuanGao/AI-Surveys)



## Interview

- [Machine Learning](./docs/interview/machine-learning.md)
- [Deep Learning](./docs/interview/deep-learning.md)
- [Word Embedding](./docs/interview/word-embedding.md)
- [Transformer](./docs/interview/transformer.md)
- [Bert](./docs/interview/bert.md)
- [Reverse](./docs/interview/reverse-interview.md)



© [JackHCC](https://github.com/JackHCC)



