# Titanic Disaster

In tackling the Titanic Kaggle competition, a comprehensive data preprocessing and analysis approach was adopted. 
The dataset primarily consists of passenger information from the Titanic disaster, and the goal is to predict survival outcomes based on various features.

## Data Preprocessing and Feature Handling

```sh
String Features: The dataset contained categorical string values, notably in the 'sex' and 'Embarked' columns. The 'sex' column was mapped to numerical values for better correlation and analysis. The 'Embarked' column, indicating the port of embarkation, was encoded using one-hot encoding to transform categorical data into a numerical format.
Missing Values: The dataset had missing values in several columns, including 'Age' and 'Cabin'. The missing 'Age' data was addressed through imputation, ensuring a more robust dataset for model training. Given the high proportion of missing data and low correlation with survival, the 'Cabin' data was deemed less relevant and thus excluded from further analysis.
Feature Encoding: The 'Embarked' column was encoded to reflect the three ports of embarkation - Cherbourg (C), Queenstown (Q), and Southampton (S). This was achieved through one-hot encoding, which transformed these categorical values into a format suitable for machine learning models.
```

## Stratified Shuffle Split and Model Selection
```sh
A Stratified Shuffle Split was implemented to ensure that the train and test sets represented the dataset proportionately, especially concerning key features like 'sex'. This approach mitigated the risk of data skewness and maintained uniformity in the dataset.
For the predictive model, the Random Forest classifier was chosen. This decision was based on its ability to handle diverse datasets through multiple decision trees. This method contrasts and combines information to make predictions, fitting well with the varied nature of the Titanic dataset.
Test Set Preparation and Final Steps

The stratification methodology was consistently applied to the test set to maintain a uniform distribution of key features.
A notable observation in the test set was a missing value in the 'Fare' column. This was addressed by filling the missing value with an appropriate statistical measure (mean, median, or mode) of the 'Fare' column from the training set, ensuring completeness of the dataset for the final model evaluation.
```

# Conclusion

This methodical approach to handling the Titanic dataset involved careful preprocessing, thoughtful feature engineering, and strategic model selection. The use of Stratified Shuffle Split ensured balanced representation in training and testing phases, and the choice of Random Forest allowed for a robust and versatile modeling approach. Handling missing values and encoding categorical data were key steps in preparing the dataset for effective machine learning application. The final step involved preparing the test set, ensuring it was complete and representative for accurate model evaluation.

This comprehensive process underscored the importance of meticulous data preparation and strategic model selection in predictive modeling, particularly in a complex and historically significant dataset like the Titanic disaster.

# Virtual Environment
```sh
pip install --upgrade pip
python3 -m pip install virtualenv
python3 -m venv env
source env/bin/activate
source env/bin/deactivate
pip3 install -r requirements.txt
```

# Github Environment

Performed from Terminal Console
```sh
1. git init
2. git remote add origin ["copy here ssh or https"]
3. git remote -v
4. git add -A
5. git add .
6. git commit -m "insert here your commit"
7. git status
8. git push origin master
```

### Additional GitHub Commands
if you already created your repository, then:
```sh
1. git remote add origin ["copy here ssh or https"] 
2. same procedure applied above
3. Note: if you already got your ReadMe.md & License.md then,
firstly request your git pull origin master. THIS IS ALWAYS A RECOMMENDED PRACTICE.
4. git push origin master
```
