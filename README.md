# data_analysis_labs

This project holds a series of Jupyter notebooks containing labs from a Data Analysis class that provides an introduction to regression and applied statistics for the social sciences, with a strong emphasis on using Python to perform the key tasks in the data analysis workflow.

## Lab Descriptions

### Lab 1

#### About  
Played around with the FiveThirtyEight “drinks” dataset to see how much alcohol different countries consume each year. Tagged the heavy drinkers and compared their beer habits with everyone else using tables and charts.

#### New Statistical Techniques Involved  
- `.describe()` – means, standard deviation, percentiles  
- `.groupby()` + `.mean()` + `.std()` – compare beer servings between heavy and non-heavy drinkers  
- `pd.crosstab()` – joint distribution of heavy drinking and high beer consumption  

---

### Lab 2

#### About  
Grabbed the Quality of Government dataset and explored how civil conflict levels relate to countries’ HDI scores. Created conflict and HDI categories, ran a Pearson correlation on a scaled conflict index, and listed high-conflict, high-HDI nations.

#### New Statistical Techniques Involved  
- `np.select()` – categorize conflict and HDI levels  
- `.corr()` – Pearson correlation between scaled conflict index and HDI  

---

### Lab 3

#### About  
Pulled the Quality of Government dataset and ran regressions to see how social capital (trust) relates to democratic performance, then added freedom of expression to see if it explained more. Finally, ranked countries by trust and free-speech scores to spot the biggest mismatches.

#### New Statistical Techniques Involved  
- `smf.ols()` – simple and multiple linear regression  
- `.rank()` – turn trust and freedom scores into ranks  
- `.sort_values()` – select the top 5 countries with the largest rank differences  

---

### Lab 4

#### About  
Pulled the World Values Survey data and ran a quick OLS regression to check if people who think men make better political leaders tend to be more religious, then fitted a first-differenced panel model to see if that relationship holds over time.

#### New Statistical Techniques Involved  
- `FirstDifferenceOLS()` – first-differenced panel regression  

---

### Lab 5

#### About  
Used an F1 dataset to predict drivers’ qualifying lap times from their fastest practice laps. After merging best practice laps with qualifying results, trained a linear regression, tuned a random forest model, compared MSE and R², plotted feature importances, and predicted and ranked drivers for the upcoming meeting.

#### New Statistical Techniques Involved  
- `train_test_split()` – split data into training and test sets  
- `LinearRegression()` – fit OLS regression model  
- `GridSearchCV()` – hyperparameter tuning for `RandomForestRegressor()`  
- `RandomForestRegressor()` – ensemble regression method  
- `mean_squared_error()` + `r2_score()` – model evaluation metrics  
- `.feature_importances_` – extract and plot variable importance  
