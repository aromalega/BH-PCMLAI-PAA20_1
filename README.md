### Project Title
Predicting the patients length of stay in a hospital

**Author**
Aroma Reddy Lega

#### Executive summary
I've taken a dataset that has 100k data points on patients admitted into hospital, indicators of their health condition and how long they were admitted in the hospital. Based on this dataset I want to predict the length of stay of a patient. I've cleaned the dataset by checking for null values, removing columns which are not required and then scaled it. I have used pricipal component analysis to reduce the dimentionality of the data.

#### Rationale
If a hospital is able to predict the patients length of stay they'll be able to preplan
- upcoming patient admissions
- number of staff required for the patients


#### Research Question
To predict the patients length of stay in a hospital based on variables like the indicators of patients health condition

#### Data Sources
I've used the below kaggle dataset
https://www.kaggle.com/datasets/aayushchou/hospital-length-of-stay-dataset-microsoft/data

### Feature Engineering
Dropped the unique id and some date columns which are not relevant to analysis
Found the correlation between numeric columns using heat map
---
Plotted Categorical Columns
---
---
---
Scaled the dataset and did Principal Component Analysis to reduce the dimentionality of the dataset
---

#### Methodology
I'm using the below modelling techniques for this analysis
    - Used a simple model like 
        - Linear Regression
    - Used regularization models like 
        - Ridge Regression
        - Lasso Regression
    - Used another model like 
        - Decision Tree Regression
    - Used an ensemble model like
        - Gradient Boosting Regression

I've also performed Grid Search with Cross-Validation on each of these models

#### Results
Mean Suared Error Comparision
---
Based on the MSE Comparision of models for the given dataset, Gradient Boosting performs better than the other models, as it has least MSE

Train Time Comparision
---
Based on the Train Time Comparision of models for the given dataset, Gradient Boosting has taken more time
According to my research Gradient Boosting Regression model gave the most accurate results

Mean Absolute Error Comparision
---
Based on the MAE Comparision of models for the given dataset, Gradient Boosting performs better than the other models, as it has least MAE

R-suared Comparision
---
Based on the R-squared Comparision of models for the given dataset, Gradient Boosting performs better than the other models. As higher R-squared value means that the model explains a larger proportion of the variability in the dependent variable. This suggests that the model is better at predicting the outcome. 

#### Next steps
We can further analyze this dataset by eliminating certain variables and trying the modeling to see if they increase accuracy

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
Aroma Reddy Lega
legaaroma@gmail.com