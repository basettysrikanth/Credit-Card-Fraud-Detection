# Credit-Card-Fraud-Detection

**Introduction:**

Financial fraud is a growing concern with far reaching consequences in the government, corporate organizations, finance industry, In Today’s world high dependency on internet technology has enjoyed increased credit card transactions but credit card fraud had also accelerated as online and offline transaction. As credit card transactions become a widespread mode of payment, focus has been given to recent computational methodologies to handle the credit card fraud problem. There are many fraud detection solutions and software which prevent frauds in businesses such as credit card, retail, e-commerce, insurance, and industries. Data mining technique is one notable and popular methods used in solving credit fraud detection problem. It is impossible to be sheer certain about the true intention and rightfulness behind an application or transaction. In reality, to seek out possible evidences of fraud from the available data using mathematical algorithms is the best effective option. Fraud detection in credit card is the truly the process of identifying those transactions that are fraudulent into two classes of legit class and fraud class transactions, several techniques are designed and implemented to solve to credit card fraud detection such as genetic algorithm, artificial neural network frequent item set mining, machine learning algorithms, migrating birds optimization algorithm, comparative analysis of logistic regression, SVM, decision tree and random forest is carried out. Credit card fraud detection is a very popular but also a difficult problem to solve. Firstly, due to issue of having only a limited amount of data, credit card makes it challenging to match a pattern for dataset. Secondly, there can be many entries in dataset with truncations of fraudsters which also will fit a pattern of legitimate behavior. Also the problem has many constraints. Firstly, data sets are not easily accessible for public and the results of researches are often hidden and censored, making the results inaccessible and due to this it is challenging to benchmarking for the models built. Datasets in previous researches with real data in the literature is nowhere mentioned. Secondly, the improvement of methods is more difficult by the fact that the security concern imposes an limitation to exchange of ideas and methods in fraud detection, and especially in credit card fraud detection. Lastly, the data sets are continuously evolving and changing making the profiles of normal and fraudulent behaviors always different that is the legit transaction in the past may be a fraud in present or vice versa. This paper evaluates four advanced data mining approaches, Decision tree, support vector machines, Logistic regression and random forests and then a collative comparison is made to evaluate that which model performed best. Credit card transaction datasets are rarely available, highly imbalanced and skewed. Optimal feature (variables) selection for the models, suitable metric is most important part of data mining to evaluate performance of techniques on skewed credit card fraud data. A number of challenges are associated with credit card detection, namely fraudulent behavior profile is dynamic, that is fraudulent transactions tend to look like legitimate ones, Credit card fraud detection performance is greatly affected by type of sampling approach used, selection of variables and detection technique used. In the end of this paper, conclusions about results of classifier evaluative testing are made and collated. From the experiments the result that has been concluded is that Logistic regression has a accuracy of 97.7% while SVM shows accuracy of 97.5% and Decision tree shows accuracy of 95.5% but the best results are obtained by Random forest with a precise accuracy of 98.6%. The results obtained thus conclude that Random forest shows the most precise and high accuracy of 98.6% in problem of credit card fraud detection with dataset provided by ULB machine learning. 

**1.1 Objective:**

The objectives of the project is to implement machine learning algorithms to detect credit card fraud detection with respect to time and amount of transaction.

**1.2 Outline:**

This work is articulated as following: after having introduced the stakes of credit card fraud detection and the properties, we will describe more formally the problem of credit card fraud detection and highlight the research questions it raises in chapter 2. Afterwards, we will present in chapter 3 the state of the art approaches for handling the special difficulties of credit card fraud detection (namely: Gass algorithm, Bayesian networks, Hidden markov model, Genetic algorithm, Decision tree, Neural network, Logistic Regression, and Random Forests). In chapter 4, we will highlight the particularities of the credit card transactions dataset used throughout this work and conduct an exploratory analysis in order to quantify the dataset shift in it and scope of the project. 

**1.3 Motivation:**

