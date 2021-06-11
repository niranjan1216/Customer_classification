# Customer Classification Using Logistic Regression

[![cc](https://raw.githubusercontent.com/niranjan1216/Machine_Learning_Foundation/main/CUSTOMER_CLASSIFICATION/images/clustering1.png "cc")](https://raw.githubusercontent.com/niranjan1216/Machine_Learning_Foundation/main/CUSTOMER_CLASSIFICATION/images/clustering1.png "cc")


## **1. Introduction**


Retail banking institution is going to float a stock trading facility for their existing customers.The idea is to use data to classify whether a customer belongs to a high net worth or low net worth group.They will have to incentivize their customers to adopt their offerings.One way to incentivize is to offer discounts on the commission for trading transactions.The company rolled out this service to about 10,000+ of its customers and observed their trading behavior for 6 months and after that, they labeled them into two revenue grids 1 and 2.

## **2. Problem Statement**

One issue is that only about 10% of the customers do enough trades for earnings after discounts to be profitable.The company wants to figure out, which are those 10% customers so that it can selectively offer them a discount.The marketing department want to supplement their campaigns with a more proactive approach.Dataset contains past customers details and their status (Revenue Grid 1 or 2).
Task is to build a classification model using Logistic Regression to predict whether a customer belongs to a high net worth or low net worth group.This model can  be evaluated using F1 Score.

[![cc2](https://raw.githubusercontent.com/niranjan1216/Machine_Learning_Foundation/main/CUSTOMER_CLASSIFICATION/images/clustering2.png "cc2")](https://raw.githubusercontent.com/niranjan1216/Machine_Learning_Foundation/main/CUSTOMER_CLASSIFICATION/images/clustering2.png "cc2")

## **3.Data Description**

dataset containing all the necessary information about the customers like their occupation, family income, gender, region, balance transfer, children, etc.Also included in the dataset is the column Revenue_Grid which classifies the customers into high net worth customers (1) and low net worth customers (2).

### **3.1 Data Statistics & Insights**

- Dataset contains 8124 rows, 32 columns.
- **61%(4989 out of 8124)** of customers are not using Credit_Card.Their Average_Credit_Card_Transaction is 0.0.
- **63%** Customers are not having Personal_Loan.
- **63%** Customers are not having Investment_Tax_Saving_Bond.
- **69%** Customers are not having Home_Loan.
- **5700** customers are not interested online Purchase.

## **4.Exploratory Data Analysis**

EDA on this dataset reveals following hidden facts in the data.
- Number of Customers in Grid-I: **860**
- Number of Customers in Grid-II: **7264**
- Average Investment of customers in **Revenue_Grid-1** is **155**.
- Average Investment of customers in **Revenue_Grid-2** is **81**.
- customers having family income >= 35000 are invested more in trading.
- Highest average Investment in Trading from Customers in the **age_band 18-21**

## **5.Model Development & Evaluation**

- **Logistic Regression** is used to build model.This model can be evaluated by computing metrics like, **Accuracy**,**Precision**, **Recall score**, **F1-Score**.
- The F measure (F1 score or F score) is a **measure of a test’s accuracy** and is defined as **the weighted harmonic mean of the precision and recall of the test**.
- The F score can **provide a more realistic measure of a test’s performance** by **using both precision and recall**. 
- The F score is often **used in information retrieval** for measuring search, **document classification**, and **query classification performance**.

<center><img src="https://raw.githubusercontent.com/insaid2018/Term-2/master/images/f1.jpg" width="300" height="240" /></center>
- Our objective is to minimize False Positive so that customer belongs to low net worth group should not predicted as high net worth group. Therefore, among recall & precision scores, we will give more importance to precision score.
**Precision score** for above model is: **0.8125.**

## **9. Conclusion**

- Studied various **features** of the given customer dataset,its **characteristics** and **distribution**.
- Investigated indepth about the features which to **retain** and which to **discard**.
- **Exploratory Data analysis** helps in finding hidden patterns in the data.
- Logistic Regression Model is Built for Prediction.
- Computed **metrics** for model Evaluation
- This **Model** now can **help us** in **identifying** the  **high net worth customer**.

