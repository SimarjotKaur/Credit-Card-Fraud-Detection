# Credit-Card-Fraud-Detection
Credit Card Fraud Detection using Neural Networks (Keras)
This involves pattern classification in an unbalanced dataset to determine the fraudulent transactions.

# Dataset
The dataset used for this research is collected from Kaggle at https://www.kaggle.com/mlg-ulb/creditcardfraud. It consists of 284,807 transactions that occurred in 2 days, of which 492 are labelled as Fraud. This means that the dataset is highly unbalanced with only 0.172% accounting for the Fraud transactions. It consists of 31 features of which 28 (V1-V28) are the result of PCA transformation, due to confidentiality issues. The remaining features that are not transformed are ‘Time’ and ‘Amount’, which represent the seconds elapsed between each transaction and the first transaction in the dataset and, the transaction amount respectively. The ‘Class’ feature represents the label of the transaction with ‘1’ for a Fraud transaction and ‘0’ for a ‘Genuine’ transaction. <br>

[Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson and Gianluca Bontempi. Calibrating Probability with Undersampling for Unbalanced Classification. In Symposium on Computational Intelligence and Data Mining (CIDM), IEEE, 2015]

# Experimental Design
<ul>
<li> 
<b>Algorithm Selection:</b>
This research is basically based
on whether the performance of a Neural Network would
significantly differ if one part of the algorithm’s configuration
is changed. Firstly, a multi-layer perceptron with 1-hidden
layer was trained followed by a multi-layer perceptron with 2
hidden layers. Most of the parameters were tuned using Gridsearch
algorithm followed by Trial and Error and, the rest
were used as default provided by the Keras library.
</li>
<li>
<b>Testable Hypothesis:</b>
A neural network’s performance on the Credit-Card Fraud dataset is affected by
the number of hidden layers.
<ul>
<li>Null Hypothesis (H0): Insufficient evidence to
support the hypothesis. </li>
<li>Alternate Hypothesis (H1): Evidence suggests the
hypothesis is likely true. </li>
</ul>
This means that if the null hypothesis is accepted, there is
no significant difference between the performance of the two
MLPs with a different number of hidden layers. However, if
the null hypothesis is rejected, i.e., the alternate hypothesis is
accepted, it implies that changing the number of hidden layers
in the neural network has a significant difference in the
performance of the model.
</li>
</ul>
