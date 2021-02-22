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

问题目录
### 1. 浅层模型篇
- 请简述基于用户的协同过滤UserCF的推荐过程。
- 在基于用户的协同过滤中，如何计算用户的相似度？
- 基于用户的协同过滤UserCF存在哪些缺陷？
- 请简述基于物品的协同过滤ItemCF的推荐过程。
- UserCF和ItemCF分别适用于哪些应用场景？为什么？
- 协同过滤算法存在哪些缺陷？
- 矩阵分解的原理是什么？求解的主要方法有哪些？
- 如何从深度学习模型的角度来认识矩阵分解模型
- 矩阵分解算法中，隐向量的长度$k$的取值是如何影响效果和工程开销的？
- 请简述奇异值分解的过程。奇异值分解存在什么缺陷？为什么不适用于互联网场景下的求解？
- 请简述梯度下降法求解用户-物品隐向量的过程。
- 如何解决矩阵分解中用户和物品打分偏差的问题？
- 矩阵分解有哪些优点与缺点？与协同过滤相比较呢？
- 如何从神经网络的角度理解矩阵分解？
- 逻辑回归模型预估相较于协同过滤，最大的优势是什么？其推荐过程是怎么样的？
- 请推导逻辑回归的数学形式。
- 请推导梯度下降法求解逻辑回归参数更新的过程。
- 逻辑回归作为CTR预估模型的优势与缺陷是什么？
- 所有的特征进行两两交叉，并对所有的的组合赋予权重的方法存在什么缺陷？
- FM的原理是什么？与矩阵分解有什么联系？
- FM相较于POLY2为什么泛化能力更好？在工程上有什么优势？
- FFM相较于FM有什么改进？
- FM的训练复杂度是多少？怎么推导？FFM的训练复杂度是多少？
- 为什么GBDT可用于特征选择和特征组合？
- GBDT+LR组合模型中，GBDT是如何生成特征向量的？
- GBDT+LR有什么优点和缺陷？
- 请简述阿里妈妈提出的LS-PLM模型的原理与数学形式。
- LS-PLM模型的优势有哪些？
- LS-PLM模型与深度学习模型有什么联系？

### 2. 深度模型篇
- 请简述Deep Crossing的网络结构。
- Deep Crossing中的残差单元有什么作用？
- NeuralCF在矩阵分解模型的基础上，做了哪些改进？
- 模型结构越复杂越好吗？特征越多越好吗？
- PNN相较NeuralCF和Deep Crossing有哪些改进？优势是什么？
- PNN中特征交叉有哪些方式？分别是怎么样的？
- PNN模型的优势和局限性是什么？
- 如何理解Wide&Deep模型的泛化能力和记忆能力？
- 请简述Wide&Deep的模型结构。
- Wide&Deep模型的创新和优势是什么？
- Deep&Cross相比Wide&Deep作了哪些改进？Deep&Cross模型的Cross网络是怎么操作的？
- FNN模型的提出主要是为了解决什么问题？它是如何解决的？
- FNN的模型结构是什么样的？
- FNN模型中是如何使用FM来初始化Embeddiing层参数的？
- DeepFM相较于Wide&Deep有什么改进？为什么这么改进？
- NFM相比Wide&Deep有什么改进？为什么这么改？
- AFM的网络结构是什么样的？
- AFM模型为何要在推荐系统模型中引入注意力机制？是如何引入注意力机制的？
- DIN的结构是怎样的？是如何引入注意力机制的？动机是什么？
- DIEN引入序列信息的动机是什么？
- 请绘制DIEN各层的结构？兴趣抽取层和兴趣进化层。
- 请说明ESSM模型的多目标优化设计的动机，以及是怎么做的？

### 3. Embedding篇
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

### 4. 特征工程篇
- 让你设计一个推荐系统的特征工程，你会怎么去设计？包括用户侧、物品侧和上下文特征。
- 在进行特征处理时，对连续型特征怎么处理？
- 在进行特征处理时，对类别型特征怎么处理？

