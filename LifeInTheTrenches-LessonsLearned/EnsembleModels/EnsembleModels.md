Ensemble Models
===============

**None of us is as smart as all of us, but some are smarter than others.**

In 1906, Sir Francis Galton attended a fair at which there was a contest to guess the weight of an ox. Galton had the idea to collect the guesses of the 787 entrants and compute the mean. To his surprise, the mean was only one pound off from the ox’s real weight of 1,198 pounds. Together, the estimates made by many amateurs formed a prediction that was more accurate than that of individual experts. 

Galton’s “wisdom of crowds” extends to Data Science in the form of ensemble learning, which is colloquially and somewhat equivalently called ensembling, blending, or stacking. An ensemble takes the predictions of many individual models and combines them to make a single prediction. Like the people guessing the ox’s weight, Data Science models have unique strengths and weaknesses (i.e., determined by their design), and are influenced by varied perspectives based on past experience (i.e., the data they have observed). 

Ensembles overcome individual weaknesses to make predictions with more accuracy than their constituent models. These models need not stem from different methodologies; an ensemble might employ the same method with different parameters or weights (e.g., boosting), feature subsets (e.g., random forests), or sub-samples of data (e.g., bagging). The ensembling methodology may be as simple as averaging two outputs, or as complex as using a “meta model” to learn an optimal combination. 

An ensemble’s ability to reduce individual errors arises from the diversity of its members. If one model over fits the data, it is balanced by a different model that under fits the data. If one subset is skewed by outlier values, another subset is included without them. If one method is unstable to noisy inputs, it is bolstered by another method that is more robust. 

In practice, ensembling typically improves a model by a few percent. The price of this accuracy is paid in complexity. The accuracy vs. complexity tradeoff can make it difficult to know when ensembling is justified. On one hand, ensembles appear to be a fit for high-stakes problems—think detecting cancer in MRI images vs. detecting unripe blueberries on a conveyer belt. On the other hand, high-stakes problems mandate higher standards for auditing model functionality. 

The Data Scientist must manage a balance between ensemble interpretability and black-box complexity. If this seems easy, it isn’t! Put yourself in the driver’s seat of the machine learning code for a self-driving car. If a well-behaved regression model makes a right decision 99.5% of the time, but a complex, less-explainable ensemble is right 99.8% of the time, which would you pick?
