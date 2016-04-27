###分析方法明细表

仅带你到一个正确的出发点是不够的。我们还要让你理解你所看到的。

明白几种可能适用于你的问题的分析技术是非常有用的，但是只提供他们叫什么就起不了太大的作用。分析方法明细表介绍一些这些方法的具体知识。一旦你明确了将一种方法用在分析选择中，就找到表中对应的行。你会找到方法简要的介绍，我们所知的一些建议和一些有用的参考文献。

| Technique（技术）| Description（描述）|Tips from the Pros（Tips）|References we love to read（参考文献）|
| -----|:----:|-----|:----:|
| 主动学习| 通过智能样本选择来提高模型的性能。应当选择能够为学习模型提供最大信息的那些样本|可以和人工参与的循环结合来帮助获取领域知识|Burr, Settles B. “Active Learning: Synthesis Lectures on Artificial Intelligence and Machine Learning.” Morgan & Claypool, 2012. Print.|
| 基于代理人的模拟|模拟具有自主意识个体的行为和交互 | 在很多系统中，复杂行为是由令人惊讶的简单规则导致的。逐步建立代理，并让其保持简单的逻辑 | Macal, Charles, and Michael North. “Agent-based Modeling and Simulation.” Winter Simulation Conference. Austin, TX. 2009. Conference Presentation.|
|方差分析|用于对两组以上数据之间的差异进行假设检验|在使用模型前先检验假设，进行多重检验时留意家族模样差别（FWE）|Bhattacharyya, Gouri K., and Richard A. Johnson. Statistical Concepts and Models. Wiley, 1977. Print.|
|Apriori关联挖掘|用于发现频繁项集的一种数据挖掘技术|用于帮助了解元素之间的潜在关系|Agrawal, Rakesh, and Ramakrishnan Srikant. “Fast Algorithms for Mining Association Rules.” Proc. Of 20th Intl. Conf. on VLDB. 1994. Conference Presentation.|
|贝叶斯网络|对条件概率进行建模，可以看成一个有向无环图|使用更大模型前先手算理解原理|Russel, Stuart, and Peter Norvig. “Artificial Intelligence: A Modern Approach.” Prentice Hall, 2009 Print.|
|协同过滤|也被称为“推荐”，通过比较用户对物品的表现来建议或者取消物品。基于相似的物品或者相似的人所使用的物品来进行推荐。|当所解问题存在潜在的因素时（比如在电影领域），使用奇异值分解。|Owen, Sean, Robin Anil, Ted Dunning, and Ellen Friedman. Mahout in Action. New Jersey: Manning, 2012. Print.|
|坐标转换|通过不同视角观察数据|改变数据坐标系统，例如使用极坐标或柱面坐标，可以更重点地突出数据结构。坐标变换过程中的关键一步是保持数据的多维性，及系统分析数据子空间。|Abbott, Edwin A., Flatland: A Romance of Many Dimensions. United Kingdom: Seely & Co., 1884. Print.|
|深度学习|通过学习低层特征形成更加高级的学习的方法。经常表现为层级较多的神经网络。|利用GPU来有效地训练这一复杂模型|Bengio, Yoshua, and Yann LeCun. “Scaling Learning Algorithms towards AI.” Large- Scale Kernel Machines. New York: MIT Press, 2007. Print.|
|实验设计|采取可控实验以量化输入对输出的影响|部分因子设计可以显著减少不同类型的实验数量|Montgomery, Douglas. Design and Analysis of Experiments. New Jersey: John Wiley & Sons, 2012. Print.|
|微分方程|用于描述函数与导数之间的关系。例如随时间改变的关系。|微分方程可用于构造模型并做出预测。方程本身可以进行数值求解，并以不同的初始条件进行测试达到研究系统轨迹的目的。|Zill, Dennis, Warren Wright,and Michael Cullen. Differential Equations with Boundary-Value Problems. Connecticut: Cengage Learning, 2012. Print.|
|离散事件仿真|模拟事件的离散序列，其中每个事件只在特定的时间点发生。模型只在时间发生的时间点更新。|在分析基于事件的过程时，如生产线和服务中心需要确定不同的工艺参数变化对系统的影响，离散事件仿真是有用的。将优化和仿真结合可以提高提高效率。|Burrus, C. Sidney, Ramesh A. Gopinath, Haitao Guo, Jan E. Odegard and Ivan W. Selesnick. Introduction to Wavelets and Wavelet Transforms: A Primer. New Jersey: Prentice Hall, 1998. Print.|
|离散小波变换|将时间序列数据转换到频域并保存原始信息|提供了一种很好的时频局部化特性。傅立叶变换的优点是保留了频域和局部性|Burrus, C.Sidney, Ramesh A. Gopinath, Haitao Guo, Jan E. Odegard, and Ivan W. Selesnick. Introduction to Wavelets and Wavelet Transforms: A Primer. New Jersey: Prentice Hall, 1998. Print.|
|学习集成|学习多个模型，并将其输出结果组合起来以获取更好的性能|不要设置过多的模型参数和过度训练，否则会造成过拟合。|Dietterich, Thomas G. “Ensemble Methods in Machine Learning.” Lecture Notes in Computer Science. Springer, 2000. Print.|
|专家系统|使用符号逻辑去推理事实。模拟人类推理过程。|以人类易懂的解释为什么系统得出结论|Shortliffe, Edward H., and Bruce G. Buchanan. “A Model of Inexact Reasoning in Medicine.” Mathematical Biosciences. Elsevier B.V., 1975. Print.|
|指数平滑|用于去除由采集误差或异常值带来的失真|相比于使用移动平均方法对过去观测值的几何平均，指数平滑方法处理时对每个值分配一个随时间衰减的权重。|Chatfield, Chris, Anne B. Koehler, J. Keith Ord, and Ralph D. Snyder. “A New Look at Models for Exponential Smoothing.” Journal of the Royal Statistical Society: Series D (The Statistician). Royal Statistical Society, 2001. Print.|
|要素分析|以降低不可观测变量（也就是要素）数量为目的，描述相关变量的可变性。|如果怀疑某些因子对数据有不可估量的影响，那么可以尝试使用因子分析|Child, Dennis. The Essentials of Factor Analysis. United Kingdom: Cassell Educational, 1990. Print.|
|快速傅立叶变换|有效地将时间序列从时域转换到频域，也可以通过空间变换来进行图像增强。|在频域中可以更有效地过滤时变信号。此外，噪声常可以通过观察在异常频率点的信号强度确定。|Mitra, Partha P., and Hemant Bokil. Observed Brain Dynamics. United Kingdom: Oxford University Press, 2008. Print.|
|格式转换|创建一个标准的数据表现方式而不用考虑原始数据格式。例如，从微软Word或者PDF中（2进制文件）抽取raw UTF-8数据。|有很多开源软件支持数据格式转换，并且支持很多不同的格式。一个好用的软件包就是Apache Tikia。|Ingersoll, Grant S., Thomas S. Morton, and Andrew L. Farris. Taming Text: How to Find, Organize, and Manipulate It. New Jersey: Manning, 2013. Print.|
|模糊逻辑|允许描述真实性等级的逻辑推理|当类别没有清晰定义时使用。例如“暖”、“冷”、“热”等概念在不同的温度和情况下有不同的含义。|Zadeh L.A., "Fuzzy Sets.” Information and Control. California: University of California, Berkeley, 1965. Print.|
|高斯过滤|删除噪声或者模糊数据|可用于从图像中去除色斑数据|Parker, James R. Algorithms for Image Processing and Computer Vision. New Jersey: John Wiley & Sons, 2010. Print.|
|广义线性模型|当误差不是正态分布时，允许把普通线性模型扩展为广义模型|当系统中的观测误差不服从正态分布时使用|MacCullagh, P., and John A. Nelder. Generalized Linear Models. Florida: CRC Press, 1989. Print.|
|遗传算法|通过改变操作和参数变化引起逐代进化改进候选模型|在考虑参数组合时，增加代数会加大多样性，但是需要更多的目标函数评估。在一代中计算个体数可以同时进行。候选解决方案的描述能影响表现。|De Jong, Kenneth A. Evolutionary Computation - A Unified Approach. Massachusetts: MIT Press, 2002. Print.|
|网格搜索|对参数探索问题的离散值进行系统搜索|网格参数用于参数可视化及评估是否存在多个极小值|Kolda, Tamara G., Robert M. Lewis, and Virginia Torczon. “Optimization by Direct Search: New Perspectives on Some Classical and Modern Methods.” SIAM Review. Society for Industrial and Applied Mathematics, 2003. Print|
|隐马尔可夫模型|通过确定离散隐含变量对序列数据建模，但可观测量可能是连续或者离散的。|隐马尔科夫模型一个最强大的特点是展现一定程度的局部变换（压缩或者延伸）时不变性。然而，它的一个明显缺点是它描述系统在一个给定状态下保持不变的时间分布。|Bishop, Christopher M. Pattern Recognition and Machine Learning. New York: Springer, 2006. Print.|
|层次聚类|基于连通性的聚类方法，在数据集中依次建立更大（凝聚）或更小（分裂）的聚簇。|按数据的亲密程度形成聚簇。在解决数据量较大的问题时，算法的复杂度为O(N2)或O(N3)|Rui Xu, and Don Wunsch. Clustering. New Jersey: Wiley- IEEE Press, 2008. Print.|
|KMeans XMeans|基于质心的聚类算法，K表示聚簇个数，X表示事先不知道聚簇个数。|应用这个聚类技术时，一定要先了解数据的形状。如果数据不是圆形或者椭圆形，这一技术的返回结果将比较差。|Rui Xu, and Don Wunsch. Clustering. New Jersey: Wiley- IEEE Press, 2008. Print.|
|线性规划，非线性规划，整数规划|在一组受约束输入参数的条件下最大化或最小化函数优化技术|先尝试线性规划，因为整数和非线性规划会运行较长时间。|Winston, Wayne L. Operations Research: Applications and Algorithms. Connecticut: Cengage Learning, 2003. Print.|
|MCMC采样|一种通过贝叶斯模型来估计给定数据联合分布参数的抽样方法|在解决高维度问题时，如果使用MCMC进行采样，那么棘手的问题可以变得易处理。可追溯性是对潜在关系进行统计的结果，也就是说，利用蒙特卡罗进行采样，同时考虑到马尔可夫链的随机顺序过程。|Andrieu, Christophe, Nando de Freitas, Amaud Doucet, and Michael I. Jordan. “An Introduction to MCMC for Machine Learning.” Machine Learning. Kluwer Academic Publishers, 2003. Print.|
|蒙特卡罗算法|用于生成随机数的算法|在数值积分、求解微分方程、计算贝叶斯后验概率、高维多元抽样等应用中比较有用。|Fishman, George S. Monte Carlo: Concepts, Algorithms, and Applications. New York: Springer, 2003. Print.|
|朴素贝叶斯|根据贝叶斯理论，一组特征出现的概率基于给定特征出现某种结果的概率。|该模型假设变量是相互独立的，所以它在解决变量高度依存的问题时存在问题。它能够在一次数据统计后就建立模型，所以当面对大数据集的时候能够以较少的开发时间来确定可能的模式是否存在。|Ingersoll, Grant S., Thomas S. Morton, and Andrew L. Farris. Taming Text: How to Find, Organize, and Manipulate It. New Jersey: Manning, 2013. Print.|
|人工网络|通过调整节点间的权重来学习数据中突出的特征并形成一个学习规则。|训练一个人工网络比利用现有模型去推断新的数据更加耗时。稀疏的网络连接能够帮助提告高分类性能。|Haykin, Simon O. Neural Networks and Learning Machines. New Jersey: Prentice Hall, 2008. Print.|
|离群点移除|从数据中识别及移除噪声的方法|删除离群点时要谨慎。有时，一个系统的最有趣行为就是异常数据点的存在。|Maimon, Oded, and Lior Rockach. Data Mining and Knowledge Discovery Handbook: A Complete Guide for Practitioners and Researchers. The Netherlands: Kluwer Academic Publishers, 2005. Print.|
|主成分分析|通过识别高度相关的维度来降维|许多大数据集包含维度之间的相关性，因此部分数据是多余的。当分析主成分时，按照方差的顺序来排序，因为方差是数据的最高级信息视角。采用skree图来推断最优的主成分的个数。|Wallisch, Pascal, Michael E. Lusignan, Marc D. Benayoun, Tanya I. Baker, Adam Seth Dickey, and Nicholas G. Hatsopoulos. Matlab for Neuroscientists. New Jersey: Prentice Hall, 2009. Print.|
|随机搜索|随机调整参数来发现一个比现有模型更好的解决方案|它被用作评判一个搜素算法好坏的一个标准。注意使用一个较好的随机数生成器和新的种子。|Bergstra J. and Bengio Y. Random Search for Hyper- Parameter Optimization, Journal of Machine Learning Research 13, 2012.|
|Lasso算法|变量选择和预测与一个可能有偏差的线性模型相结合的方法|有很多不同的方法去选择lambda参数。一个典型的选择方法是通过均方差来进行交叉验证。|Tibshirani, Robert. “Regression Shrinkage and Selection via the Lasso.” Journal of the Royal Statistical Society. Series B (Methodological). Toronto: Royal Statistical Society, 1996. Print.|
|敏感性分析|包含分析或者模型中的检验单个参数，观察影响程度。|将不敏感的参数作为常量的候选，这样可以减少优化问题的维度，并提供一个算法加速的机会。|Saltelli, A., Marco Ratto, Terry Andres, Francesca Campolongo, Jessica Cariboni, Debora Gatelli, Michaela Saisana, and Stefano Tarantola. Global Sensitivity Analysis: the Primer. New Jersey: John Wiley & Sons, 2008. Print.|
|模拟退火|退火是冶金工业控制的冷却过程的专有名词，并通过类比，使用温度变化或退火时间表来改变算法的收敛性。|标准的“退火”功能允许开始时广泛探索参数空间，然后在更小范围内搜索。依赖于搜索的优先级，“退火”功能可以在更高温度时进行更长时间的探索性搜索。|Bertsimas, Dimitris, and John Tsitsiklis. “Simulated Annealing.” Statistical Science. 1993. Print.|
|逐步回归|一种变量选择和预测方法。将Akaike信息准则AIC作为选择度量。由此产生的预测模型是基于普通最小二乘法或基于极大似然的一般线性参数估计。|在考虑使用逐步回归时，必须要谨慎，因为过拟合经常发生。通过限制自由变量的数目来减少过度拟合的可能。|Hocking, R.R. “The Analysis and Selection of Variables in Linear Regression.” Biometrics. 1976. Print.|
|随机梯度下降|用于优化神经网络、支持向量机、逻辑回归模型|在使用子梯度时当目标函数不是绝对可微时使用。|Witten, Ian H., Eibe Frank,  and Mark A. Hall. Data Mining: Practical Machine Learning Tools and Techniques. Massachusetts: Morgan Kaufmann, 2011. Print.|
|支持向量机|衡量语料库中一个词的相对重要性的一种方法|尝试使用不同的核函数，并用k折交叉验证来验证选取的最好模型|Hsu, Chih-Wei, Chih-Chung Chang, and Chih-Jen Lin. “A Practical Guide to Support Vector Classification.” National Taiwan University Press, 2003. Print.|
|TF-IDF|衡量语料库中一个词的相对重要性的一种方法|通常用于文本挖掘。假设在一个新闻题材的语料库中，"the"这个词可能出现在多篇文章中，但是它具有很低的价值。一个比较罕见的术语，比如某个人名只出现在一个单一的文章中，那么将获得很高的tfidf分值。|Ingersoll, Grant S., Thomas S. Morton, and Andrew L. Farris. Taming Text: How to Find, Organize, and Manipulate It. New Jersey: Manning, 2013. Print.|
|LDA主题模型|通过单词共现来确定文中的潜在主题|使用词性标注除名词和动词以外的其他词。使用原始的次计数代替TF/IDF|Blei, David M., Andrew Y. Ng, and Michael I. Jordan. “Latent Dirichlet Allocation.” Journal of Machine Learning Research. 2003. Print.|
|树模型|模型的结构与树结构一致，分支表明决策。|可用于处理一个过程，或者作为一个分类器。|James, G., D. Witten, T. Hastie, and R. Tibshirani. “Tree Based Methods.” An Introduction to Statistical Learning. New York: Springer, 2013. Print.|
|T校验|检验两个组差异的假设检验。|确保符合测试假设，并在运行多个测试时观察多重比较误差|Bhattacharyya, Gouri K., and Richard A. Johnson. Statistical Concepts and Models. Wiley, 1977. Print.|
|Wrapper Methods|通过某个模型中一组特征的表现来进行降维。通过特征组合来提高模型性能|使用k折交叉验证来控制过拟合|John, George H., Ron Kohavi, and Karl Pfleger. “Irrelevant Features and the Subset Selection Problem.” Proceedings of ICML-94, 11th International Converence on Machine Learning. New Brunswick, New Jersey. 1994. Conference Presentation.|