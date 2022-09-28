**Algorithm Understanding:** Is SVM (Support Vector Machine) a supervised or unsupervised learning algorithm? Why is SVM such a powerful classification method? What are 3 disadvantages of SVMs?

It is supervised. Non-linear SVMs transform linear non-separably data to higher dimensional linear separable data.

Non-linear SVM is slow on large dataset. 


**Interview Readiness:** What is the time complexity of SVM? What is it for Logistic Regression?

The training time complexity for SVM is $O(n\times d)$ and for non-linear SVM is $O(n^2 \times d)$ or $O(n^3\times d)$ where n is the number of data ponits and d is the number of features. 

For Logistic Regresion, the training complexity is $O(n\times d)$ where $n$ and $d$ are as above. 


**Interview Readiness:** Explain feature importance for the Random Forest algorithm? When examining feature importance, what is Gini impurity or information gain?

Random Forest is an ensemble of decision trees (with bagging). In the decision tree algorithm, at each iteration, the program greedily looks for a feature and a threshold to minimize the Gini impurity of the children nodes. 

Given a feature, one can look at all nodes that use that feature and compute the weighted average of the reduction of Gini impurity at these nodes. This will give a measure of the importance of each feature. 


**Interview Readiness:** SHAP (SHapley Additive exPlanations) is a game theoretic approach to explain the output of any machine learning model, what is it and how does it work?

SHAP is a python library for explaining ML models by assign a SHAP values to each feature. 


Reference: [link](https://www.mage.ai/blog/how-to-interpret-explain-machine-learning-models-using-shap-values)