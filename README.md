# Churn Prediction for Energy Company SME Customers

## Introduction

### The Project

At the end of my Master in Big Data program in IE School of Human Sciences and Technology, we were given the opportunity to participate in a datathon hosted by BCG Gamma. We were given a dataset of more than 16,000 existing customers in Jan 2016 and whether they have churned by March 2016 as training data. The data also consisted of their energy consumption, price history, gross margin, zip code, industry, etc.

### Goals & Objectives

Our task was to create descriptive statistics and visuzliation of the drivers of churn, build statistical model to predict churn, and assess the opportunity of giving all identified churners a 20% discount and come up with additional measures.

### Uploaded Information

As this was a group project with a tight turnaround time, we split up the tasks and I was responsible for coming up with a model for the prediction. Since I was not responsible for the visualization or evaluating the viability of the discount pertaining to the financials, I have uploaded only the codes for data cleaning and the model. It is of note that a good portion of the data cleaning was completed by my teammate, Emily, but the codes uploaded were rewritten by me.

## Data

Due to the NDA Agreement, I have excluded the data files and any printing of the data in the Jupyter Notebooks.

While examining the data, we found that forecasted data were durastically different from the historical data, especially in terms of energy consumption. Due to the unexplained inconsistancy of the forecast and that I wanted to refrain from using forecasted data to predict churn behavior, none of the forecasted features were used in the models.

## Evaluation Metrics & Best Model

The main evaluation metrics were AUC Score and F1 Score. While the normal business process would be to calculate percentage of churn and target the customers with high percentages, the datathon requirements specifically asked for 0/1 classifications of churners.

The best model was able to achieve a AUC Score of 0.7585. The F1 Score depened on the cut-off threshold. A 0.5 cut-off yielded a score of 0.2434, and a 0.35 cut-off yielded a score of 0.3941.
