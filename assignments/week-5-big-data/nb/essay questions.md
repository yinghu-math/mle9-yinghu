 
**Algorithm Understanding Qeusiton:** How does the Gradient-Boosted Tree Algorithm work in Classification? How does Gradient Boost differ from AdaBoost and Logistic Regression?

**Ans:** Gradient Boost and AdaBoost are two examples of ensemble methods that combine several weaker predictors into a stronger one. In both algorithms, weaker predictors are produced sequentially. The difference between the two methods lies in how they produce and combine these weaker models. 

AdaBoost trains the new model by increasing weights to the data points that were incorrectly predicted by the previous model. On the other hand, in the Gradient Boosting algorithm, one trains the next model on the errors made by the previous predictor.  

I saw how gradient boost being used in regression tasks before. For using the Gradient-Boosted Tree Algorithm in a classification task, I think one would first train a base model on the entire train data as the starting point. Then to get the next model, one would collect the data points that were misclassified by the previous model and train a model just on these data. **But I am not sure how to aggregate these models together in this case. Do you have any references I can look at?**


**Interview Readiness Qeusiton:** What is a Delta Lake and how does it offer a solution to building reliable data pipelines?

**Ans:** Delta lake can be used as a layer in the lakehouse architecture between the unstructured data in Data lake and other compute engines/applications that use these data. It has many functionalites. For one, it can filter and clean the unstructured data before they are fed into a machine learning pipeline. 


**Interview Readiness  Qeusiton:** When working with Pandas, we use the class pandas.core.frame.DataFrame and when working with the pandas API in Spark, we use the class pyspark.pandas.frame.DataFrame, are these the same, explain why or why not?


**Ans:** Both DataFrame classes are suitable for tabular data. 

Pandas is a convenient python library for analyzing tabular data. But it does in-memory analytics and should not be used if the dataset is larger than size of the RAM. (https://pandas.pydata.org/docs/user_guide/scale.html)

On the other hand, Spark is a distributed computation system; naturally, it is ideal if we are dealing with large data.  

**Interview Readiness  Qeusiton:** What is a Machine Learning Pipeline is and why it’s important? What are the steps in a Machine Learning workflow?

**Ans:** A Machine learning workflow usually consists of 

(1) data collecting and processing (this including feature extraction), 

(2) train the model, and 

(3) evaluate the model and possibly go back to steps (1) or (2)

(4) deploy the model

(5) continue monitoring the model and go back to steps (1) or (2) when needed.

A machine learning pipeline is a software construct that orchestrates modules in the machine learning workflow, and automates it as much as possible. 