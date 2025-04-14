# Titanic_EDA_Task5
A Data Analysis project exploring the Titanic dataset using pandas, matplotlib, seaborn to identify trends, correlations, and survival factors.  
🛳 Titanic EDA (Exploratory Data Analysis) Project

## 📄 Overview  
This project performs exploratory data analysis (EDA) on the Titanic dataset to understand survival patterns among passengers based on features like age, gender, ticket class, fare, family size, and titles.


## 📂 Files Used  
- `cleaned_train.csv`: Cleaned Titanic dataset used for analysis.


##  Technologies & Libraries  
- **Python**  
- **Pandas**  
- **Seaborn**  
- **Matplotlib**


## 🔍 Steps in the Analysis

1. **Import Libraries**  
   - `pandas`, `matplotlib.pyplot`, `seaborn`  

2. **Load Dataset**  
   - Dataset loaded using `pd.read_csv("cleaned_train.csv")`

3. **Initial Data Exploration**
   - Checked data types with `.info()`
   - Viewed basic stats with `.describe()`
   - Checked for missing values (none found)

4. **Categorical Features Count**  
   - Analyzed value counts for: `Sex`, `Embarked`, `Pclass`, and `Title`

5. **Univariate Analysis**
   - Plotted **histograms** for Age
   - Used **boxplots** for Fare across Pclass

6. **Bivariate/Multivariate Analysis**
   - Created **correlation heatmap** of numeric features
   - **Pairplots** by survival status
   - **Countplots** showing survival by `Sex`, `Pclass`, and `Embarked`

7. **Fancy Visuals**
   - Pie chart showing gender distribution


## Key Insights from the Data

- **Gender & Survival:**  
  - Females had a significantly higher survival rate  
  - Supports "women and children first" protocol  

- **Passenger Class (Pclass):**  
  - 1st class had highest survival; 3rd class the lowest  

- **Embarkation Port:**  
  - Passengers from Cherbourg (C) survived more than others  

- **Age Distribution:**  
  - Majority of passengers were 20–40 years old  
  - Children under 10 had better survival rates  

- **Fare Insight:**  
  - Higher fare = better accommodation and higher survival chances  

- **Family Features (SibSp, Parch):**  
  - Passengers with 1–2 family members had better chances  
  - Alone or too many dependents reduced survival  

- **Title Feature (Mr, Miss, Mrs, etc.):**  
  - `Miss` and `Mrs` had higher survival rates  
  - `Mr` had the lowest

- **Correlation Summary:**  
  - Survival was positively correlated with:
    - **Fare**
    - **Sex** (when encoded)
    - **Pclass** (inversely)
  - Minor positive effect from **SibSp** and **Parch**


##  Conclusion  
The Titanic dataset reveals strong survival patterns based on social status, gender, and ticket fare. EDA helped uncover important relationships that would assist in building predictive models.