### 5. 召回系统篇
- 假设物品库数量达到百万级别，如何设计方法从这个数量级别的物品中推荐给用户top10的物品，同时可以减少计算的压力？
- 推荐系统中为什么要有召回？在推荐系统中召回和排序有什么异同？
- 请举例说明一些简单的多路召回策略。
- 请简述基于embedding的召回方法，优势是什么？
- 请简要描述DSSM是如何应用于召回的？结构是怎样的？
- 请简述YoutubeDNN的结构和其原理
- 请简述用户多兴趣网络MIND的出发点是什么，描述其结构？
- SDM是如何结合用户长期和短期兴趣建模的？其结构如何？
- TDM 深度树匹配召回

### 6. 性能与评估篇
- 模型的实时性是如何影响推荐系统的效果的？
- 客户端是如何做到对于实时特征进行实时推荐的？
- 流计算平台是如何进行准实时特征处理的？
- 分布式存储系统HDFS和分布式批处理平台在推荐中的作用有哪些？
- 请简述offline/nearline/online训练方法和步骤。
- 请说出几种离线评估的指标。
- 请说出P-R曲线、ROC曲线和AUC的含义和关系。
- 如何巧妙地绘制ROC曲线？
- 线下AUC提升，一定会带来线上指标的提升吗？为什么？
- 为什么要进行AB测试？相比离线评估的优势是什么？
- AB测试是如何设计分层和分流机制的？

### 7. 冷启动与EE
- 当新用户注册或新物品入库的时候，该怎么给用户提供满意的推荐服务，以及怎么将新物品推荐出去，推荐给喜欢他的用户？
- 简述探索与利用的含义。
- Greedy算法的原理是什么？有什么缺陷？
- 请简述Thompson Sampling方法的原理和步骤。
- 请问UCB方法是如何解决冷启动中的探索和利用问题的？
- 简述LinUCB的原理与具体的做法。


## :art: 机器学习