In the current state of the nation, by using revolutionary services such as credit cards, Automated Teller Machines (ATM), services and digital banking services, financial organizations are expanding the availability of financial facilities. Besides, along with the rapid advances of e-commerce, the use of deposit card has grown to be a convenience and essential phase of monetary life. Credit card is a charge card supplied to clients as a system of payment. 

**1.4	Scope of the Project:**

In this proposed project we designed a protocol or a model to detect the fraud activity in credit card transactions. This system is capable of providing most of the essential features required to detect fraudulent and legitimate transactions.
As technology changes, it becomes difficult to track the behaviour and pattern of fraudulent transactions. With the upsurge of artificial intelligence and other relevant fields of information technology, it becomes feasible to automate the process and to save some of the effective amount of labor that is put into detecting credit card fraudulent activities.

**IDENTIFYING FRAUDULENT DETECTION TECHNIQUES:**

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

**MODEL PREDICTION**

Now it is time to start building the model .The types of algorithms we are going to use to try to do anomaly detection on this dataset are as follow:

**ISOLATION FOREST ALGORITHM :**

One of the newest techniques to detect anomalies is called Isolation Forests. The algorithm is based on the fact that anomalies are data points that are few and different. As a result of these properties, anomalies are susceptible to a mechanism called isolation.
Typical machine learning methods tend to work better when the patterns they try to learn are balanced, meaning the same amount of good and bad behaviors are present in the dataset.
How Isolation Forests Work The Isolation Forest algorithm isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature. The logic argument goes: isolating anomaly observations is easier because only a few conditions are needed to separate those cases from the normal observations. On the other hand, isolating normal observations require more conditions. Therefore, an anomaly score can be calculated as the number of conditions required to separate a given observation.
The way that the algorithm constructs the separation is by first creating isolation trees, or random decision trees. Then, the score is calculated as the path length to isolate the observation.

**LOCAL OUTLIER FACTOR (LOF) ALGORITHM**

The LOF algorithm is an unsupervised outlier detection method which computes the local density deviation of a given data point with respect to its neighbors. It considers as outlier samples that have a substantially lower density than their neighbors.
The number of neighbors considered, (parameter n_neighbors) is typically chosen 1) greater than the minimum number of objects a cluster has to contain, so that other objects can be local outliers relative to this cluster, and 2) smaller than the maximum number of close by objects that can potentially be local outliers. In practice, such informations are generally not available, and taking n_neighbors=20 appears to work well in general.

**RESULT**

•	Isolation Forest detected 73 errors versus Local Outlier Factor detecting 97 errors vs. SVM detecting 8516 errors
•	Isolation Forest has a 99.74% more accurate than LOF of 99.65% and SVM of 70.09
•	When comparing error precision & recall for 3 models , the Isolation Forest performed much better than the LOF as we can see that the detection of fraud cases is around 27 % versus LOF detection rate of just 2 % and SVM of 0%.
•	So overall Isolation Forest Method performed much better in determining the fraud cases which is around 30%.
•	We can also improve on this accuracy by increasing the sample size or use deep learning algorithms however at the cost of computational expense.We can also use complex anomaly detection models to get better accuracy in determining more fraudulent cases

**CONCLUSION**
At present credit card fraud detection is one of the major issues in current transaction that are made online. Fraud can be committed in different ways and in many industries. The majority of detection methods combine a variety of fraud detection datasets to form a connected overview of both valid and non-valid payment data to make a decision. This decision must consider IP address, geolocation, device identification, “BIN” data, global latitude/longitude, historic transaction patterns, and the actual transaction information. In practice, this means that merchants and issuers deploy analytically based responses that use internal and external data to apply a set of business rules or analytical algorithms to detect fraud.

To avoid such situation, it is mandatory to design a classifier that can classify which transaction are fraud and which are real ones. We are going to divide the dataset into training and testing phase for implementing further processes. We have used K-means algorithm which is an unsupervised in nature for clustering. We need a dataset which have both the entries fraudulent and genuine as we require this for training phase. Thus, by K-Means clustering and machine learning algorithms (Isolation forest and local outlier factor) which can be best adapt to the change in scenario taking place can be used and developed on a very large scale to detect the fraudulent transactions and used to ensure the credibility of payment system.


