# COVID-19-Socio_Economic_Analysis Project
Analysis by Machine Learning

 # Introduction:
The UN’s Framework for the Immediate Socio-Economic Response to the COVID 19 Crisis warns that “The COVID-19 pandemic is far more than a health crisis: it is affecting societies and economies at their core. While the impact of the pandemic will vary from county to county, it will most likely increase poverty and inequalities at a state to country scale.

In this Jupyter Notebook, we will use a dataset which has been constructed from data about Median Household Income, Poverty, Unemployment and COVID cases and deaths in USA at state and county level from 6 datasets from census.gov and usda.gov. This analysis will perform machine learning analysis.

 # Libraries:

Matplolib has been used for visualizations and SKLearn multiple liberaries have been used for machine learning models.

 # Analysis:

Feature Importance: Random forest consists of a number of decision trees. Every node in the decision trees is a condition on a single feature, designed to split the dataset into two so that similar response values end up in the same set. The measure based on which the (locally) optimal condition is chosen is called impurity. When training a tree, it can be computed by how much each feature decreases the weighted impurity in a tree. For a forest, the impurity decrease from each feature that can be averaged and the features that are ranked according to this measure.

PCA: Principal component analysis (PCA) is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components. This transformation is defined in such a way that the first principal component has the largest possible variance (that is, accounts for as much of the variability in the data as possible), and each succeeding component in turn has the highest variance possible under the constraint that it is orthogonal to the preceding components.

We can use PCA to reduce the number of features to use in our ML algorithms, and graphing the variance gives us an idea of how many features we really need to represent our dataset fully.

Splitting Data into Training and Testing Datasets: We need to split the data back into the training and testing datasets.

Removing Samples with Missing data: We could have removed rows with missing data during feature cleaning, but we're choosing to do it at this point. It's easier to do it this way, right after we split the data into Training and Testing. Otherwise we would have had to keep track of the number of deleted rows in our data and take that into account when deciding on a splitting boundary for our joined data.

 The following algorithms are used:

KNN: Logistic Regression: Random Forest: Naive Bayes: Decision Tree:

The Accuracy score of Logistic Regression is 77.09 which predicts that COVID-19 impacts states and counties at a socio-economic level.

The Accuracy score of the Naive Bayes Classifier is 98.4. The model behind Naive Bayes Classifier has something to do with probability distributions. The aim is to maximize the probability of the target class given the x features. As such, based on our data and analysis, the accuracy score predicts that there is a high chance that COVID-19 impacts the states and counties at a socio-economic level.

The Accuracy score of KNN is 79.47.  The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other. Our KNN implementation above relies on structured data. It needs to be in a table format. Additionally, the implementation assumes that all columns contain numerical data and that the last column of our data has labels that we can perform some function on. So, the KNN accuracy score of 79.47 here predicts that the our data and variables are related. To better explain this, socio-economic factors in our communities are impacted by COVID-19.

The Accuracy score of Decision Tree is 100. Decision Tree algorithms predicts to make decision making easier. A higher accuracy score means that the model is taking into account all variables and predicts a strong relationship between variables.

The Accuracy score of Randon Forest classifier is 99.15.  Random forests is considered as a highly accurate and robust method because of the number of decision trees participating in the process. Because the accuracy score is high, our data analysis model implies that variables are related and can be highly impacted by each other.

The combination of the COVID-19 pandemic, a drop in unemployment, increasing number of cases and deaths have the potential to seriously impact stability state and county wide, and will strain public health and social security systems in the short to medium terms. This analysis uses machine learning models' accuracy scores to predict relationship betwen covid-19 cases/deaths and several socio-economic factors like poverty, household income, unemployment, education and race. The high accuracy scores of each model indicate that there is a strong relationship and all dependent variables can be highly impacted by changes in independent variables, such as covid-19 cases/deaths.

  # Author:
  Shahid Mumtaz
