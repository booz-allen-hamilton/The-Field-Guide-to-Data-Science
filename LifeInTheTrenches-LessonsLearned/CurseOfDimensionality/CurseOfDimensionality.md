The Curse of Dimensionality
=============
*There is no magical potion to cure the curse, but there is PCA.*

The “curse of dimensionality” is one of the most important results in machine learning. Most texts on machine learning mention this phenomenon in the first chapter or two, but it often takes many years of practice to understand its true implications.

Classification methods are subject to the implications of the curse of dimensionality. The basic intuition in this case is that as the number of data dimensions increases, it becomes more difficult to create generalizable classification models (models that apply well over phenomena not observed in the training set). This difficulty is usually impossible to overcome in real world settings. There are some exceptions in domains where things happen to work out, but usually you must work to minimize the number of dimensions. This requires a combination of clever feature engineering and use of dimensionality reduction techniques (see Feature Engineering and Feature Selection Life in the Trenches). In our practical experience, the maximum number of dimensions seems to be ~10 for linear model-based approaches. The limit seems to be in the tens of thousands for more sophisticated methods such as support vector machine, but the limit still exists nonetheless.

A counterintuitive consequence of the curse of dimensionality is that it limits the amount of data needed to train a classification model. There are roughly two reasons for this phenomenon. In one case, the dimensionality is small enough that the data is small enough to train the model on a single machine. In the other case, the exponentially expanding complexity of a high-dimensionality problem makes it (practically) computationally impossible to train a model. In our experience, it is quite rare for a problem to fall in a “sweet spot” between these two extremes. 

This observation is not to say that such a condition never arises. We believe it is rare enough, however, that practitioners need not concern themselves with how to address this case. Rather than trying to create super-scalable algorithm implementations, focus your attention on solving your immediate problems with basic methods. Wait until you encounter a problem where an algorithm fails to converge or provides poor cross-validated results, and then seek new approaches. Only when you find that alternate approaches don’t already exist, should you begin building new implementations. The expected cost of this work pattern is lower than over-engineering right out of the gate. 

Put otherwise, “Keep it simple, Stupid”.

