# Comparing `tmp/text2vec-1.1.7.tar.gz` & `tmp/text2vec-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2vec-1.1.7.tar", last modified: Thu Jul 21 14:22:51 2022, max compression
+gzip compressed data, was "text2vec-1.1.8.tar", last modified: Sun Apr 16 08:49:07 2023, max compression
```

## Comparing `text2vec-1.1.7.tar` & `text2vec-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-07-21 14:22:51.194157 text2vec-1.1.7/
--rw-r--r--   0 xuming     (501) staff       (20)    41521 2022-07-21 14:22:51.193647 text2vec-1.1.7/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    34225 2022-05-22 11:08:21.000000 text2vec-1.1.7/README.md
--rw-r--r--   0 xuming     (501) staff       (20)       38 2022-07-21 14:22:51.194299 text2vec-1.1.7/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1834 2022-03-12 04:27:55.000000 text2vec-1.1.7/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-07-21 14:22:51.175368 text2vec-1.1.7/text2vec/
--rw-r--r--   0 xuming     (501) staff       (20)     1068 2022-03-02 13:21:27.000000 text2vec-1.1.7/text2vec/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     4675 2022-03-03 03:38:02.000000 text2vec-1.1.7/text2vec/bertmatching_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    17829 2022-05-17 02:33:11.000000 text2vec-1.1.7/text2vec/bertmatching_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     1802 2022-02-25 17:25:53.000000 text2vec-1.1.7/text2vec/bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)     2534 2022-03-01 13:17:26.000000 text2vec-1.1.7/text2vec/cosent_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    13470 2022-05-17 02:33:11.000000 text2vec-1.1.7/text2vec/cosent_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     3250 2022-02-16 09:01:18.000000 text2vec-1.1.7/text2vec/ngram.py
--rw-r--r--   0 xuming     (501) staff       (20)    11911 2022-05-20 03:11:08.000000 text2vec-1.1.7/text2vec/sentence_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    14092 2022-05-17 02:33:11.000000 text2vec-1.1.7/text2vec/sentencebert_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     9876 2022-05-17 02:26:31.000000 text2vec-1.1.7/text2vec/similarity.py
--rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.1.7/text2vec/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     4462 2022-03-01 14:06:06.000000 text2vec-1.1.7/text2vec/text_matching_dataset.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-07-21 14:22:51.191120 text2vec-1.1.7/text2vec/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.1.7/text2vec/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6413 2022-01-21 13:50:54.000000 text2vec-1.1.7/text2vec/utils/distance.py
--rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.1.7/text2vec/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)     5848 2021-09-11 10:12:24.000000 text2vec-1.1.7/text2vec/utils/ngram_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.1.7/text2vec/utils/rank_bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.1.7/text2vec/utils/stats_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.1.7/text2vec/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)       84 2022-07-21 14:21:07.000000 text2vec-1.1.7/text2vec/version.py
--rw-r--r--   0 xuming     (501) staff       (20)     6275 2022-03-12 06:18:04.000000 text2vec-1.1.7/text2vec/word2vec.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-07-21 14:22:51.181550 text2vec-1.1.7/text2vec.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    41521 2022-07-21 14:22:50.000000 text2vec-1.1.7/text2vec.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      754 2022-07-21 14:22:50.000000 text2vec-1.1.7/text2vec.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-07-21 14:22:50.000000 text2vec-1.1.7/text2vec.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.1.7/text2vec.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       93 2022-07-21 14:22:50.000000 text2vec-1.1.7/text2vec.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        9 2022-07-21 14:22:50.000000 text2vec-1.1.7/text2vec.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-16 08:49:07.032316 text2vec-1.1.8/
+-rw-r--r--   0 xuming     (501) staff       (20)    41245 2023-04-16 08:49:07.030526 text2vec-1.1.8/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    34181 2023-04-16 03:56:54.000000 text2vec-1.1.8/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-04-16 08:49:07.032703 text2vec-1.1.8/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1619 2023-04-16 08:47:20.000000 text2vec-1.1.8/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-16 08:49:07.014531 text2vec-1.1.8/text2vec/
+-rw-r--r--   0 xuming     (501) staff       (20)     1068 2022-03-02 13:21:27.000000 text2vec-1.1.8/text2vec/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4675 2022-03-03 03:38:02.000000 text2vec-1.1.8/text2vec/bertmatching_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17829 2022-05-17 02:33:11.000000 text2vec-1.1.8/text2vec/bertmatching_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1802 2022-02-25 17:25:53.000000 text2vec-1.1.8/text2vec/bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2534 2022-03-01 13:17:26.000000 text2vec-1.1.8/text2vec/cosent_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13441 2022-08-04 07:57:15.000000 text2vec-1.1.8/text2vec/cosent_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3250 2022-02-16 09:01:18.000000 text2vec-1.1.8/text2vec/ngram.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12375 2023-04-16 07:11:30.000000 text2vec-1.1.8/text2vec/sentence_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14092 2022-05-17 02:33:11.000000 text2vec-1.1.8/text2vec/sentencebert_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9876 2022-05-17 02:26:31.000000 text2vec-1.1.8/text2vec/similarity.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.1.8/text2vec/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     4462 2022-03-01 14:06:06.000000 text2vec-1.1.8/text2vec/text_matching_dataset.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-16 08:49:07.028870 text2vec-1.1.8/text2vec/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.1.8/text2vec/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6413 2022-01-21 13:50:54.000000 text2vec-1.1.8/text2vec/utils/distance.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.1.8/text2vec/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.1.8/text2vec/utils/rank_bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.1.8/text2vec/utils/stats_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.1.8/text2vec/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)       84 2023-04-16 08:47:20.000000 text2vec-1.1.8/text2vec/version.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6275 2022-03-12 06:18:04.000000 text2vec-1.1.8/text2vec/word2vec.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-16 08:49:07.021926 text2vec-1.1.8/text2vec.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    41245 2023-04-16 08:49:06.000000 text2vec-1.1.8/text2vec.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      725 2023-04-16 08:49:06.000000 text2vec-1.1.8/text2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-16 08:49:06.000000 text2vec-1.1.8/text2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.1.8/text2vec.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       87 2023-04-16 08:49:06.000000 text2vec-1.1.8/text2vec.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        9 2023-04-16 08:49:06.000000 text2vec-1.1.8/text2vec.egg-info/top_level.txt
```

### Comparing `text2vec-1.1.7/PKG-INFO` & `text2vec-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,39 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.1.7
+Version: 1.1.8
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [![PyPI version](https://badge.fury.io/py/text2vec.svg)](https://badge.fury.io/py/text2vec)
         [![Downloads](https://pepy.tech/badge/text2vec)](https://pepy.tech/project/text2vec)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # Text2vec
         text2vec, Text to Vector.
         
         文本向量表征工具，把文本转化为向量矩阵，是文本进行计算机处理的第一步。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         
         **Guide**
-        - [Question](#Question)
-        - [Solution](#Solution)
         - [Feature](#Feature)
         - [Evaluation](#Evaluation)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
         - [Reference](#reference)
         
-        # Question
-        文本向量表示咋做？文本匹配任务用哪个模型效果好？
-        
-        许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
-        # Solution
-        ### 传统方法：基于特征的匹配
-        
-        - 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
-        - 优点：可解释性较好
-        - 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
-        
-        代表模型：
-        - BM25
-        
-        BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
-        
-        ### 深度方法：基于表征的匹配
-        - 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
-        - 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
-        - 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
-        
-        > 主要原因是：
-        > 
-        > 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
-        > 
-        > 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
-        
-        
-        代表模型：
-        
-        - [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
-        - [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
-        - [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-        - [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
-        - [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
-        - [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
-        - [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
-        - [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
-        - [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
-        - [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
-        - [CoSENT(2022)](https://kexue.fm/archives/8847)
-        
-        由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
-        
-        所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
-        
-        ### 深度方法：基于交互的匹配
-        
-        - 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
-        - 优点：基于交互的匹配模型端到端处理，效果好
-        - 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
-        
-        
-        代表模型：
-        
-        - [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-        - [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
-        - [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
-        - [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
-        - [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
-        - [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
-        - [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
-        
-        Cross-Encoder适用于向量检索精排。
         
         # Feature
         ### 文本向量表示模型
         - [Word2Vec](text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
@@ -136,32 +69,32 @@
         
         - 本项目release模型的中文匹配评测结果：
         
         | Arch | Backbone | Model Name | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
         | :-- | :--- | :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
         | Word2Vec | word2vec | w2v-light-tencent-chinese | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 |
         | SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 |
-        | CoSENT | hfl/chinese-macbert-base | text2vec-base-chinese | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+        | CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+        | CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese) | - | - | - | - | - | - | - |
         
         说明：
         - 结果值均使用spearman系数
         - 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-        - `CoSENT-macbert-base`模型达到同级别参数量SOTA效果，是用CoSENT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可在各数据集复现结果
-        - `text2vec-base-chinese`模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
+        - [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可复现结果，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
         - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码复现结果
-        - `paraphrase-multilingual-MiniLM-L12-v2`模型名称是`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+        - `paraphrase-multilingual-MiniLM-L12-v2`模型名称是[sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
-        - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base`
+        - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
         - 中文匹配数据集下载[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`first_last_avg`，即 SentenceModel 的`EncoderType.FIRST_LAST_AVG`，其与`EncoderType.MEAN`的方法在预测效果上差异很小
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
         # Demo
         
-        Official Demo: http://42.193.145.218/product/short_text_sim/
+        Official Demo: https://www.mulanai.com/product/short_text_sim/
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         ```shell
@@ -181,74 +114,34 @@
         pip install -r requirements.txt
         
         git clone https://github.com/shibing624/text2vec.git
         cd text2vec
         pip install --no-deps .
         ```
         
-        ### 数据集
-        中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
-        
-        数据集使用示例：
-        ```shell
-        pip install datasets
-        ```
-        
-        ```python
-        from datasets import load_dataset
-        
-        dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
-        print(dataset)
-        print(dataset['test'][0])
-        ```
-        
-        output:
-        ```shell
-        DatasetDict({
-            train: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 5231
-            })
-            validation: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 1458
-            })
-            test: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 1361
-            })
-        })
-        {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
-        ```
-        
-        常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
-        [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
-        可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
-        其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
-        
         # Usage
         
         ## 文本向量表征
         
         基于`pretrained model`计算文本向量：
         
-        ```shell
+        ```zsh
         >>> from text2vec import SentenceModel
         >>> m = SentenceModel()
         >>> m.encode("如何更换花呗绑定银行卡")
         Embedding shape: (768,)
         ```
         
         example: [examples/computing_embeddings_demo.py](examples/computing_embeddings_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
-        from text2vec import SentenceModel, EncoderType
+        from text2vec import SentenceModel
         from text2vec import Word2Vec
         
         
         def compute_emb(model):
             # Embed a list of sentences
             sentences = [
                 '卡',
@@ -268,21 +161,19 @@
                 print("Embedding shape:", embedding.shape)
                 print("Embedding head:", embedding[:10])
                 print()
         
         
         if __name__ == "__main__":
             # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
-            t2v_model = SentenceModel("shibing624/text2vec-base-chinese",
-                                      encoder_type=EncoderType.FIRST_LAST_AVG)
+            t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
             compute_emb(t2v_model)
         
             # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
-                                        encoder_type=EncoderType.MEAN)
+            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
             compute_emb(sbert_model)
         
             # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
             w2v_model = Word2Vec("w2v-light-tencent-chinese")
             compute_emb(w2v_model)
         
         ```
@@ -294,15 +185,15 @@
         Embedding shape: (768,)
         
         Sentence: 银行卡
         Embedding shape: (768,)
          ... 
         ```
         
-        - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`
+        - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
         - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
         模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
         是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
         模型自动下载到本机路径：`~/.cache/huggingface/transformers`
         - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
         适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
         - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
@@ -365,16 +256,16 @@
         print(sentence_embeddings)
         ```
         
         #### `Word2Vec`词向量
         
         提供两种`Word2Vec`词向量，任选一个：
         
-          - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制，运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
-          - [腾讯词向量-官方全量](https://ai.tencent.com/ailab/nlp/zh/download.html), 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/embedding.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/zh/data/Tencent_AILab_ChineseEmbedding.tar.gz  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
+          - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制文件，111M，是简化后的高频143613个词，每个词向量还是200维（跟原版一样），运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
+          - 腾讯词向量-官方全量, 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/index.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/en/download.html  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
         
         
         
         ## 下游任务
         ### 1. 句子相似度计算
         
         example: [examples/semantic_text_similarity_demo.py](examples/semantic_text_similarity_demo.py)
@@ -545,60 +436,51 @@
         
         
         Inference:
         
         <img src="docs/inference.png" width="300" />
         
         #### CoSENT 监督模型
-        训练和预测，最简示例:
-        
-        ```python
-        from text2vec import CosentModel
-        m = CosentModel("bert-base-chinese")
-        print(m)
-        m.train_model(use_hf_dataset=True, num_epochs=1, output_dir="./temp")
-        r = m.encode(["我爱北京天安门"])
-        print(r)
-        ```
+        训练和预测CoSENT模型：
         
-        - 在中文STS-B数据集训练和评估`MacBERT+CoSENT`模型
+        - 在中文STS-B数据集训练和评估`CoSENT`模型
         
         example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-cosent
         ```
         
-        - 在蚂蚁金融匹配数据集ATEC上训练和评估`MacBERT+CoSENT`模型
+        - 在蚂蚁金融匹配数据集ATEC上训练和评估`CoSENT`模型
         
         支持这些中文匹配数据集的使用：'ATEC', 'STS-B', 'BQ', 'LCQMC', 'PAWSX'，具体参考HuggingFace datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
         ```shell
         python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
         ```
         
         - 在自有中文数据集上训练模型
         
         example: [examples/training_sup_text_matching_model_selfdata.py](examples/training_sup_text_matching_model_selfdata.py)
         
         ```shell
         python training_sup_text_matching_model_selfdata.py --do_train --do_predict
         ```
         
-        - 在英文STS-B数据集训练和评估`BERT+CoSENT`模型
+        - 在英文STS-B数据集训练和评估`CoSENT`模型
         
         example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased  --output_dir ./outputs/STS-B-en-cosent
         ```
         
         #### CoSENT 无监督模型
-        - 在英文NLI数据集训练`BERT+CoSENT`模型，在STS-B测试集评估效果
+        - 在英文NLI数据集训练`CoSENT`模型，在STS-B测试集评估效果
         
         example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
         ```
@@ -616,33 +498,33 @@
         
         
         Inference:
         
         <img src="docs/sbert_inference.png" width="300" />
         
         #### SentenceBERT 监督模型
-        - 在中文STS-B数据集训练和评估`MacBERT+SBERT`模型
+        - 在中文STS-B数据集训练和评估`SBERT`模型
         
         example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-sbert
         ```
-        - 在英文STS-B数据集训练和评估`BERT+SBERT`模型
+        - 在英文STS-B数据集训练和评估`SBERT`模型
         
         example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-sbert
         ```
         
         #### SentenceBERT 无监督模型
-        - 在英文NLI数据集训练`BERT+SBERT`模型，在STS-B测试集评估效果
+        - 在英文NLI数据集训练`SBERT`模型，在STS-B测试集评估效果
         
         example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
         ```
@@ -733,20 +615,132 @@
         - 调用服务：
         ```shell
         curl -X 'GET' \
           'http://0.0.0.0:8001/emb?q=hello' \
           -H 'accept: application/json'
         ```
         
+        
+        ## 数据集
+        中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
+        
+        数据集使用示例：
+        ```shell
+        pip install datasets
+        ```
+        
+        ```python
+        from datasets import load_dataset
+        
+        dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
+        print(dataset)
+        print(dataset['test'][0])
+        ```
+        
+        output:
+        ```shell
+        DatasetDict({
+            train: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 5231
+            })
+            validation: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 1458
+            })
+            test: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 1361
+            })
+        })
+        {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
+        ```
+        
+        常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
+        [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
+        可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
+        其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
+        
+        <details>
+        <summary>文本向量方法介绍</summary>
+        
+        # Question
+        文本向量表示咋做？文本匹配任务用哪个模型效果好？
+        
+        许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
+        # Solution
+        ### 传统方法：基于特征的匹配
+        
+        - 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
+        - 优点：可解释性较好
+        - 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
+        
+        代表模型：
+        - BM25
+        
+        BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
+        
+        ### 深度方法：基于表征的匹配
+        - 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
+        - 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
+        - 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
+        
+        > 主要原因是：
+        > 
+        > 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
+        > 
+        > 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
+        
+        
+        代表模型：
+        
+        - [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
+        - [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
+        - [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+        - [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
+        - [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
+        - [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
+        - [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
+        - [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
+        - [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
+        - [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
+        - [CoSENT(2022)](https://kexue.fm/archives/8847)
+        
+        由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
+        
+        所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
+        
+        ### 深度方法：基于交互的匹配
+        
+        - 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
+        - 优点：基于交互的匹配模型端到端处理，效果好
+        - 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
+        
+        
+        代表模型：
+        
+        - [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+        - [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
+        - [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
+        - [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
+        - [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
+        - [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
+        - [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
+        
+        Cross-Encoder适用于向量检索精排。
+        
+        </details>
+        
+        
+        
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         - 邮件我：xuming: xuming624@qq.com
-        - 微信我：
-        加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
+        - 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
         
         # Citation
         
         如果你在研究中使用了text2vec，请按如下格式引用：
@@ -754,19 +748,21 @@
         APA:
         ```latex
         Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
         ```
         
         BibTeX:
         ```latex
-        @software{Xu_Text2vec_Text_to,
-        author = {Xu, Ming},
-        title = {{Text2vec: Text to vector toolkit}},
-        url = {https://github.com/shibing624/text2vec},
-        version = {1.1.2}
+        @misc{Text2vec,
+          author = {Xu, Ming},
+          title = {Text2vec: Text to vector toolkit},
+          year = {2022},
+          publisher = {GitHub},
+          journal = {GitHub repository},
+          howpublished = {\url{https://github.com/shibing624/text2vec}},
         }
         ```
         
         # License
         
         
         授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
@@ -795,14 +791,10 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `text2vec-1.1.7/README.md` & `text2vec-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,98 +1,31 @@
 [![PyPI version](https://badge.fury.io/py/text2vec.svg)](https://badge.fury.io/py/text2vec)
 [![Downloads](https://pepy.tech/badge/text2vec)](https://pepy.tech/project/text2vec)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
 # Text2vec
 text2vec, Text to Vector.
 
 文本向量表征工具，把文本转化为向量矩阵，是文本进行计算机处理的第一步。
 
 **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
 
 
 **Guide**
-- [Question](#Question)
-- [Solution](#Solution)
 - [Feature](#Feature)
 - [Evaluation](#Evaluation)
 - [Install](#install)
 - [Usage](#usage)
 - [Contact](#Contact)
 - [Reference](#reference)
 
-# Question
-文本向量表示咋做？文本匹配任务用哪个模型效果好？
-
-许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
-# Solution
-### 传统方法：基于特征的匹配
-
-- 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
-- 优点：可解释性较好
-- 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
-
-代表模型：
-- BM25
-
-BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
-
-### 深度方法：基于表征的匹配
-- 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
-- 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
-- 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
-
-> 主要原因是：
-> 
-> 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
-> 
-> 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
-
-
-代表模型：
-
-- [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
-- [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
-- [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-- [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
-- [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
-- [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
-- [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
-- [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
-- [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
-- [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
-- [CoSENT(2022)](https://kexue.fm/archives/8847)
-
-由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
-
-所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
-
-### 深度方法：基于交互的匹配
-
-- 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
-- 优点：基于交互的匹配模型端到端处理，效果好
-- 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
-
-
-代表模型：
-
-- [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-- [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
-- [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
-- [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
-- [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
-- [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
-- [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
-
-Cross-Encoder适用于向量检索精排。
 
 # Feature
 ### 文本向量表示模型
 - [Word2Vec](text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
 - [SBERT(Sentence-BERT)](text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
 - [CoSENT(Cosine Sentence)](text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
 
@@ -128,32 +61,32 @@
 
 - 本项目release模型的中文匹配评测结果：
 
 | Arch | Backbone | Model Name | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
 | :-- | :--- | :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
 | Word2Vec | word2vec | w2v-light-tencent-chinese | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 |
 | SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 |
-| CoSENT | hfl/chinese-macbert-base | text2vec-base-chinese | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+| CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+| CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese) | - | - | - | - | - | - | - |
 
 说明：
 - 结果值均使用spearman系数
 - 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-- `CoSENT-macbert-base`模型达到同级别参数量SOTA效果，是用CoSENT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可在各数据集复现结果
-- `text2vec-base-chinese`模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
+- [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可复现结果，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
 - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码复现结果
-- `paraphrase-multilingual-MiniLM-L12-v2`模型名称是`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+- `paraphrase-multilingual-MiniLM-L12-v2`模型名称是[sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
 - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
-- 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base`
+- 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
 - 中文匹配数据集下载[链接见下方](#数据集)
 - 中文匹配任务实验表明，pooling最优是`first_last_avg`，即 SentenceModel 的`EncoderType.FIRST_LAST_AVG`，其与`EncoderType.MEAN`的方法在预测效果上差异很小
 - QPS的GPU测试环境是Tesla V100，显存32GB
 
 # Demo
 
-Official Demo: http://42.193.145.218/product/short_text_sim/
+Official Demo: https://www.mulanai.com/product/short_text_sim/
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
 
 ![](docs/hf.png)
 
 run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
 ```shell
@@ -173,74 +106,34 @@
 pip install -r requirements.txt
 
 git clone https://github.com/shibing624/text2vec.git
 cd text2vec
 pip install --no-deps .
 ```
 
-### 数据集
-中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
-
-数据集使用示例：
-```shell
-pip install datasets
-```
-
-```python
-from datasets import load_dataset
-
-dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
-print(dataset)
-print(dataset['test'][0])
-```
-
-output:
-```shell
-DatasetDict({
-    train: Dataset({
-        features: ['sentence1', 'sentence2', 'label'],
-        num_rows: 5231
-    })
-    validation: Dataset({
-        features: ['sentence1', 'sentence2', 'label'],
-        num_rows: 1458
-    })
-    test: Dataset({
-        features: ['sentence1', 'sentence2', 'label'],
-        num_rows: 1361
-    })
-})
-{'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
-```
-
-常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
-[LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
-可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
-其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
-
 # Usage
 
 ## 文本向量表征
 
 基于`pretrained model`计算文本向量：
 
-```shell
+```zsh
 >>> from text2vec import SentenceModel
 >>> m = SentenceModel()
 >>> m.encode("如何更换花呗绑定银行卡")
 Embedding shape: (768,)
 ```
 
 example: [examples/computing_embeddings_demo.py](examples/computing_embeddings_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
-from text2vec import SentenceModel, EncoderType
+from text2vec import SentenceModel
 from text2vec import Word2Vec
 
 
 def compute_emb(model):
     # Embed a list of sentences
     sentences = [
         '卡',
@@ -260,21 +153,19 @@
         print("Embedding shape:", embedding.shape)
         print("Embedding head:", embedding[:10])
         print()
 
 
 if __name__ == "__main__":
     # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
-    t2v_model = SentenceModel("shibing624/text2vec-base-chinese",
-                              encoder_type=EncoderType.FIRST_LAST_AVG)
+    t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
     compute_emb(t2v_model)
 
     # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-    sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
-                                encoder_type=EncoderType.MEAN)
+    sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
     compute_emb(sbert_model)
 
     # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
     w2v_model = Word2Vec("w2v-light-tencent-chinese")
     compute_emb(w2v_model)
 
 ```
@@ -286,15 +177,15 @@
 Embedding shape: (768,)
 
 Sentence: 银行卡
 Embedding shape: (768,)
  ... 
 ```
 
-- 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`
+- 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
 - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
 模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
 是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
 模型自动下载到本机路径：`~/.cache/huggingface/transformers`
 - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
 适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
 - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
@@ -357,16 +248,16 @@
 print(sentence_embeddings)
 ```
 
 #### `Word2Vec`词向量
 
 提供两种`Word2Vec`词向量，任选一个：
 
-  - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制，运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
-  - [腾讯词向量-官方全量](https://ai.tencent.com/ailab/nlp/zh/download.html), 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/embedding.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/zh/data/Tencent_AILab_ChineseEmbedding.tar.gz  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
+  - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制文件，111M，是简化后的高频143613个词，每个词向量还是200维（跟原版一样），运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
+  - 腾讯词向量-官方全量, 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/index.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/en/download.html  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
 
 
 
 ## 下游任务
 ### 1. 句子相似度计算
 
 example: [examples/semantic_text_similarity_demo.py](examples/semantic_text_similarity_demo.py)
@@ -537,60 +428,51 @@
 
 
 Inference:
 
 <img src="docs/inference.png" width="300" />
 
 #### CoSENT 监督模型
-训练和预测，最简示例:
-
-```python
-from text2vec import CosentModel
-m = CosentModel("bert-base-chinese")
-print(m)
-m.train_model(use_hf_dataset=True, num_epochs=1, output_dir="./temp")
-r = m.encode(["我爱北京天安门"])
-print(r)
-```
+训练和预测CoSENT模型：
 
-- 在中文STS-B数据集训练和评估`MacBERT+CoSENT`模型
+- 在中文STS-B数据集训练和评估`CoSENT`模型
 
 example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
 
 ```shell
 cd examples
 python training_sup_text_matching_model.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-cosent
 ```
 
-- 在蚂蚁金融匹配数据集ATEC上训练和评估`MacBERT+CoSENT`模型
+- 在蚂蚁金融匹配数据集ATEC上训练和评估`CoSENT`模型
 
 支持这些中文匹配数据集的使用：'ATEC', 'STS-B', 'BQ', 'LCQMC', 'PAWSX'，具体参考HuggingFace datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
 ```shell
 python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
 ```
 
 - 在自有中文数据集上训练模型
 
 example: [examples/training_sup_text_matching_model_selfdata.py](examples/training_sup_text_matching_model_selfdata.py)
 
 ```shell
 python training_sup_text_matching_model_selfdata.py --do_train --do_predict
 ```
 
-- 在英文STS-B数据集训练和评估`BERT+CoSENT`模型
+- 在英文STS-B数据集训练和评估`CoSENT`模型
 
 example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
 
 ```shell
 cd examples
 python training_sup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased  --output_dir ./outputs/STS-B-en-cosent
 ```
 
 #### CoSENT 无监督模型
-- 在英文NLI数据集训练`BERT+CoSENT`模型，在STS-B测试集评估效果
+- 在英文NLI数据集训练`CoSENT`模型，在STS-B测试集评估效果
 
 example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
 
 ```shell
 cd examples
 python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
 ```
@@ -608,33 +490,33 @@
 
 
 Inference:
 
 <img src="docs/sbert_inference.png" width="300" />
 
 #### SentenceBERT 监督模型
-- 在中文STS-B数据集训练和评估`MacBERT+SBERT`模型
+- 在中文STS-B数据集训练和评估`SBERT`模型
 
 example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
 
 ```shell
 cd examples
 python training_sup_text_matching_model.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-sbert
 ```
-- 在英文STS-B数据集训练和评估`BERT+SBERT`模型
+- 在英文STS-B数据集训练和评估`SBERT`模型
 
 example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
 
 ```shell
 cd examples
 python training_sup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-sbert
 ```
 
 #### SentenceBERT 无监督模型
-- 在英文NLI数据集训练`BERT+SBERT`模型，在STS-B测试集评估效果
+- 在英文NLI数据集训练`SBERT`模型，在STS-B测试集评估效果
 
 example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
 
 ```shell
 cd examples
 python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
 ```
@@ -725,20 +607,132 @@
 - 调用服务：
 ```shell
 curl -X 'GET' \
   'http://0.0.0.0:8001/emb?q=hello' \
   -H 'accept: application/json'
 ```
 
+
+## 数据集
+中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
+
+数据集使用示例：
+```shell
+pip install datasets
+```
+
+```python
+from datasets import load_dataset
+
+dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
+print(dataset)
+print(dataset['test'][0])
+```
+
+output:
+```shell
+DatasetDict({
+    train: Dataset({
+        features: ['sentence1', 'sentence2', 'label'],
+        num_rows: 5231
+    })
+    validation: Dataset({
+        features: ['sentence1', 'sentence2', 'label'],
+        num_rows: 1458
+    })
+    test: Dataset({
+        features: ['sentence1', 'sentence2', 'label'],
+        num_rows: 1361
+    })
+})
+{'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
+```
+
+常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
+[LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
+可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
+其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
+
+<details>
+<summary>文本向量方法介绍</summary>
+
+# Question
+文本向量表示咋做？文本匹配任务用哪个模型效果好？
+
+许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
+# Solution
+### 传统方法：基于特征的匹配
+
+- 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
+- 优点：可解释性较好
+- 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
+
+代表模型：
+- BM25
+
+BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
+
+### 深度方法：基于表征的匹配
+- 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
+- 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
+- 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
+
+> 主要原因是：
+> 
+> 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
+> 
+> 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
+
+
+代表模型：
+
+- [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
+- [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
+- [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+- [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
+- [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
+- [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
+- [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
+- [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
+- [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
+- [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
+- [CoSENT(2022)](https://kexue.fm/archives/8847)
+
+由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
+
+所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
+
+### 深度方法：基于交互的匹配
+
+- 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
+- 优点：基于交互的匹配模型端到端处理，效果好
+- 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
+
+
+代表模型：
+
+- [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+- [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
+- [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
+- [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
+- [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
+- [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
+- [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
+
+Cross-Encoder适用于向量检索精排。
+
+</details>
+
+
+
 # Contact
 
 - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
 - 邮件我：xuming: xuming624@qq.com
-- 微信我：
-加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
+- 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
 
 # Citation
 
 如果你在研究中使用了text2vec，请按如下格式引用：
@@ -746,19 +740,21 @@
 APA:
 ```latex
 Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
 ```
 
 BibTeX:
 ```latex
-@software{Xu_Text2vec_Text_to,
-author = {Xu, Ming},
-title = {{Text2vec: Text to vector toolkit}},
-url = {https://github.com/shibing624/text2vec},
-version = {1.1.2}
+@misc{Text2vec,
+  author = {Xu, Ming},
+  title = {Text2vec: Text to vector toolkit},
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/shibing624/text2vec}},
 }
 ```
 
 # License
 
 
 授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
```

### Comparing `text2vec-1.1.7/setup.py` & `text2vec-1.1.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import sys
 
 from setuptools import setup, find_packages
 
 # Avoids IDE errors, but actual version is read from version.py
-__version__ = None
+__version__ = ""
 exec(open('text2vec/version.py').read())
 
 if sys.version_info < (3,):
     sys.exit('Sorry, Python3 is required.')
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
@@ -29,29 +29,24 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords='word embedding,text2vec,Chinese Text Similarity Calculation Tool,similarity,word2vec',
     install_requires=[
         "jieba>=0.39",
         "loguru",
         "transformers>=4.6.0",
         "datasets",
         "tqdm",
         "scikit-learn",
         "gensim>=4.0.0",
-        "numpy",
         "pandas",
     ],
     packages=find_packages(exclude=['tests']),
     package_dir={'text2vec': 'text2vec'},
     package_data={'text2vec': ['*.*', 'data/*.txt']}
 )
```

### Comparing `text2vec-1.1.7/text2vec/__init__.py` & `text2vec-1.1.8/text2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/bertmatching_dataset.py` & `text2vec-1.1.8/text2vec/bertmatching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/bertmatching_model.py` & `text2vec-1.1.8/text2vec/bertmatching_model.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/bm25.py` & `text2vec-1.1.8/text2vec/bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/cosent_dataset.py` & `text2vec-1.1.8/text2vec/cosent_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/cosent_model.py` & `text2vec-1.1.8/text2vec/cosent_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         )
         logger.info(f" Training model done. Saved to {output_dir}.")
 
         return global_step, training_details
 
     def calc_loss(self, y_true, y_pred):
         """
-        CoSENT的排序loss，refer：https://kexue.fm/archives/8847
+        矩阵计算batch内的cos loss
         """
         # 1. 取出真实的标签
         y_true = y_true[::2]  # tensor([1, 0, 1]) 真实的标签
         # 2. 对输出的句子向量进行l2归一化   后面只需要对应为相乘  就可以得到cos值了
         norms = (y_pred ** 2).sum(axis=1, keepdims=True) ** 0.5
         y_pred = y_pred / norms
         # 3. 奇偶向量相乘, 相似度矩阵除以温度系数0.05(等于*20)
```

### Comparing `text2vec-1.1.7/text2vec/ngram.py` & `text2vec-1.1.8/text2vec/ngram.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/sentence_model.py` & `text2vec-1.1.8/text2vec/sentence_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: Base sentence model function, add encode function.
-Parts of this file is adapted from the sentence-transformers library at https://github.com/UKPLab/sentence-transformers.
+Parts of this file is adapted from the sentence-transformers: https://github.com/UKPLab/sentence-transformers
 """
 import os
 from enum import Enum
 from typing import List, Union, Optional
 from tqdm.autonotebook import trange
 import numpy as np
 import torch
@@ -73,15 +73,27 @@
         self.device = torch.device(device)
         logger.debug("Use device: {}".format(self.device))
         self.bert.to(self.device)
         self.results = {}  # Save training process evaluation result
 
     def __str__(self):
         return f"<SentenceModel: {self.model_name_or_path}, encoder_type: {self.encoder_type}, " \
-               f"max_seq_length: {self.max_seq_length}>"
+               f"max_seq_length: {self.max_seq_length}, emb_dim: {self.get_sentence_embedding_dimension()}>"
+
+    def get_sentence_embedding_dimension(self):
+        """
+        Get the dimension of the sentence embeddings.
+
+        Returns
+        -------
+        int or None
+            The dimension of the sentence embeddings, or None if it cannot be determined.
+        """
+        # Use getattr to safely access the out_features attribute of the pooler's dense layer
+        return getattr(self.bert.pooler.dense, "out_features", None)
 
     def get_sentence_embeddings(self, input_ids, attention_mask, token_type_ids):
         """
         Returns the model output by encoder_type as embeddings.
 
         Utility function for self.bert() method.
         """
@@ -128,24 +140,24 @@
             self,
             sentences: Union[str, List[str]],
             batch_size: int = 64,
             show_progress_bar: bool = False,
             convert_to_numpy: bool = True,
             convert_to_tensor: bool = False,
             device: str = None,
-        ):
+    ):
         """
         Returns the embeddings for a batch of sentences.
 
         :param sentences: str/list, Input sentences
         :param batch_size: int, Batch size
         :param show_progress_bar: bool, Whether to show a progress bar for the sentences
         :param convert_to_numpy: If true, the output is a list of numpy vectors. Else, it is a list of pytorch tensors.
         :param convert_to_tensor: If true, you get one large tensor as return. Overwrites any setting from convert_to_numpy
-        :param device: Which torch.device to use for the computation
+        :param device: Which device to use for the computation
         """
         self.bert.eval()
         if device is None:
             device = self.device
         if convert_to_tensor:
             convert_to_numpy = False
         input_is_string = False
```

### Comparing `text2vec-1.1.7/text2vec/sentencebert_model.py` & `text2vec-1.1.8/text2vec/sentencebert_model.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/similarity.py` & `text2vec-1.1.8/text2vec/similarity.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/stopwords.txt` & `text2vec-1.1.8/text2vec/stopwords.txt`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/text_matching_dataset.py` & `text2vec-1.1.8/text2vec/text_matching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/utils/distance.py` & `text2vec-1.1.8/text2vec/utils/distance.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/utils/get_file.py` & `text2vec-1.1.8/text2vec/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/utils/rank_bm25.py` & `text2vec-1.1.8/text2vec/utils/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/utils/stats_util.py` & `text2vec-1.1.8/text2vec/utils/stats_util.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/utils/tokenizer.py` & `text2vec-1.1.8/text2vec/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec/word2vec.py` & `text2vec-1.1.8/text2vec/word2vec.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.1.7/text2vec.egg-info/PKG-INFO` & `text2vec-1.1.8/text2vec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,39 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.1.7
+Version: 1.1.8
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [![PyPI version](https://badge.fury.io/py/text2vec.svg)](https://badge.fury.io/py/text2vec)
         [![Downloads](https://pepy.tech/badge/text2vec)](https://pepy.tech/project/text2vec)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # Text2vec
         text2vec, Text to Vector.
         
         文本向量表征工具，把文本转化为向量矩阵，是文本进行计算机处理的第一步。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         
         **Guide**
-        - [Question](#Question)
-        - [Solution](#Solution)
         - [Feature](#Feature)
         - [Evaluation](#Evaluation)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
         - [Reference](#reference)
         
-        # Question
-        文本向量表示咋做？文本匹配任务用哪个模型效果好？
-        
-        许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
-        # Solution
-        ### 传统方法：基于特征的匹配
-        
-        - 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
-        - 优点：可解释性较好
-        - 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
-        
-        代表模型：
-        - BM25
-        
-        BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
-        
-        ### 深度方法：基于表征的匹配
-        - 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
-        - 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
-        - 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
-        
-        > 主要原因是：
-        > 
-        > 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
-        > 
-        > 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
-        
-        
-        代表模型：
-        
-        - [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
-        - [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
-        - [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-        - [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
-        - [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
-        - [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
-        - [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
-        - [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
-        - [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
-        - [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
-        - [CoSENT(2022)](https://kexue.fm/archives/8847)
-        
-        由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
-        
-        所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
-        
-        ### 深度方法：基于交互的匹配
-        
-        - 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
-        - 优点：基于交互的匹配模型端到端处理，效果好
-        - 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
-        
-        
-        代表模型：
-        
-        - [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
-        - [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
-        - [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
-        - [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
-        - [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
-        - [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
-        - [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
-        
-        Cross-Encoder适用于向量检索精排。
         
         # Feature
         ### 文本向量表示模型
         - [Word2Vec](text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
@@ -136,32 +69,32 @@
         
         - 本项目release模型的中文匹配评测结果：
         
         | Arch | Backbone | Model Name | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
         | :-- | :--- | :---- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
         | Word2Vec | word2vec | w2v-light-tencent-chinese | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 |
         | SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 |
-        | CoSENT | hfl/chinese-macbert-base | text2vec-base-chinese | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+        | CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | **48.25** | 3008 |
+        | CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese) | - | - | - | - | - | - | - |
         
         说明：
         - 结果值均使用spearman系数
         - 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-        - `CoSENT-macbert-base`模型达到同级别参数量SOTA效果，是用CoSENT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可在各数据集复现结果
-        - `text2vec-base-chinese`模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
+        - [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)模型，是用CoSENT方法训练，基于MacBERT在中文STS-B数据训练得到，并在中文STS-B测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码可复现结果，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文语义匹配任务推荐使用
         - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)代码复现结果
-        - `paraphrase-multilingual-MiniLM-L12-v2`模型名称是`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+        - `paraphrase-multilingual-MiniLM-L12-v2`模型名称是[sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)，是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
-        - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base`
+        - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
         - 中文匹配数据集下载[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`first_last_avg`，即 SentenceModel 的`EncoderType.FIRST_LAST_AVG`，其与`EncoderType.MEAN`的方法在预测效果上差异很小
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
         # Demo
         
-        Official Demo: http://42.193.145.218/product/short_text_sim/
+        Official Demo: https://www.mulanai.com/product/short_text_sim/
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         ```shell
@@ -181,74 +114,34 @@
         pip install -r requirements.txt
         
         git clone https://github.com/shibing624/text2vec.git
         cd text2vec
         pip install --no-deps .
         ```
         
-        ### 数据集
-        中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
-        
-        数据集使用示例：
-        ```shell
-        pip install datasets
-        ```
-        
-        ```python
-        from datasets import load_dataset
-        
-        dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
-        print(dataset)
-        print(dataset['test'][0])
-        ```
-        
-        output:
-        ```shell
-        DatasetDict({
-            train: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 5231
-            })
-            validation: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 1458
-            })
-            test: Dataset({
-                features: ['sentence1', 'sentence2', 'label'],
-                num_rows: 1361
-            })
-        })
-        {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
-        ```
-        
-        常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
-        [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
-        可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
-        其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
-        
         # Usage
         
         ## 文本向量表征
         
         基于`pretrained model`计算文本向量：
         
-        ```shell
+        ```zsh
         >>> from text2vec import SentenceModel
         >>> m = SentenceModel()
         >>> m.encode("如何更换花呗绑定银行卡")
         Embedding shape: (768,)
         ```
         
         example: [examples/computing_embeddings_demo.py](examples/computing_embeddings_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
-        from text2vec import SentenceModel, EncoderType
+        from text2vec import SentenceModel
         from text2vec import Word2Vec
         
         
         def compute_emb(model):
             # Embed a list of sentences
             sentences = [
                 '卡',
@@ -268,21 +161,19 @@
                 print("Embedding shape:", embedding.shape)
                 print("Embedding head:", embedding[:10])
                 print()
         
         
         if __name__ == "__main__":
             # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
-            t2v_model = SentenceModel("shibing624/text2vec-base-chinese",
-                                      encoder_type=EncoderType.FIRST_LAST_AVG)
+            t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
             compute_emb(t2v_model)
         
             # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
-                                        encoder_type=EncoderType.MEAN)
+            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
             compute_emb(sbert_model)
         
             # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
             w2v_model = Word2Vec("w2v-light-tencent-chinese")
             compute_emb(w2v_model)
         
         ```
@@ -294,15 +185,15 @@
         Embedding shape: (768,)
         
         Sentence: 银行卡
         Embedding shape: (768,)
          ... 
         ```
         
-        - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`
+        - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
         - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
         模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
         是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
         模型自动下载到本机路径：`~/.cache/huggingface/transformers`
         - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
         适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
         - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
@@ -365,16 +256,16 @@
         print(sentence_embeddings)
         ```
         
         #### `Word2Vec`词向量
         
         提供两种`Word2Vec`词向量，任选一个：
         
-          - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制，运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
-          - [腾讯词向量-官方全量](https://ai.tencent.com/ailab/nlp/zh/download.html), 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/embedding.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/zh/data/Tencent_AILab_ChineseEmbedding.tar.gz  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
+          - 轻量版腾讯词向量 [百度云盘-密码:tawe](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) 或 [谷歌云盘](https://drive.google.com/u/0/uc?id=1iQo9tBb2NgFOBxx0fA16AZpSgc-bG_Rp&export=download)，二进制文件，111M，是简化后的高频143613个词，每个词向量还是200维（跟原版一样），运行程序，自动下载到 `~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
+          - 腾讯词向量-官方全量, 6.78G放到： `~/.text2vec/datasets/Tencent_AILab_ChineseEmbedding.txt`，腾讯词向量主页：https://ai.tencent.com/ailab/nlp/zh/index.html 词向量下载地址：https://ai.tencent.com/ailab/nlp/en/download.html  更多查看[腾讯词向量介绍-wiki](https://github.com/shibing624/text2vec/wiki/%E8%85%BE%E8%AE%AF%E8%AF%8D%E5%90%91%E9%87%8F%E4%BB%8B%E7%BB%8D)
         
         
         
         ## 下游任务
         ### 1. 句子相似度计算
         
         example: [examples/semantic_text_similarity_demo.py](examples/semantic_text_similarity_demo.py)
@@ -545,60 +436,51 @@
         
         
         Inference:
         
         <img src="docs/inference.png" width="300" />
         
         #### CoSENT 监督模型
-        训练和预测，最简示例:
-        
-        ```python
-        from text2vec import CosentModel
-        m = CosentModel("bert-base-chinese")
-        print(m)
-        m.train_model(use_hf_dataset=True, num_epochs=1, output_dir="./temp")
-        r = m.encode(["我爱北京天安门"])
-        print(r)
-        ```
+        训练和预测CoSENT模型：
         
-        - 在中文STS-B数据集训练和评估`MacBERT+CoSENT`模型
+        - 在中文STS-B数据集训练和评估`CoSENT`模型
         
         example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-cosent
         ```
         
-        - 在蚂蚁金融匹配数据集ATEC上训练和评估`MacBERT+CoSENT`模型
+        - 在蚂蚁金融匹配数据集ATEC上训练和评估`CoSENT`模型
         
         支持这些中文匹配数据集的使用：'ATEC', 'STS-B', 'BQ', 'LCQMC', 'PAWSX'，具体参考HuggingFace datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
         ```shell
         python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
         ```
         
         - 在自有中文数据集上训练模型
         
         example: [examples/training_sup_text_matching_model_selfdata.py](examples/training_sup_text_matching_model_selfdata.py)
         
         ```shell
         python training_sup_text_matching_model_selfdata.py --do_train --do_predict
         ```
         
-        - 在英文STS-B数据集训练和评估`BERT+CoSENT`模型
+        - 在英文STS-B数据集训练和评估`CoSENT`模型
         
         example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased  --output_dir ./outputs/STS-B-en-cosent
         ```
         
         #### CoSENT 无监督模型
-        - 在英文NLI数据集训练`BERT+CoSENT`模型，在STS-B测试集评估效果
+        - 在英文NLI数据集训练`CoSENT`模型，在STS-B测试集评估效果
         
         example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
         ```
@@ -616,33 +498,33 @@
         
         
         Inference:
         
         <img src="docs/sbert_inference.png" width="300" />
         
         #### SentenceBERT 监督模型
-        - 在中文STS-B数据集训练和评估`MacBERT+SBERT`模型
+        - 在中文STS-B数据集训练和评估`SBERT`模型
         
         example: [examples/training_sup_text_matching_model.py](examples/training_sup_text_matching_model.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/STS-B-sbert
         ```
-        - 在英文STS-B数据集训练和评估`BERT+SBERT`模型
+        - 在英文STS-B数据集训练和评估`SBERT`模型
         
         example: [examples/training_sup_text_matching_model_en.py](examples/training_sup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_sup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-sbert
         ```
         
         #### SentenceBERT 无监督模型
-        - 在英文NLI数据集训练`BERT+SBERT`模型，在STS-B测试集评估效果
+        - 在英文NLI数据集训练`SBERT`模型，在STS-B测试集评估效果
         
         example: [examples/training_unsup_text_matching_model_en.py](examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
         ```
@@ -733,20 +615,132 @@
         - 调用服务：
         ```shell
         curl -X 'GET' \
           'http://0.0.0.0:8001/emb?q=hello' \
           -H 'accept: application/json'
         ```
         
+        
+        ## 数据集
+        中文语义匹配数据集已经上传到huggingface datasets [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)
+        
+        数据集使用示例：
+        ```shell
+        pip install datasets
+        ```
+        
+        ```python
+        from datasets import load_dataset
+        
+        dataset = load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or STS-B
+        print(dataset)
+        print(dataset['test'][0])
+        ```
+        
+        output:
+        ```shell
+        DatasetDict({
+            train: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 5231
+            })
+            validation: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 1458
+            })
+            test: Dataset({
+                features: ['sentence1', 'sentence2', 'label'],
+                num_rows: 1361
+            })
+        })
+        {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
+        ```
+        
+        常见中文语义匹配数据集，包含[ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)、[BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)、
+        [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)、[PAWSX](https://arxiv.org/abs/1908.11828)、[STS-B](https://github.com/pluto-junzeng/CNSD)共5个任务。
+        可以从数据集对应的链接自行下载，也可以从[百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)下载。
+        其中senteval_cn目录是评测数据集汇总，senteval_cn.zip是senteval目录的打包，两者下其一就好。
+        
+        <details>
+        <summary>文本向量方法介绍</summary>
+        
+        # Question
+        文本向量表示咋做？文本匹配任务用哪个模型效果好？
+        
+        许多NLP任务的成功离不开训练优质有效的文本表示向量。特别是文本语义匹配（Semantic Textual Similarity，如paraphrase检测、QA的问题对匹配）、文本向量检索（Dense Text Retrieval）等任务。
+        # Solution
+        ### 传统方法：基于特征的匹配
+        
+        - 基于TF-IDF、BM25、Jaccord、SimHash、LDA等算法抽取两个文本的词汇、主题等层面的特征，然后使用机器学习模型（LR, xgboost）训练分类模型
+        - 优点：可解释性较好
+        - 缺点：依赖人工寻找特征，泛化能力一般，而且由于特征数量的限制，模型的效果比较一般
+        
+        代表模型：
+        - BM25
+        
+        BM25算法，通过候选句子的字段对qurey字段的覆盖程度来计算两者间的匹配得分，得分越高的候选项与query的匹配度更好，主要解决词汇层面的相似度问题。
+        
+        ### 深度方法：基于表征的匹配
+        - 基于表征的匹配方式，初始阶段对两个文本各自单独处理，通过深层的神经网络进行编码（encode），得到文本的表征（embedding），再对两个表征进行相似度计算的函数得到两个文本的相似度
+        - 优点：基于BERT的模型通过有监督的Fine-tune在文本表征和文本匹配任务取得了不错的性能
+        - 缺点：BERT自身导出的句向量（不经过Fine-tune，对所有词向量求平均）质量较低，甚至比不上Glove的结果，因而难以反映出两个句子的语义相似度
+        
+        > 主要原因是：
+        > 
+        > 1.BERT对所有的句子都倾向于编码到一个较小的空间区域内，这使得大多数的句子对都具有较高的相似度分数，即使是那些语义上完全无关的句子对。
+        > 
+        > 2.BERT句向量表示的聚集现象和句子中的高频词有关。具体来说，当通过平均词向量的方式计算句向量时，那些高频词的词向量将会主导句向量，使之难以体现其原本的语义。当计算句向量时去除若干高频词时，聚集现象可以在一定程度上得到缓解，但表征能力会下降。
+        
+        
+        代表模型：
+        
+        - [DSSM(2013)](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf)
+        - [CDSSM(2014)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/www2014_cdssm_p07.pdf)
+        - [ARC I(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+        - [Siamese Network(2016)](https://www.aclweb.org/anthology/W16-1617.pdf)
+        - [InferSent(2017)](https://arxiv.org/pdf/1705.02364.pdf)
+        - [BERT(2018)](https://arxiv.org/pdf/1810.04805.pdf)
+        - [Sentence-BERT(2019)](https://arxiv.org/abs/1908.10084)
+        - [BERT-flow(2020)](https://arxiv.org/abs/2011.05864)
+        - [SimCSE(2021)](https://arxiv.org/abs/2104.08821)
+        - [ConSERT(2021)](https://aclanthology.org/2021.acl-long.393/)
+        - [CoSENT(2022)](https://kexue.fm/archives/8847)
+        
+        由于2018年BERT模型在NLP界带来了翻天覆地的变化，此处不讨论和比较2018年之前的模型（如果有兴趣了解的同学，可以参考中科院开源的[MatchZoo](https://github.com/NTMC-Community/MatchZoo) 和[MatchZoo-py](https://github.com/NTMC-Community/MatchZoo-py)）。
+        
+        所以，本项目主要调研以下比原生BERT更优、适合文本匹配的向量表示模型：Sentence-BERT(2019)、BERT-flow(2020)、SimCSE(2021)、CoSENT(2022)。
+        
+        ### 深度方法：基于交互的匹配
+        
+        - 基于交互的匹配方式，则认为在最后阶段才计算文本的相似度会过于依赖文本表征的质量，同时也会丢失基础的文本特征（比如词法、句法等），所以提出尽可能早的对文本特征进行交互，捕获更基础的特征，最后在高层基于这些基础匹配特征计算匹配分数
+        - 优点：基于交互的匹配模型端到端处理，效果好
+        - 缺点：这类模型（Cross-Encoder）的输入要求是两个句子，输出的是句子对的相似度值，模型不会产生句子向量表示（sentence embedding），我们也无法把单个句子输入给模型。因此，对于需要文本向量表示的任务来说，这类模型并不实用
+        
+        
+        代表模型：
+        
+        - [ARC II(2014)](https://arxiv.org/pdf/1503.03244.pdf)
+        - [MV-LSTM(2015)](https://arxiv.org/pdf/1511.08277.pdf)
+        - [MatchPyramid(2016)](https://arxiv.org/pdf/1602.06359.pdf)
+        - [DRMM(2016)](https://www.bigdatalab.ac.cn/~gjf/papers/2016/CIKM2016a_guo.pdf)
+        - [Conv-KNRM(2018)](https://www.cs.cmu.edu/~zhuyund/papers/WSDM_2018_Dai.pdf)
+        - [RE2(2019)](https://www.aclweb.org/anthology/P19-1465.pdf)
+        - [Keyword-BERT(2020)](https://arxiv.org/ftp/arxiv/papers/2003/2003.11516.pdf)
+        
+        Cross-Encoder适用于向量检索精排。
+        
+        </details>
+        
+        
+        
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         - 邮件我：xuming: xuming624@qq.com
-        - 微信我：
-        加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
+        - 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
         
         # Citation
         
         如果你在研究中使用了text2vec，请按如下格式引用：
@@ -754,19 +748,21 @@
         APA:
         ```latex
         Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
         ```
         
         BibTeX:
         ```latex
-        @software{Xu_Text2vec_Text_to,
-        author = {Xu, Ming},
-        title = {{Text2vec: Text to vector toolkit}},
-        url = {https://github.com/shibing624/text2vec},
-        version = {1.1.2}
+        @misc{Text2vec,
+          author = {Xu, Ming},
+          title = {Text2vec: Text to vector toolkit},
+          year = {2022},
+          publisher = {GitHub},
+          journal = {GitHub repository},
+          howpublished = {\url{https://github.com/shibing624/text2vec}},
         }
         ```
         
         # License
         
         
         授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
@@ -795,14 +791,10 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `text2vec-1.1.7/text2vec.egg-info/SOURCES.txt` & `text2vec-1.1.8/text2vec.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,11 +19,10 @@
 text2vec.egg-info/dependency_links.txt
 text2vec.egg-info/not-zip-safe
 text2vec.egg-info/requires.txt
 text2vec.egg-info/top_level.txt
 text2vec/utils/__init__.py
 text2vec/utils/distance.py
 text2vec/utils/get_file.py
-text2vec/utils/ngram_util.py
 text2vec/utils/rank_bm25.py
 text2vec/utils/stats_util.py
 text2vec/utils/tokenizer.py
```

