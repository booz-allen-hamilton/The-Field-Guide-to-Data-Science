### 分析方法选择指南

由于你无法凭感觉准确认知整个数据科学领域，所以我们为你绘制了一个导图。

分析技术这个领域是无比广阔的，也是很难理解的。我们用下面这个图来帮助你找到分析数据的方法。首先，我们回答如何认知分析目标及确认问题特征等相关问题。这些答案将引导你了解数据分析技术，并对相关技术做一些思考。

![](http://i2.piimg.com/13f1b78d257d7bdc.png)

1.有很多原因需要我们进行数据降维：

- 模型不收敛

- 模型输出的结果相当于随机结果

- 在当前多维度特征空间中，无法获取足够的计算资源以完成特定目标

- 不知道数据的哪方面是最重要的

2.__特征提取__是一个广泛的话题，并且与具体问题高度相关，这一主题展开说可以独自成书。所以我们将其从该图中删除。请参阅战壕的生活中的特征工程和特征选择章节。

3.应当检查数据标签的正确性，尤其是时间戳，因为它很可能恢复成系统默认值。

4.巧妙的丰富可以极大提高计算时间，也可能成为在不同的端到端分析解决方案之间的巨大差异。


- DESCRIBE 描述：通过何种方式去认识数据？
	- PROCESSING 处理:如何进行数据清洗？
		- FILTERING: 过滤  
		如何根据绝对或者相对值识别数据？
			- 如果你想基于自身的值添加或者删除数据，
				- Relational algebra projection and selection 可以利用关系代数投影和选择
			- 如果原始数据是无信息或者重复的，可以考虑：
				- Outlier removal 去除离群点
				- Gaussian filter 高斯过滤
				- Exponential smoothing 指数平滑
				- Median filter 均值过滤
		- IMPUTATION: 缺失值填充  
		如何填充缺失值？
			- 如果从数据集中该特征的其他值来确定缺失值
				- Random sampling 随机采样
				- Markov Chain Monte Carlo (MC) MCMC 采样法
			- 如果不通过其他观测值来确定缺失值，可通过
				- Mean 均值
				- Regression models 回归
				- Statistical distributions 统计概率分布
		- DIMENSIONALITY RDDUCTION:降维  
		如何降低维度？
			- 如果需要判断是否存在多维相关
				- PCA and other factor analysis PCA 主成分分析或其他因素分析方法
			- 如果能够以一个组内的关系单独观察，从如下开始：：
				- K-Means 聚类
				- Canopy 聚类
			- 如果是非结构化的文本数据
				- Term Frequency/Inverse Document Frequency (TF IDF)
			- 如果现有算法只能使用特定数量的特征，而现有特征比较多：
				- Feature hashing 特征散列
			- 如果不确定哪个特征比较重要：
				- Wrapper methods Wrapper 方法
				- Sensitivity analysis 灵敏度分析
			- 如果需要增加对于当前数据空间概率分布的理解
				- Self organizing maps
		- NORMALIZATION & TRANSFORMATION 标准化
		如何对数据去除重复数据？
			- 如果怀疑数据元素重复
				- Deduplication 重复数据删除 
			- 如果希望数据取值在某个特定区间
				- Normalization 数据标准化 
			- 如果数据以二进制存储
				- Format Conversion 格式化转换
			- 如果在频域进行计算
				- Fast Fourier Transform (FFT) 快速傅立叶变换(FFT)
				- Discrete wavelet transform 离散小波变换
			- 如果在欧几里德空间进行计算
				- Coordinate transform 坐标变换
		- FEATURE EXTRACTION:特征抽取
	- 聚合 如何收集和总结数据?
		- 如果对数据集不熟悉，从基本的统计学开始: 
			- Count 计数
			- Mean 平均
			- Standard deviation 标准差
			- Range 范围
			- Box plots 直方图
			- Scatter plots 散点图
		- 如果方法假设数据服从某个分布: 
			- Distribution fitting 分布拟合
		- 如果想理解数据所有可用信息:
			- Baseball card” aggregation “棒球卡”式聚合
	- 丰富 如何往数据中添加信息?
		- 如果需要跟踪源信息或者其他用户定义的参数:
			- Annotation 标注
		- 如果某些数域需要一起处理，或者使用一个数域计算其他域的值:
			- Relational algebra rename 相关代数
			- Feature addition 特征增加(例如地理、气候、天气)

- DISCOVER 探索 数据中的关键关系是什么？
	- CLUSTERING 聚类:如何发现数据自然分组？
		- 如果希望按某种层次来对数据进行聚类：
			- Hierachical 层次聚类法
		- 如果已知聚簇个数：
			- X-Means 算法
			- Canopy 算法
			- Apriori 算法
		- 如果是文本数据：
			- Topic modeling 主题模型
		- 如果想获取任意形状的聚簇：
			- Fractal 聚类
			- DB Scan 聚类
		- 如果希望获取聚簇内数据的软关系：
			- Gaussian mixture models 高斯混合模型
		- 如果不知道聚簇个数：
			- k-Means(通过 Canopy 或者层次聚类来获取聚类个数)
	- Regression 回归: 如何确定哪个变量比较重要？
		- 如果数据具有未知结构：
			- Tree-based methods 基于树结构的一系列方法
		- 如果比较重视统计衡量方法的重要性：
			- Generalized linear models 广义线性模型
		- 如果不侧重统计衡量方法的重要性：
			- Regression with shrinkage (e.g., LASSO, Elastic net) 收缩回归
			- Stepwise regression Stepwise 回归
	- HYPOTHESIS TESTING 假设检验: 如何验证算法？
		- 如果想比较两组结果的差别：
			- T-test T 校验
		- 如果想比较多组的结果的差别：
			- ANOVA
- PREDICT 预测: 可能的输出结果会是什么？
	- CLASSIFICATION 分类 如何预测组关系？
		- 如果已知变量间的依赖关系: 
			- Bayesian network 贝叶斯网络
		- 如果不知道特征重要性: 
			- Neural nets 人工网络
			- Random forests 随机森林
			- Deep learning
		- 如果需要高度透明的模型: 
			- Decision trees 决策树
		- 如果维度小于 20: 
			- K-nearest neighbours K 近邻算法
		- 如果待分类的数据量较大: 
			- Native Bayes 朴素贝叶斯
		- 如果想通过已观测值来预测未观测值: 
			-  Hidden markov model 隐马尔可夫模型
		- 如果上述步骤后还是不知道如何开始: 
			- Support vector Machine(SVM) 支持向量机
			- Random forests 随机森林
	- REGRESSION 回归 如何预测一个未知量？
		- 如果数据结构未知: 
			- Tree-based methods 基于树结构的一系列方法
		- 如果比较重视统计衡量方法的重要性: 
			- Generalized linear models 广义线性模型
		- 如果维度小于 20: 
			- K-nearest neighbours K 近邻算法
	- RECOMMENDATION 推荐 
		- 如果你仅仅知道人与物品之间是如何互动的: 
			- Collaborative filtering 协同过滤
		- 如果知道物品本身的特征向量: 
			- Content-based methods 基于内容的方法
		- 如果你只知道物品间相互联系: 
			- Graph-based methods 基于图形的方法
- ADVISE 建议: 应该采取什么样的行动？
	- LOGICAL REASONING 逻辑推理 如何通过不同的证据进行推断
		- 如果你有专业的知识: 
			- Expert systems 专业系统
		- 如果你只需要基本事实: 
			- Logical reasoning 逻辑推理
	- OPTIMIZATION 优化 	
	 - 当目标可表达成一个效用函数，如何找到最好的行动方针？
		- 如果问题是由非确定性效用函数来表示: 
			- Stochastic search 随机搜索
		- 如果近似解是可以接受的: 
			- Genetic algorithms 遗传算法
			- Simulated annealing 模拟退火
			- Gradient search 梯度搜索
		- 如果问题是由确定性效用函数来表示: 
			- Linear programming 线性规划
			- Integer programming 整数规划
			- Non-linear programming 非线性规划
		- 如果你想尝试多种模式: 
			- Ensemble learning 集成学习
	- SIMULATION 模拟 如何通过不同的证据进行推断
		- 如果需要建立离散实体模型: 
			- Discrete event simulation (DES) 离散事件仿真
		- 如果有一组离散可能的状态: 
			- Markov models 马尔可夫模型
		- 如果有独立的实体之间的动作和互动: 
			- Agent-based simulation 代理人基模型
		- 如果不需要离散实体模型: 
			- Monte Carlo simulation 蒙特卡罗模拟
		- 如果正在模拟一个反馈机制与执行之间的复杂系统: 
			- Systems dynamics 系统动力学
		- 如果需要持续跟踪系统行为: 
			- Activity-based simulation 基于活动的模拟
		- 如果你了解什么样的因素驱动系统: 
			- ODES
			- PDES
		- 如果类别不准确: 
			- Fuzzy logic 模糊逻辑

<br/>