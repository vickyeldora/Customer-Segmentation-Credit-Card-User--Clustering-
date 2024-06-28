## Assignment Objectives

### Clustering Concepts:

- Obtain data using BigQuery
- Prepare data for Clustering
- Understand the concept of Clustering using Scikit-Learn
- Implement Clustering on the given data

---

## Dataset

```{attention}
Pay attention to the dataset usage instructions!
```

1. For this assignment, the dataset will **not use `bigquery-public-data`**.

2. Access Google BigQuery and use the following information for the `FROM` clause:
   * Project ID: `ftds-hacktiv8-project`
   * Dataset Name: `phase1_ftds_005_bsd`
   * Table Name: `credit-card-information`

3. Fetch data with the following criteria: 
   * All data with an odd `CUST_ID` value.

4. Below is the information for each column:
   <img src='https://i.ibb.co/2sbf0Js/P1-G4-Dataset-Information.png'>

5. Save the dataset as a `.csv` file named `DataSet.csv`.

---

## Problem Statement:

A bank wants to better understand the behavior and habits of credit card users. The bank collected data on credit card users over six months regarding their habits and preferences. This information can help the bank formulate more effective marketing strategies and provide services that better meet customer needs. The bank has provided this data to me, a data scientist, to categorize credit card users.

## Objective:

This project aims to build a clustering model for customer segmentation based on the bank's credit card data. The goal is to create a `clustering model` using K-MEANS to identify groups of users with similar behavioral characteristics. This will enable the bank to tailor its marketing strategies and services more specifically to the needs and preferences of each customer segment.

---

## The notebook format:

1. The machine learning framework used should be Scikit-Learn.

2. Utilize visualization libraries such as matplotlib, seaborn, or others.

3. The notebook content should follow the outline below:
   1. Introduction
      > Contains the objective.

   2. SQL Query
      > Contains the query created to fetch data from Google Cloud Platform.

   3. Import Libraries
      > Contains all the libraries used in the project.

   4. Data Loading
      > This section includes the process of preparing data before further exploration, such as renaming columns, checking dataset size, etc.

   5. Exploratory Data Analysis (EDA)
      > This section contains data exploration on the dataset using queries, grouping, simple visualizations, and other techniques.

   6. Feature Engineering
      > This section contains the process of preparing data for model training, such as splitting data into train-test sets, data transformation (normalization, encoding, etc.), and other necessary processes.

   7. Model Definition
      > This section contains cells to define the model. Explain the reasons for using a particular algorithm/model, the hyperparameters used, the chosen metrics, and other related details.

   8. Model Training
      > This section contains only the code to train the model and the output generated. Perform several training processes with different hyperparameters to observe the results. Analyze and narrate these results in the Model Evaluation section.

   9. Model Evaluation
      > This section evaluates the model, showing its performance based on the chosen metrics. This is demonstrated through visualizations of performance trends and/or model error rates.

   10. Model Saving
       > This section contains the process of saving the model and other related files from the model-building process.
   
   11. Model Inference
       > The trained model is tested on data that is not part of the train-set or test-set. This data is in its original format, not scaled data. Use the best model based on the Model Evaluation results.

   12. Conclusion
       > Conclusions reflecting the results obtained in relation to the objective stated in the introduction.

---