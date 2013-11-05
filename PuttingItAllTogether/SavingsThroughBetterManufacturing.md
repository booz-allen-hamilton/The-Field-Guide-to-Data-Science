#SAVINGS THROUGH BETTER MANUFACTURING 


##ANALYTIC CHALLENGE
A manufacturing company engaged Booz Allen to explore data related to chemical compound production. These processes are quite complex. They involve a long chain of interconnected events, which ultimately leads to high variability in product output. This makes the production very expensive. 

Understanding the production process is not easy – sensors collect thousands of time series variables and thousands of point-in-time measurements, yielding terabytes of data. There was a huge opportunity if the client could make sense of this data. Reducing the variance and improving the product yield by even a small amount could result in significant cost savings. 



##OUR SOLUTION
Due to the size and complexity of the process data, prior analysis efforts that focused on data from only a single sub-process had limited success. Our Data Science team took a different approach: analyzing all the data from all the sub-processes with the goal of identifying the factors driving variation. Once we understood those factors, we could develop recommendations on how to control them to increase yield. The client’s process engineers had always wanted to pursue this approach but lacked the tools to carry out the analysis. 

We decomposed the problem into a series of smaller problems. First, it was necessary to identify which time series parameters likely affected product yield. We engaged the client’s domain experts to identify their hypotheses surrounding the process. Once we discerned a set of hypotheses, we identified the sensors that collected the relevant data. 

We began initial data processing, which included filtering bad values and identifying patterns in the time series. We then needed to segment the data streams into individual production runs. We identified a sensor that stored the high-level information indicating when a production process began. This sensor provided exactly what we needed, but we quickly noticed that half of the expected data was missing. Examining the data more closely, we realized the sensor had only been used within recent years. We had to take a step back and reassess our plan. After discussions with the domain experts, we identified a different sensor that gave us raw values directly from the production process. The raw values included a tag that indicated the start of a production run. The sensor was active for every production run and could be used reliably to segment the data streams into production runs.
 
Next, we had to determine which time series parameters affected product yield. Using the cleaned and processed data and a non-parametric correlation technique, we compared each time series in a production run to all other time series in that same run. Given the pair-wise similarities, we estimated correlation of the similarities to final product yield. We then used the correlations as input into a clustering algorithm to find clusters of time series parameters that correlated with each other in terms of product yield, not in terms of the time series themselves. This data analysis was at a scale not previously possible – millions of comparisons for whole production runs. Engineers were able to look at all the data for the first time, and to see impacts of specific parameters across different batches and sensors.

In addition to identifying the key parameters, the engineers needed to know how to control the parameters to increase product yield. Discussions with domain experts provided insight into which time series parameters could be easily controlled. This limited the candidate parameters to only those that the process engineers could influence. We extracted features from the remaining time series signals and fed them into our models to predict yield. The models quantified the correlation between the pattern of parameter values and yield, providing insights on how to increase product yield. 



##OUR IMPACT
With controls identified and desirable patterns quantified, we provided the engineers with a set of process control actions to improve product output. The raw sensor data that came directly from the production process drove our analysis and recommendations, thus providing the client with confidence in the approach. The reduction in product yield variability will enable the client to produce a better product with lower risk at a reduced cost. 
