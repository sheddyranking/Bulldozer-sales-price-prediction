# Bulldozer-sales-price-prediction

 **Predicting the Sale Price of Bulldozers using Machine Learning**
 
In this notebook, we're going to go through an example machine learning project with the goal of predicting the sale price of bulldozers.

Since we're trying to predict a number, this kind of problem is known as a `regression problem`.

### **1. Problem Definition** 

For this dataset, the problem we're trying to solve, or better, the question we're trying to answer is,

> How well can we predict the future sale price of a bulldozer, given its characteristics previous examples of how much similar bulldozers have been sold for?

### **2. Data**

Looking at the dataset from Kaggle(https://www.kaggle.com/c/bluebook-for-bulldozers/data), you can you it's a time series problem. This means there's a time attribute to dataset.

In this case, it's historical sales data of bulldozers. Including things like, model type, size, sale date and more.

There are 3 datasets:

`Train.csv `- Historical bulldozer sales examples up to 2011 (close to 400,000 examples with 50+ different attributes, including SalePrice which is the target variable).

`Valid.csv` - Historical bulldozer sales examples from January 1 2012 to April 30 2012 (close to 12,000 examples with the same attributes as Train.csv).

`Test.csv` - Historical bulldozer sales examples from May 1 2012 to November 2012 (close to 12,000 examples but missing the SalePrice attribute, as this is what we'll be trying to predict).

### **3. Evaluation**

For this problem, Kaggle has set the evaluation metric to being root mean squared log error (RMSLE)(https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation). As with many regression evaluations, the goal will be to get this value as low as possible.

To see how well our model is doing, we'll calculate the RMSLE and then compare our results to others on the Kaggle leaderboard(https://www.kaggle.com/c/bluebook-for-bulldozers/leaderboard).


### **4. Features**

Features are different parts of the data. During this step, you'll want to start finding out what you can about the data.

One of the most common ways to do this, is to create a data dictionary.

For this dataset, Kaggle provide a data dictionary which contains information about what each attribute of the dataset means. You can download this file directly from the Kaggle competition page (https://www.kaggle.com/competitions/bluebook-for-bulldozers/data?select=Data+Dictionary.xlsx)

First, we'll import the dataset and start exploring. Since we know the evaluation metric we're trying to minimise, our first goal will be building a baseline model and seeing how it stacks up against the competition



### **5.Experimental and conclusion**

From the experiment/modelling the `RMSLE` which is the set as the evaluation metric was `0.24540654616643515` on the `validation set`. and the model predicted the prices for the bulldozer sales perfectly on the `test set`, click here to view https://drive.google.com/file/d/1Z40zNlFM35ldUGM7r-3Uae0-iiuH9fuv/view?usp=sharing

download the model fitted/trained model here : https://drive.google.com/file/d/1h2M51_cXKaxUiH9uqSZ7NFt7PclHfmM5/view?usp=sharing

### **6.Feature importance**
From the table below it can be seen that the `yearMade` contributed more to the sale price prediction model

![feature](https://user-images.githubusercontent.com/42388234/193078318-1a68408f-a59f-432e-9ce1-4861416ce66b.png)