### 逻辑回归
- 推导一下逻辑回归的损失函数，并解释其含义。
- 在广告LR模型中，为什么要做特征组合？
- 为什么 LR 模型要使用 sigmoid 函数，背后的数学原理是什么？为什么不用其他函数？
- 为什么LR可以用来做点击率预估？
- 满足什么样条件的数据用LR最好？换句话说，为了LR工作的更好，要对数据做一些什么处理？
- 逻辑斯蒂回归能否解决非线性分类问题？
- 给一个有m个样本n维特征的数据集，LR算法中梯度的维度是多少?
- 逻辑回归损失函数为什么使用最大似然估计而不用最小二乘法？
- 如何求解逻辑回归的参数？
- SVM 和 LR 有什么异同？分别在什么情况下使用？
- 为什么LR不适合用MSE？
- 为什么逻辑回归需要先对特征离散化？
- 并行LR的实现
- 逻辑回归（Logistic regression）在金融领域有什么应用呢？
### 贝叶斯
- 怎么简单理解贝叶斯公式？如何推导朴素贝叶斯分类？
- 贝叶斯学派与频率学派有何不同？
- 朴素贝叶斯分类器和一般的贝叶斯分类器有什么区别？
- 极大似然估计法推出朴素贝叶斯法中的先验概率估计公式？
- 为什么朴素贝叶斯分类中引入的拉普拉斯修正是正确的？
- 举个实例说明朴素贝叶斯是如何分类的。
- 逻辑回归与朴素贝叶斯有什么区别？
### 决策树
- 决策树节点分裂时如何选择特征？他们的区别和使用条件是什么？写出Gini index和Information Gain的公式并举例说明
- cart算法为什么选用gini指数？
- 为什么信息增益可以用来选特征？简述信息熵和基尼指数的关系。c4.5为什么使用信息增益比来选择特征？
- 决策树算法中，CART与ID3、C4.5特征选择之间的区别会对实际应用有哪些影响？哪种的结果会更好些？
- 为什么C4.5决策树克服了ID3决策树偏向选择取值较多的属性（特征）的这一问题？
- 决策树是如何处理连续值和缺失值的？
- 如何计算决策树的各特征重要程度？
- 如何理解决策树的损失函数?
- sklearn中的决策树是否应该用one-hot编码？
- 既然使用神经网络也可以解决分类问题，那SVM、决策树这些算法还有什么意义呢？
- 分类树和回归树的区别是什么？
### 随机森林
- 请解释随机森林算法的细节。
- 随机森林中每一棵树的特征是怎么选取的？
- 随机森林树的深度和模型复杂度有关吗？随机森林是否会出现过拟合？
- 随机森林是否需要后剪枝？
- 随机森林为什么不用分训练集和测试集？
- 怎么理解决策树、xgboost能处理缺失值？而有的模型(svm)对缺失值比较敏感呢?
### GBDT
- 请简述GBDT的原理
- 机器学习算法中GBDT与Adaboost的区别与联系是什么？
- 机器学习算法中 GBDT 和 XGBOOST 的区别有哪些？
- gbdt的残差为什么用负梯度代替？
- 梯度提升树中为什么说目标函数关于当前模型的负梯度是残差的近似值？
- 为什么xgboost/gbdt在调参时为什么树的深度很少就能达到很高的精度？
- 为什么在实际的kaggle比赛中，GBDT和Random Forest效果非常好？
- GBDT怎么用在点击率预测中？
- GBDT中的梯度怎么计算的？是谁对谁的梯度？
- m×n数据集，如果用GBDT，那么梯度是几维？或者是与树的深度有关？或者与树的叶子节点的个数有关？
- 随机森林和GBDT的异同点
### XGBoost
- 请推导一下Xgboost
- XGBoost算法防止过拟合的方法有哪些？
- 使用XGBoost训练模型时，如果过拟合了怎么调参？
- XGBoost的正则项是什么？
- XGBoost为什么对缺失值不敏感？XGBoost怎么处理缺失值？
- XGBoost中的一棵树的停止生长条件是什么？
- XGBoost可以做特征选择，它是如何评价特征重要性的？
- XGBoost如何选择最佳分裂点？
- XGBoost的延展性很好，怎么理解？
- XGBoost的正则化是如何实现的?
- XGBoost的并行化部分是如何实现的?
- XGBoost是如何求Hessian矩阵逆的？
- xgboost里叶子节点的score或weight是怎么得到的？
- 为什么 Xgboost中树的叶节点得分可以用来衡量树的复杂度？
- xgboost算法中使用近似算法求取分割点如何理解？
### LightGBM
- LightGBM相较于XGBoost有什么优缺点？
### 聚类
### SVM
- 关于SVM中，对常数C的理解？
- 机器学习SVM中关于函数间隔为什么可以设置为1？
- 机器学习有很多关于核函数的说法，核函数的定义和作用是什么？
### 降维
### 优化算法
- 什么是梯度下降法？
- 用梯度下降训练 SVM 会有什么问题？
- 最小二乘、极大似然、梯度下降有何区别？
- 最优化问题中，牛顿法为什么比梯度下降法求解需要的迭代次数更少？
- 为什么nn的较大问题是会陷入局部最优时，不选用凸函数作为激活函数？
### 损失函数
- 对于逻辑回归，为什么说平方损失函数是非凸的？
- 如何把SVM的推导和损失函数联系起来？
- 怎么样理解SVM中的hinge-loss？SVM中的正则化和损失是什么？
- 神经网络如何设计自己的loss function，如果需要修改或设计自己的loss，需要遵循什么规则？
- softmax和cross-entropy是什么关系？
- 神经网络的损失函数为什么是非凸的?
- 深度学习中有哪些常用损失函数(优化目标函数)？
- 神经网络中，设计loss function有哪些技巧?
- 对数损失函数是如何度量损失的？
- 神经网络中，为何不直接对损失函数求偏导后令其等于零，求出最优权重，而要使用梯度下降法（迭代）计算权重？
- 在用交叉熵损失函数时，只希望惩罚 0.4~0.6 这样模糊的值，应该怎么改？
### 正则化
- 请解释正则化的含义。
- 请说明正则化与数据先验分布的关系？
- L1 相比于 L2 为什么容易获得稀疏解？
- L1正则为什么能让系数变为0？L1正则怎么处理0点不可导的情形？
- 为什么L1正则可以实现参数稀疏，而L2正则不可以？为什么L1很多系数可以被压缩为0，L2是被压缩至接近于0？
- 深度学习怎么防止过拟合？
- 目标函数中同时使用多个L1和L2正则化项的情况，应该怎么求解？
- 机器学习中的Bias(偏差)，Error(误差)，和Variance(方差)有什么区别和联系？
- 为什么模型复杂度增加时，模型预测的方差会增大，偏差会减小？
### 模型融合
- 为什么说bagging是减少variance，而boosting是减少bias?
### 性能评价
- 请解释一下AUC。
- AUC和准确率一定是正相关的吗？有什么内在关系吗？
- 精确率、召回率、F1 值、ROC、AUC 各自的优缺点是什么？
- 为什么accuracy、precision、f1-score、recall得分都很高但是AUC得分低？
- 机器学习中，F1和ROC/AUC，关于多分类如何做指标评估？
- 如何解决离线和线上auc和线上点击率不一致的问题？
- 为什么AUC对正负样本比例不敏感
- AUC要到多少才算好？
- AUC的概率解释。
### 非平衡数据
- 机器学习中有哪些非均衡数据集的处理方法？
- 数据不均衡对分类模型有什么影响，该怎样降低影响？
- 欠采样（undersampling）和过采样（oversampling）会对模型带来怎样的影响？
### 特征工程
- 机器学习中，有哪些特征选择的工程方法？
- 广告点击率模型中，LR, GBDT+LR, FM, DNN等模型的优点和缺点？实际效果如何?
- 多标签（multi-label）数据的学习问题，常用的分类器或者分类策略有哪些？


