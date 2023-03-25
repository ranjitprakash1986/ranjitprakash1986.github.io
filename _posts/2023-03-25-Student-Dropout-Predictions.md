---
layout: post
title: Predicting Student Dropout
subtitle: Using ML algorithms to predict student dropout from college
cover-img: /assets/img/banner-dark.jpg
thumbnail-img: /assets/img/student-thumb.jpg
share-img: /assets/img/path.jpg
tags: [Prediction, Classification]
---
### Introduction

Academic performance/graduation in a population is an important factor in their overall employability which contributes towards economic development. This Data Science project predicts Student Dropout given the factors on demography, socioeconomics, macroeconomics, and relevant academic data provided by the Student on enrollment. This prediction is important to understand the student's academic capacity. This important knowledge can be used to identify key areas of development such as the development of socially disadvantaged communities, improvement of academic programs, development of educational funding programs, etc. This project will try to investigate the following research question:

>Given a student with his/her demography, socioeconomics, macroeconomics, and relevant academic data, how accurately can we predict whether he/she will drop out of school?

For complete information, code and report, please visit this [repository](https://github.com/ranjitprakash1986/dropout_predictions)

### Data

The dataset used in the project contains data collected at the time of student enrollment and a snapshot of their performance at the end of the 2nd semester at their respective Universities. This includes discrete and continuous data that capture the various facets of the student. These include macroeconomic factors of inflation, GDP, and the unemployment rate. It covers the personal/family details of the student such as gender, previous grade, educational special needs, financial status, parents’ education, and parents’ occupation. It captures aspects of the educational system such as coursework enrolled, day/evening classes, scholarships offered, etc. The dataset is created by Valentim Realinho, Mónica Vieira Martins, Jorge Machado, and Luís Baptista from the Polytechnic Institue of Portalegre. It was sourced from the UCI Machine Learning Repository and can be downloaded from here. Each row represents the details pertaining to an individual student and there are no duplicates.

The original dataset exhibits three classifications (class) of students - Graduate, Enrolled, and Dropout. For the binary classification question pursued in this project, the class Enrolled is omitted from the dataset. The preliminary EDA shows there are 2209 examples of Graduate students and 1421 examples of Dropouts. Thus the dataset imbalance is not a major concern and can be addressed through balancing techniques learned in the MDS program.

### Results

The objective of this project is to investigate how accurately we can predict that a student will drop out of school. Furthermore what underlying factors are the predominant influencing this outcome? Accurate classification of a true drop out in the available data is our chosen metric of interest. This is defined as Recall and it represents the proportion of the true drop-outs in the dataset, accurately predicted by the model. Each of the three models Naive Bayes, Logistic Regression and Random Forest Classifier were fitted on training data. The hyperparameter tuning was performed on using Random Search CV for Logistic Regression and Random Forest Classifier. The optimized models were then used to predict the classification on the test data. The performance of the models was compared through the Confusion Matrix, Precision-Recall curve, and Receive-Operating Characteristics plots. The metrics were tabulated for numerical interpretation.

![Precision_Recall_table](../assets/img/precision_recall_table_dropout_prediction.png)

Our train-test split yielded 726 examples in the testing dataset. There are 425 actual class Dropout and the rest are Graduate. The classification as a Dropout is considered as a Positive in the context of this project. The Logistic Regression model identified the highest True positives among the three models (386) and achieved a superior recall metric of 0.83. Naive Bayes model came close behind with 400 true positives at a recall metric of 0.66. The Random Forest model achieved an appreciable recall metric of 0.8 with 403 true positive. Overall, the Logistic Regression model result in the highest recall score (0.83) and since we focus on the recall score (those who drop out of school), therefore, we conclude that the Logistic Regression model perform the best in terms of recall.

The Random Forest Classifier and Logistic Regression performed appreciably on the f1 score which is a balanced measure of model precision and recall. However Naive Bayes suffered a relative low f1 score due to a low precision. This is due to more False Positives predicted by Naive Bayes than the other models. The corresponding confusion matrices derived from the analysis are shown below for reference.

![Precision_Recall_Curve](../assets/img/PR_curve_dropout_prediction.png)

![Precision_Recall_Curve](../assets/img/ROC_curve_dropout_prediction.png)

The correlation plot between the factors and the target objective reveals some that female students with Debts have a high possibility of dropping out of school.

![correlation_dropout_prediction](../assets/img/correlation_dropout_prediction.png)

This project was completed in accordance to the requirements in the MDS program 2022-2023. If you have any questions, please feel free to connect with me at my social media handles.
