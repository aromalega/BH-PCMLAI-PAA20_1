### Project Title
Predicting the patients length of stay in a hospital

**Author**
Aroma Reddy Lega

#### Executive summary
I've taken a dataset that has 100k data points on patients admitted into hospital, indicators of their health condition and how long they were admitted in the hospital. Based on this dataset I want to predict the length of stay of a patient. I've cleaned the dataset by checking for null values, removing columns which are not required and then scaled it. I have used pricipal component analysis to reduce the dimentionality of the data. I've used multiple modelling techniques to predict the length of stay of patient but found that Gradient Boosting has the best results even though its a bit time consuming.

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
![Heat Map](https://github.com/user-attachments/assets/c3640713-e133-4b49-87d3-cbe8d5add111)

Plotted Categorical Columns
![Gender Plot](https://github.com/user-attachments/assets/a901bfe1-b14a-4eb3-86e7-9eb4972f7bd9)

![Readmission Plot](https://github.com/user-attachments/assets/b8eb0f9c-1fad-4b8f-a6bf-de3fa162e372)

![Facility Plot](https://github.com/user-attachments/assets/f8a5ccf2-5a0f-4a14-a7a2-44b8b50ebd3b)

Scaled the dataset and did Principal Component Analysis to reduce the dimentionality of the dataset
![PCA](https://github.com/user-attachments/assets/0749060f-fb1a-4856-a7ef-ae05c2d13283)


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

![Prediction 1](https://github.com/user-attachments/assets/aebb6df4-8489-4139-a159-fd5c5035605d)


#### Results
Mean Suared Error Comparision
![MSE](https://github.com/user-attachments/assets/0487bf86-a96c-4eaa-a1f5-7e5c3ab6918a)

Based on the MSE Comparision of models for the given dataset, Gradient Boosting performs better than the other models, as it has least MSE

Train Time Comparision
![Train Time](https://github.com/user-attachments/assets/0b5b269a-75bc-420f-822d-904502cc17b9)

Based on the Train Time Comparision of models for the given dataset, Gradient Boosting has taken more time
According to my research Gradient Boosting Regression model gave the most accurate results

Mean Absolute Error Comparision
![MAE](https://github.com/user-attachments/assets/9c4d7538-79e2-4468-a282-f6600e27cfca)

Based on the MAE Comparision of models for the given dataset, Gradient Boosting performs better than the other models, as it has least MAE

R-suared Comparision
![R-squared](https://github.com/user-attachments/assets/bb5db71b-5427-4f25-8eae-8ddfea081fef)

Based on the R-squared Comparision of models for the given dataset, Gradient Boosting performs better than the other models. As higher R-squared value means that the model explains a larger proportion of the variability in the dependent variable. This suggests that the model is better at predicting the outcome. 

So, the best results are from Gradient Boosting ensemble technique even though it takes higher time than the other models.
![Prediction 2](https://github.com/user-attachments/assets/58fc016b-603b-4080-8e28-90322900200b)


#### Next steps
We can further analyze this dataset by eliminating certain variables and trying the modeling to see if they increase accuracy

#### Outline of project
Below is the link to the jupyter notebook
https://github.com/aromalega/BH-PCMLAI-PAA20_1/blob/main/LenthOfPatientStay.ipynb


##### Contact and Further Information
Aroma Reddy Lega
legaaroma@gmail.com