## :bulb: Spark

- 请简述RDD的概念，如何创建RDD？
- RDD支持哪些操作？
- RDD支持哪些操作？分别有什么特点？
- 请举例说明RDD转化操作和行动操作
- 说明RDD的惰性求值机制
- 分别说明转换操作map、flatMap、filter、distinct的作用和用法
- 分别说明转化操作union、intersection、subtract、cartesian的作用和用法
- 分别说明行动操作reduce、fold、aggregate的用法及其区别
- 为什么要对RDD进行持久化，请简述不同级别的缓存机制。
- 请简述reduceByKey、groupByKey、combineByKey的作用与区别。
- RDD之间的依赖关系宽依赖和窄依赖的含义与区别
- RDD中Client、Master、Worker、Driver、Executor的含义分别是什么
- DataFrame与RDD的主要区别在于?
- 为什么Spark快于mapreduce？
- Spark有那些组件？
- Spark Streaming的基本原理
- 如何解决Spark中数据倾斜的问题
- 请说明SparkSQL中三种join 1.Broadcast Join 2.Shuffle Hash Join 3.Sort Merge Join的含义与区别
- spark 能代替hadoop 吗？
- Executor 的作用？
- Driver 的作用？
- spark Rdd 的缓存？
- spark spark-submit脚本的参数有哪些？
- 宽依赖和窄依赖
- 总结一下Rdd算子（30个以上）
- coalesce 和 repartition 的区别？
- reduceByKey 和 groupByKey 的区别？
- union 和 intersection 的区别？
- 常用的宽依赖算子和窄依赖算子有哪些？
- DAG 如何划分stage？
- 如何划分 job？
- Spark 持久化的选择？
- 持久化和容错的应用场景？
- 什么是累加器？
- 什么是广播变量？
- 节点和task执行的关系？
-  cluster 模式如何查看日志
- Spark优化？
- 什么是DataFrame？
- Rdd，DataFrame，DataSet的区别？
- spark底层核心RDD的缓存机制、应用场景、如何使用、如何清除缓存
- DAG有向无环图和划分stage


