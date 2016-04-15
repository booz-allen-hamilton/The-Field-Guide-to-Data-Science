#Predicting Customer Response

##Analytic Challenge

It is very challenging to know how a customer will respond to a given promotional campaign. Together with the InterContinental Hotels Group (IHG), Booz Allen Hamilton explored approaches to predict customer-by-customer response to a stateof- the-art promotional campaign in order to better understand and increase return on investment (ROI). 

In the past, conventional statistics have worked well for analyzing the impact of direct marketing promotions on purchase behavior. Today, modern multi-channel promotions often result in datasets that are highly dimensional and sometimes sparse, which strains the power of conventional statistical methods to accurately estimate the effect of a promotion on individual purchase decisions. Because of the growing frequency of multi-channel promotions, IHG was driven to investigate new approaches. In particular, IHG and Booz Allen studied one recent promotional campaign using hotel, stay, and guest data for a group of loyalty program customers.

##Our Approach

Working closely with IHG experts, Booz Allen investigated three key elements related to different stages of analytic maturity: 

Describe: Using initial data mining, what insights or tendencies in guest behaviors can be identified after joining multiple, disparate datasets? 

Discover: Can we determine which control group members would be likely to register for a promotion if offered? If so, can we also quantify their registration? 

Predict: How would a hotel guest that received the promotion have responded if they were not offered the promotion? How would a hotel guest that did not receive the promotion have responded if they were offered the promotion? For the promotion that was the focus of this case study, not everything about customers could be controlled as required by traditional statistics. However, because a probabilistic Bayesian Belief Network (BBN) can learn the pairwise relationships between all individual customer attributes and their impact on promotional return, Booz Allen investigated how this technique could be used to model each treated customer without an exact controlled look-alike. 

Specifically, Booz Allen developed a BBN to predict customer-by-customer impacts driven by promotional campaign offers, subsequently estimating the aggregated ROI of individual campaigns. We used six machine learning techniques (support vector machine, random forest, decision tree, neural network, linear model, and AdaBoost) in unison with the BBN to predict how each customer would be influenced by a promotional offer.

##Our Impact

The probabilistic model was capable of predicting customer response to the promotion, without relying on a costly control group. This finding represents millions of dollars of savings per promotional campaign. This analysis is an industryfirst for the travel and hospitality sector, where demand for more data-driven approaches to optimize marketing ROI at an individual level is rapidly growing. 

Because Booz Allen and IHG’s approach enabled estimation of ROI for each hypothetical customer, even when no exact look-alikes exist, there are a number of valuable future applications. One such application is optimal campaign design— the ability to estimate the promotional attributes for an individual customer that are likely to drive the greatest incremental spend. Another application is efficient audience selection - which would reduce the risk of marketing “spam” that prompts costly unsubscriptions and can negatively impact a hotel’s brand.