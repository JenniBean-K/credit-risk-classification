## Credit Risk Classification

### Overview of the Analysis

The purpose of this analysis was to build a machine learning model that can predict the credit risks of loans, identifying wheter a loan is likely to be healthy (0) or hig-risk (1), using historical data from a peer-to-peer lending platform.

The dataset included borrower financial features such as:
* Loan size
* Intreset rate
* Income
* Debt-to-income ratio
* Number of accounts
* Deragatory marks
* Total debt

A logistic regression model was evaluated on a test set, and the results were as follows:
* Accuracy Score: ~0.995
* Precision:
    * Class 0 (Healthy Loans): 1.00
    * Class 1 (High_Risk Loans): 0.87
* Recall:
 
    * Class 0: 0.995
    * Class 1: 0.95

### Confusion Matrix
```
[[18673    86]
 [   32   593]]
```
### Summary 

This logistic regression model preformed exceptionally well overall, particularly in identifying healthy loans:

* It correctly predicted 18,673 out of 18,759 health loans (true negatives).
* It identified 593 out of 625 high- risk loans correctly (true positives).
* The model only misclassified 32 high-risk loans as healthy (false-negatives), and 86 healthy laons as high-risk (false-positives).

Given the high accuracy, percision, and recall, especially on the minority class ( high-risk loans), this model is a strong baseline solution.

### Recommendation

I recommend using this logistic regression model for initial credit risk classification. It provides reliable predictions, is computationally efficent, and interpretable, making it sutible for finacial decision making.

However, since misclassifying high-risk laons could result in finacial losses, the model could be further improved by:

* Testing alternative algorithms 
* Addressing class imbalance
* Incorporating additional borrower attributes it available