## :floppy_disk: python

- python中list、tuple、dict、set等类型有什么区别?
- 函数传参有哪些形式？分别有什么特点？
- 请解释python的默认参数陷阱问题。
- 请举例说明浅拷贝和深拷贝的区别
- 生成器与迭代器的概念分别是什么？
- 请简述内置函数zip的用法。迭代器的长度不一致时，是如何处理的，有什么替代方案吗？
- 高阶函数map/reduce/filter/sorted的用法分别是怎样的？举例说明。
- 闭包的概念是什么？举例说明。
- 匿名函数有什么好处？请举一个例子说明其用法。
- 装饰器的概念是什么？如何使用？
- 偏函数的概念是什么？如何使用？
- enumerate相比range有什么优势？
- 什么是工厂函数？举例说明。
- 举例说明类属性和实例属性的区别。
- 请实例解释继承和多态的概念。
- 如何设置类内属性的访问限制？
- 如何使用__slots__？
- 定制类__str__，__iter__， __getitem__，__getattr__，__call__分别有什么作用？
- 静态方法、类方法和成员方法有什么区别
- @classmethod, @staticmethod, @property这些都是什么？
- “__init__”和”__new__”的区别是什么？
- 什么是Python自省？
- python是如何进行内存管理的？
- 什么是GIL？
- 请简述python的异常处理机制。
- 你是如何如何定位python程序的bug的？在python中如何实现单步执行？
- assert断言有什么用处？
- 类有哪些内置的属性？
- 元素为字符串的列表如何转变为空格分隔的字符串？
- python中的is操作符是如何进行对比的？
- 请写出匹配邮箱地址的正则表达式。
- python如何传递命令行参数的？
- 如何理解python中的线程？
- 请简述python中的多进程。


## :coffee C++


### 基础
- 变量的作用是什么？创建变量的语法是什么？
- C++中常量的作用是什么？请写出定义常量的两种方式。
- 请举几个C++中预先保留的关键字的例子
- short类型、int类型、long类型和long long类型所占用的内存空间分别是多少？
- sizeof关键字的作用是什么？
- 字符型变量所占的内存空间为多少？它在存储的时候有什么特点？
- 请举几个你常用的C++中的转义字符？
- C++中前置递增和后置递增的区别是？
- 写一个三目运算符的例子？并解释一下。
- switch case语句中break的作用是什么？
- 一个for循环语句中的起始表达式、条件表达式、末尾循环体和循环语句的执行顺序是什么？
- break语句和continue语句的作用是什么？
### 数组
- 数组的特点是什么？如何定义数组？
- 一维数组的名称和其内存地址的关系是什么？
- 如何定义二维数组？二维数组的名称和其内存地址的关系是什么？
### 函数
- 说明形参与实参的含义。
- 值传递的含义是什么？对形参和实参的影响是什么？
- 函数声明的作用是什么？
### 指针
- 指针的作用是什么？指针变量和普通变量的区别是什么？
- 指针所占内存空间有多大？
- 常量指针、指针常量有什么区别？
- 值传递和地址传递有什么区别？
### 结构体
- 如何创建一个结构体？请写出两种方法。
- 如何创建结构体数组？
- 结构体指针如何访问结构体的成员？
- 结构体如何嵌套结构体？举个实例
- 结构体可以作为参数向函数传参吗？
### 内存
- 请简述C++程序在执行时各个内存区块（代码区、全局区、栈区、堆区）的功能特点。
- new操作符的作用是什么？怎么使用？
### 引用
- 引用的作用是什么？其本质是什么？
- 引用在作为函数参数时，和值传递、地址传递有什么区别？
- 常量引用的作用和写法分别是什么？
- 在写函数默认参数时，有什么需要注意的？
### 重载
- 函数重载需要满足什么条件？
### 封装
- 封装的意义是什么？
- 类的成员和行为的访问权限有哪些？分别是什么样的？
- 类和结构体的区别是什么？
- 将成员属性设置为私有的优点是什么？
### 初始化与清理
- 构造函数和析构函数的作用是什么？
- 构造函数语法是什么？构造函数有什么特点?
- 析构函数语法是什么？析构函数有什么特点?
- 构造函数调用规则是什么？
- 请解释C++中的深拷贝与浅拷贝？
- C++中初始化列表语法是什么？
- B类中有对象A作为成员，A为对象成员，当创建B对象时，A与B的构造和析构的顺序是谁先谁后？
- 静态成员的特点是什么？
- 类内的成员变量和成员函数是分开存储的吗？非静态成员变量占用对象空间吗？
- this指针的作用是什么？
- const修饰成员函数会起到什么效果？关键字mutable的作用是什么？
### 友元
- C++中友元的作用是什么？全局函数、类、成员函数作为友元分别是怎么实现的？
### 重载
### 继承
- 继承的方式有哪几种？其权限是什么样的？
- 子类可以继承父类的私有成员吗？
- 父类和子类的构造函数和析构顺序是什么样的？
- 当子类与父类出现同名的成员，如何通过子类对象，访问到子类或父类中同名的数据？
- 菱形继承会带来什么问题？C++中是怎么解决的？
### 多态
- 静态多态和动态多态有什么区别？
- 多态的满足条件和使用条件是什么？
- 多态有什么优点？
- 纯虚函数的意义是什么？语法是什么样的？他和抽象类有什么关系？
- 解释虚析构和纯虚析构的含义、语法及其区别？
### 文件操作
### 模板
- 如何建立函数模板？其作用是什么？需要注意什么？
- 普通函数与函数模板有什么区别？其调用规则是什么？
- 具体化函数模板是为了解决什么问题？
- 类模板的作用是什么？语法是什么样的？与函数模板区别有什么区别？
- 类模板中成员函数创建时机是什么
### 标准库
- 请解释STL中的容器、算法和迭代器。

