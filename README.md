# Paper sharing

[TOC]

## Text Matching

#### LET: Linguistic Knowledge Enhanced Graph Transformer for Chinese Short Text Matching, AAAI 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/17592)

此文解决了两个问题：一是中文词语的多义性（构造word lattice graph解决）；二是模型受分词效果的影响（多粒度信息解决）。

提出了语言知识增强匹配模型。不是将句子分词成词序列，而是采用不同的分词工具，保留分词路径，形成一个词格图，文本匹配转化成图匹配任务，解决了问题2。通过HowNet获取到一个词的不同意义，解决问题1，HowNet作为外部知识库。



## Graph Neural Network

#### The Graph Neural Network Model, IEEE Transactions on Neural Networks, 2009

此文为GNN的起源



## Information Retrieval

#### Transformer Memory as a Differentiable Search Index, NlPS2022. [paper](https://arxiv.org/abs/2202.06991)

这篇文章挺有意思，不是学习doc本身的表示来与query进行匹配，而是学习doc的id来进行匹配。

关联doc与docid的方式为Seq2seq模型，通过自回归生成来进行检索排序。

改进点：将检索和排序放在一个模型中，改变了双塔模型的范式。
