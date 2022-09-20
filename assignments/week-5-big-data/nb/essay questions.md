 
**Algorithm Understanding Qeusiton:** How does the Gradient-Boosted Tree Algorithm work in Classification? How does Gradient Boost differ from AdaBoost and Logistic Regression?

**Ans:**


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