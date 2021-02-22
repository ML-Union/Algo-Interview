# Algo-Interview

| 推荐系统&nbsp; | 计算广告 | 深度学习&nbsp;| &nbsp;机器学习&nbsp;&nbsp;|&nbsp;python&nbsp;&nbsp;|C++| &nbsp;&nbsp;spark&nbsp;&nbsp; |自然语言处理| 
| :---: | :----: | :---: | :----: | :----: | :----: | :----: | :----: | 
| [:computer:](#computer-推荐系统) |[:pencil2:](#pencil2-计算广告) | [:cloud:](#cloud-深度学习) | [:art:](#art-机器学习) | [:floppy_disk:](#floppy_disk-python) |[:coffee:](#coffee-C++)| [:bulb:](#bulb-Spark) |[:wrench:](#wrench-自然语言处理)|


## :computer: 推荐系统百问百答

网站版

- [1. 浅层模型篇](http://ml-union.com/2021/02/18/Recommend-1/)
- [2. 深度模型篇](http://ml-union.com/2021/02/19/Recommend-2/)
- [3. Embedding篇](http://ml-union.com/2021/02/20/Recommend-3/)
- [4. 召回篇](http://ml-union.com/2021/02/21/Recommend-4/)
- [5. 特征工程篇](http://ml-union.com/2021/02/22/Recommend-5/)
- [6. 冷启动与EE](http://ml-union.com/2021/02/23/Recommend-6/)
- [7. 性能与评估](http://ml-union.com/2021/02/24/Recommend-7/)

github版

- [1. 浅层模型篇](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/1.%20%E6%B5%85%E5%B1%82%E6%A8%A1%E5%9E%8B%E7%AF%87.md)
- [2. 深度模型篇](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/2.%20%E6%B7%B1%E5%BA%A6%E6%A8%A1%E5%9E%8B%E7%AF%87.md)
- [3. Embedding篇](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/3.%20Embedding%E7%AF%87.md)
- [4. 召回篇](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/4.%20%E5%8F%AC%E5%9B%9E%E7%B3%BB%E7%BB%9F%E7%AF%87.md)
- [5. 特征工程篇](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/5.%20%E7%89%B9%E5%BE%81%E5%B7%A5%E7%A8%8B%E7%AF%87.md)
- [6. 冷启动与EE](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/6.%20%E5%86%B7%E5%90%AF%E5%8A%A8%E4%B8%8EEE.md)
- [7. 性能与评估](https://github.com/ML-Union/Algo-Interview/blob/main/Recommendation-system/7.%20%E6%80%A7%E8%83%BD%E4%B8%8E%E8%AF%84%E4%BC%B0.md)

问题目录：
### 浅层模型篇
#### 协同过滤
- 请简述基于用户的协同过滤UserCF的推荐过程。
- 在基于用户的协同过滤中，如何计算用户的相似度？
- 基于用户的协同过滤UserCF存在哪些缺陷？
- 请简述基于物品的协同过滤ItemCF的推荐过程。
- UserCF和ItemCF分别适用于哪些应用场景？为什么？
- 协同过滤算法存在哪些缺陷？
#### 矩阵分解
- 矩阵分解的原理是什么？求解的主要方法有哪些？
- 如何从深度学习模型的角度来认识矩阵分解模型
- 矩阵分解算法中，隐向量的长度$k$的取值是如何影响效果和工程开销的？
- 请简述奇异值分解的过程。奇异值分解存在什么缺陷？为什么不适用于互联网场景下的求解？
- 请简述梯度下降法求解用户-物品隐向量的过程。
- 如何解决矩阵分解中用户和物品打分偏差的问题？
- 矩阵分解有哪些优点与缺点？与协同过滤相比较呢？
- 如何从神经网络的角度理解矩阵分解？
#### 逻辑回归
- 逻辑回归模型预估相较于协同过滤，最大的优势是什么？其推荐过程是怎么样的？
- 请推导逻辑回归的数学形式。
- 请推导梯度下降法求解逻辑回归参数更新的过程。
- 逻辑回归作为CTR预估模型的优势与缺陷是什么？
#### FM与FFM
- 所有的特征进行两两交叉，并对所有的的组合赋予权重的方法存在什么缺陷？
- FM的原理是什么？与矩阵分解有什么联系？
- FM相较于POLY2为什么泛化能力更好？在工程上有什么优势？
- FFM相较于FM有什么改进？
- FM的训练复杂度是多少？怎么推导？FFM的训练复杂度是多少？
#### GBDT+LR
- 为什么GBDT可用于特征选择和特征组合？
- GBDT+LR组合模型中，GBDT是如何生成特征向量的？
- GBDT+LR有什么优点和缺陷？
#### LS-PLM
- 请简述阿里妈妈提出的LS-PLM模型的原理与数学形式。
- LS-PLM模型的优势有哪些？
- LS-PLM模型与深度学习模型有什么联系？

### 深度模型篇
#### Deep Crossing
- 请简述Deep Crossing的网络结构。
- Deep Crossing中的残差单元有什么作用？
#### NeuralCF
- NeuralCF在矩阵分解模型的基础上，做了哪些改进？
- 模型结构越复杂越好吗？特征越多越好吗？
#### PNN模型
- PNN相较NeuralCF和Deep Crossing有哪些改进？优势是什么？
- PNN中特征交叉有哪些方式？分别是怎么样的？
- PNN模型的优势和局限性是什么？
#### Wide&Deep
- 如何理解Wide&Deep模型的泛化能力和记忆能力？
- 请简述Wide&Deep的模型结构。
- Wide&Deep模型的创新和优势是什么？
#### Deep&Cross模型
- Deep&Cross相比Wide&Deep作了哪些改进？Deep&Cross模型的Cross网络是怎么操作的？
#### FNN模型
- FNN模型的提出主要是为了解决什么问题？它是如何解决的？
- FNN的模型结构是什么样的？
- FNN模型中是如何使用FM来初始化Embeddiing层参数的？
#### DeepFM
- DeepFM相较于Wide&Deep有什么改进？为什么这么改进？
#### NFM
- NFM相比Wide&Deep有什么改进？为什么这么改？
#### AFM
- AFM的网络结构是什么样的？
- AFM模型为何要在推荐系统模型中引入注意力机制？是如何引入注意力机制的？
#### DIN
- DIN的结构是怎样的？是如何引入注意力机制的？动机是什么？
#### DIEN
- DIEN引入序列信息的动机是什么？
- 请绘制DIEN各层的结构？兴趣抽取层和兴趣进化层。
#### ESSM
- 请说明ESSM模型的多目标优化设计的动机，以及是怎么做的？

### Embedding篇
#### Embeddng
- Embedding技术为何对深度学习推荐系统来说非常重要？
- 请简述Word2Vec的原理和结构。
- 为了加快Word2Vec的训练，采取了什么方法？
- 谈谈你对Item2Vec的理解，它的局限是什么？
- 请简述双塔模型的结构，其中物品塔的作用是什么？
- DeepWalk的主要思想是什么？说出算法步骤
- DeepWalk中随机游走的跳转概率是怎么计算的？
- Node2Vec中的同质性和结构性指的是什么？他们与DFS和BFS的对应关系如何？
- 请写出Node2Vec的节点间跳转概率公式。
- 举例说明Node2Vec的同质性和结构性在推荐系统中的直观解释。
- LINE
- EGES的提出主要是为了弥补DeepWalk的缺陷的？怎么弥补的？
- 请简述EGES模型的结构，并简述每一层的做法。
- SDNE
- Struc2Vec
- Embedding在深度学习推荐系统中有哪些应用？列举三个方向。
- Embedding作为深度学习模型的训练会存在什么问题？
- Embedding有哪些预训练方法，分别介绍一下.
- 请简述Embedding作为召回层的过程。
- 请简述局部敏感哈希的原理及其在推荐系统中的作用。

### 特征工程篇
#### 特征工程
- 让你设计一个推荐系统的特征工程，你会怎么去设计？包括用户侧、物品侧和上下文特征。
- 在进行特征处理时，对连续型特征怎么处理？
- 在进行特征处理时，对类别型特征怎么处理？

### 召回系统篇
#### 召回
- 假设物品库数量达到百万级别，如何设计方法从这个数量级别的物品中推荐给用户top10的物品，同时可以减少计算的压力？
- 推荐系统中为什么要有召回？在推荐系统中召回和排序有什么异同？
- 请举例说明一些简单的多路召回策略。
- 请简述基于embedding的召回方法，优势是什么？
- 请简要描述DSSM是如何应用于召回的？结构是怎样的？
- 请简述YoutubeDNN的结构和其原理
- 请简述用户多兴趣网络MIND的出发点是什么，描述其结构？
- SDM是如何结合用户长期和短期兴趣建模的？其结构如何？
- TDM 深度树匹配召回

### 性能与评估篇
#### 推荐系统的性能
- 模型的实时性是如何影响推荐系统的效果的？
- 客户端是如何做到对于实时特征进行实时推荐的？
- 流计算平台是如何进行准实时特征处理的？
- 分布式存储系统HDFS和分布式批处理平台在推荐中的作用有哪些？
- 请简述offline/nearline/online训练方法和步骤。
#### 性能评估
- 请说出几种离线评估的指标。
- 请说出P-R曲线、ROC曲线和AUC的含义和关系。
- 如何巧妙地绘制ROC曲线？
- 线下AUC提升，一定会带来线上指标的提升吗？为什么？
#### AB测试
- 为什么要进行AB测试？相比离线评估的优势是什么？
- AB测试是如何设计分层和分流机制的？

### 冷启动与EE
#### 冷启动
- 当新用户注册或新物品入库的时候，该怎么给用户提供满意的推荐服务，以及怎么将新物品推荐出去，推荐给喜欢他的用户？
#### 探索与利用
- 简述探索与利用的含义。
- Greedy算法的原理是什么？有什么缺陷？
- 请简述Thompson Sampling方法的原理和步骤。
- 请问UCB方法是如何解决冷启动中的探索和利用问题的？
- 简述LinUCB的原理与具体的做法。