## :pencil2: 计算广告

- 计算广告的核心问题是什么？
- 请简述点击率、到达率和转化率的概念。
- 请简述ecpm的含义
- 请说明一下CPT/CPM/CPC/CPA计费方式的含义与特点
- OCPX结算有什么优势？含义是什么？
- 搜索广告中查询扩展有哪些匹配方式？举例说明。
- 搜索广告中对于广告放置有哪些要求？
- 广告定价时，为什么要设置市场保留价？
- 请简述广义第二高价的原理。
- 请简述VCG定价的原理，并分析为何它无法作为主流的的定价方式。
- 价格挤压的原理和作用是什么？


## :cloud: 深度学习

- 请写出常用的损失函数，平方损失、交叉熵损失、softmax损失函数和hinge损失函数。
- 为什么深层神经网络的训练的难度很大？主要有哪几方面的原因。
- 请你用实例说明一下前向传播和反向传播
- 在深度学习中引入非线性激活函数的作用是什么？
- 请说出常用的激活函数，并画出他们相应的图像。
- 如何选择激活函数？请说明各种激活函数的特点。
- Relu激活函数的优点是什么？
- 请说明Softmax激活函数的定义及其作用？Softmax激活函数如何应用于多分类？
- 在深度模型训练时，为什么需要batch size?如何选择合适的batch size，对结果有和影响？
- 请说明BN的原理，为什么要进行批归一化？
- 什么是模型微调fine tuning？请说明fine-tuning 模型的三种状态，各自的特点是什么？
- 为什么无监督预训练可以帮助深度学习？
- 权重偏差初始化有哪些方法？分别说明他们的特点。
- 设置学习率的作用是什么？常用的学习率衰减方法有哪些？说明他们各自的特点
- 深度学习中有哪些防止过拟合的方法？
- 请说出几种常用的优化算法，以及他们各自的特点。
- 深度学习中如何平衡方差与偏差？如果偏差过大我们应该怎么做？方差过大呢？
- 请说明Dropout的原理，在训练与测试的时候dropout会有什么区别？
- 深度学习中常用的数据增强方法？
- 如何理解 Internal Covariate Shift？
