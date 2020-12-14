# Churn-Analysis-with-PySpark
#### Problem statement
Sparkify is a fictional music streaming company similar to Spotify. It business model follows subscriber-based model, which means users can choose to pay a monthly fee to enjor their premiumn service. However, users can also choose to switch to free tier anytime.
In this post, I am going to manipulate the datasets with Spark to predict custumer churn.
Medium: https://medium.com/@zyan5/predicting-churn-for-music-streaming-app-with-spark-5527764c6157
#### Metrics
Here I will test out several of the most common machine learning methods and evaluated the accuracy of the three models using the F1 Score. Since the churned users are a fairly small subset, the F1 score should be used to balance the precision and recall.

#### Data Exploration & Data Visualization
In the data exploration phase, I have define the churn varaible and used EDA against other related variables.For example, I investigated location attributes and provides visuliazation to show the number of churned customers by various cities. I have also provide analysis on music, length, gender and other attributes in this section.

#### Data Preprocessing
In this section, I prepared the data ready for mahchine learning model.When writing the script, I also make sure the script is scalable and modular.
One of the examples of such practice is using pipelines. I used the pipeline to transform categorical variable location and gender data to the numeric form because most of the current ML algorithm requires a numeric vector. The pipeline will help us streamline the fit and transform process and make the code looks clean and easy.
#### Implementation
Here I have used out several of the most common machine learning methods and evaluated the accuracy of the three models: Logistic Regression, Random Forest, and Decision Tree. 
The reason I prefer simpler model is because we can better interprete the model result and communicate the finding to bussiness users. We use the model here as a baseline. Then try to refine and tune it in the next section.
#### Refinement
In this section, I have used the grid search to tune the logistic regression model because it has the best baseline performance out of the box.
#### Model Evaluation and Validation
After tunning, the linear regression model come back with an F1 score of 
#### Justification

#### Reflection and Improvement
