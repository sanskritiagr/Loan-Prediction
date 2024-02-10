# Loan-Prediction
A machine learning model designed to predict whether a loan application will be approved or rejected based on the applicant's personal information and credit history. The model utilizes a dataset containing historical loan application data to train and validate its predictions. 
## Dataset: 
The dataset used for training and testing the model consists of various features that includes:
1. Personal information such as gender, marital status, dependents, education, self-employed, property area.
2. Financial information such as applicant income, coapplicant income, credit history.
3. Loan-specific details such as loan amount, loan term.
4. Target variable indicating whether the loan was approved or rejected.
## Dependencies: 
Libraries used: Numpy, Pandas, Matplotlib, missingno, seaborn, scipy, sklearn.
## Visualization:
To gain insights into the dataset before building the model, i tried to visualize the model using some plots like:</br>
Countplot(): Counting the number of observations in each categorical bin using bars. For example, after visualizing i observed that we have more males than females applying for a loan. Similarly we have more married couples than singles. </br>
Histplot(): Showing the distribution of dataset. Our data is normally distributed which is good for us. </br>
Heatmap(): Checked if our attributes are codependent on one another. If were so, we could have simply used any one of them but all our attributes are independent.</br>
Crosstab(): We observed that loan status is not dependent on gender since we have almost equal ratio for male and female.</br>
Boxplot(): We observed that we have outliers that needs to be taken care of.</br>
## Data Preprocessing
Treating NaN values: For the categorical attributes I used 'mode' to fill in the emply cells and for the numerical values, 'mean' was used.</br>
Treating Outliers: We simply dropped the values which were not in the range. </br>
SMOTE(): Increasing the data for minority class.</br>
MinMaxScaler: Linearly scales them down into a fixed range. </br>
## Model Training
1. Linear Regression: Accuracy- 92.59%
2. KNN: Best Accuracy- 90.74%
3. SVC: Accuracy- 92.59%
4. Decision Tree: Best Accuracy- 92.59%
5. Random Forest: Best accuracy- 92.59%
6. Gradient Boosting: Best Accuracy- 85.19%
7. ### Finally I used MaxVoting to ensemble all the models and got final accuracy as 92.59%.
