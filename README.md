# Bank Customer Churn Rate Prediction using a Artifical Neural Network

* Created visuals to analyze the customer churn rate to see which factors could affect the churn rate
* Processed and adjusted the categorical data using the Label Encoder and One Hot Encoder from Sklearn
* Standardardized the data to improve the Artificial Neural Network
* Trained the Artificial Neural Network with two hidden layers using the rectifier and sigmoid activation function 
* Created a confusion matrix to visualize the accuracy of the model 

# Code and Packages Used

Python Version: 3.9
Packages: Pandas, NumPy, Matplotlib, Seaborn, Sklearn, TensorFlow

# Introduction
A bank has noticed an increase in its churn rates. A sample of 10,000 customers was taken with the information available to the bank. In this report, I will construct a  model using an Artificial Neural Network to find the probability of a customer terminating their service. This can be used to find customers with a churn probability greater than 50% and inform the bank to offer incentives for the customer to retain them.

# Data Visuals

<img src= "https://github.com/JMarcoOviedo/Bank_Customer_Churn-Model/blob/main/images/bank7.png"/>

<img src= "https://github.com/JMarcoOviedo/Bank_Customer_Churn-Model/blob/main/images/Bank1.png"/>
Looking at the pie chart, we can see that the bank has retained 79% of its customers while only 20.4% have discontinued their service. Also, looking at the count plots, we can see that the proportion of females discontinuing their service compared to males is greater. Lastly, customers with only one product from the bank have the highest proportion of discontinuing service, while customers with two or more products have a smaller proportion.


<img src= "https://github.com/JMarcoOviedo/Bank_Customer_Churn-Model/blob/main/images/Bank4.png"/>
Looking at the Correlation Matrix we can see that the Balance and Number of Products have a negative correlation value meaning that they have an inverse relation. Secondly the age and the Exited have the second highest correlation value.

# Data Processing

<img src="https://github.com/JMarcoOviedo/Bank_Customer_Churn-Model/blob/main/images/data.png"/>


Here is the first five objects in the data set. For our ANN model we will not include the columns 'RowNumber', 'CustomerId', 'Surname' because they will not provide any useful information to our prediction model. Then after I will transform the categorical variable into binary values. 
