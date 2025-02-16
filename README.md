# Housing Price Prediction for Residential Properties in the DC area

# Introduction
Currently living in the DC area and passionate about real estate and construction, I want to analyze and understand the different criteria that define the selling price for residential properties.
The real estate market is every growing with properties more and more expensive.
The goal of this study is to identify the parameters that influence the selling price and map the area in DC with the most expensive houses.

# Unit of Analysis
My unit of analysis is housing in Washington DC at a city level and the unit type (houses).

# Hypothesis / Research Question(s)
- What are the attributes that affect the selling prices in DC downtown for houses?
- Are structural characteristics playing a role in the selling price?
- How fast did the prices and the number of houses sold increased over the last two years?
- How well can this dataset predict houses price?

# Dataset
- The first dataset contains attribution on housing and structural characteristics for residential properties.
Computer Assisted Mass Appraisal (CAMA) database. 
- The dataset contains attribution on housing characteristics for residential properties, and was created as part of the DC Geographic Information System (DC GIS) for the D.C. Office of the Chief Technology Officer (OCTO) and participating D.C. government agencies.
- Number of rows: 108,197 
- Number of columns: 39
- Examples of attributes: #bathroom, #bedrooms, #kitchens, GBA (Gross building area), saledate, heat type, stories,external walls type, internal walls type,roof type, structure type 
- Web link: https://opendata.dc.gov/datasets/DCGIS::computer-assisted-mass-appraisal-residential/about
- The second dataset is the adress residential units
- Number of rows: 272,531
- Number of columns: 8
- Web link: https://opendata.dc.gov/datasets/address-residential-units/explore

# Exploratory Data Analysis (EDA)

## EDA: General Statistics

![image](https://user-images.githubusercontent.com/70168968/155884650-797530ef-e449-46ce-9910-c463f3039872.png)

- Max selling price:
         $25,100,000
- Average selling price:
         $450,000
- Average bathrooms: 2
- Average bedrooms: 3
- Average stories: 2
- Average GBA: 1742 sqft

## EDA: Sales Frequency
### Year
![image](https://user-images.githubusercontent.com/70168968/155884737-69bcf267-6ac4-40c1-9bbc-5297c1438368.png)

- 2021 (8935),2020 (6650) and 2019 (5857)are the top years: More houses sold during the COVID-19

### Month
![image](https://user-images.githubusercontent.com/70168968/155884759-49ea4dc5-ba1d-4183-990e-91204c97f88f.png)

- More houses sold in January, July and June


### Mean Price Over Year
![image](https://user-images.githubusercontent.com/70168968/161561148-05b3c4eb-c725-4bd8-af47-ac807390e75e.png)

- 2021: $726,258  (+8,4 %) 
- 2020: $670,103 (+ 7,3 %) 
- 2019: $624,484  (+ 2%) 
- 2018: $612,418 (+ 3,8%) 
- 2017: $589,815  

In the last two years, the mean price increased by more than 7% each year. 

### COVID-19 influence
![new-salescovid](https://user-images.githubusercontent.com/70168968/156957806-9090630a-204e-45ac-b671-fa55d4ed8ad1.png)

- 2014-2015: +8,2%
- 2015-2016: +12%
- 2016-2017: +15,7%
- 2017-2018: +7,9%
- 2018-2019: +7,4%
- 2019-2020: +13,5%
- 2020-2021: +34,4%

In 2021, the number of houses sold increased by 34,4% as compared to 2020. The COVID-19 may be a valid explanation.

## EDA: Variables Frequency 
### 1.Heat type
![image](https://user-images.githubusercontent.com/70168968/161833010-bb608235-ccc6-4f7d-a144-3ad84d2c39a6.png)
The three most common heat type are:
- Hot Water Rad (36.8%)
- Forced Air (35.8%)
- Warm Cool (25%)
### 2. House structure
![image](https://user-images.githubusercontent.com/70168968/161833261-ce511270-e81b-40da-bc4a-eb7ee7fe8f53.png)
The three most common house structures are:
- Row houses (50.6%)
- Single houses (29.4%)
- Semi-detached houses (15%)
### 3. Exterior Walls
![image](https://user-images.githubusercontent.com/70168968/161833426-71cd337f-554b-4fd3-94f8-22736be094de.png)

The five common exterior walls are: 92056
- Common brick (75%)
- Brick/Siding (5.7%)
- Vinyl Siding (5.4%)
- Wood Siding (4.1%)
- Stucco (2.9%)
### 4. Interior walls
![image](https://user-images.githubusercontent.com/70168968/161833535-8ffacbe6-3fc9-49e1-92a0-6e1e960029cd.png)

The four common interior walls are:
- Hardwood (78.3%)
- Hardwood/carp (10.9%)
- Wood floor (7.1%)
- Carpet (3.3%)
### 5.Roof type
![image](https://user-images.githubusercontent.com/70168968/161833666-9881b85b-71dd-4904-a41d-f5906e4ea798.png)

The four most common roof types are:

- Built up (29.7%)
- Comp Shingle (28.7%)
- Metal-sms (27.7%)
- Slate (10.1%)
### 6. Number of bathrooms
![image](https://user-images.githubusercontent.com/70168968/161833845-98bfb824-c941-46cc-8c0e-96adc48509fd.png)
Most of the houses have:

- 2 bathrooms (35.8%)
- 1 bathroom (30.6%)
- 3 bathrooms (22.4%)
- 4 bathrooms (8.8%)
### 7. Number of rooms
![image](https://user-images.githubusercontent.com/70168968/161834032-debe75a1-5c3d-4d03-96a1-7f01230168be.png)

The most common rooms numbers are:

- 6 rooms (31.4%)
- 7 rooms (20.2%)
- 8 rooms (15.9%)
- 5 rooms (8.1%)
- 9 rooms (7.3%)
- 10 rooms (6%)
- 12 rooms (2.9%)
- 11 rooms (2.3%)
- 16 rooms (1.3%)
### 8. Number of bedrooms
![image](https://user-images.githubusercontent.com/70168968/161834575-728b0aa2-de94-466b-9656-e3f3f8ddb198.png)
The most common rooms numbers are:

- 3 bedrooms (48.3%)
- 4 bedrooms (25%)
- 2 bedrooms (13.5%)
- 5 bedrooms (7.6%)
- 6 bedrooms (3.3%)

### 9. Number of stories
![image](https://user-images.githubusercontent.com/70168968/161834693-d0c569fe-fc9f-407b-a449-2708375ccd32.png)

The most common stories numbers are:

- 2 stories (73.9%)
- 3 stories (9.4%)
- 2.5 stories (5.9%)
- 1 story (4.1%)
- 1.5 stories (2%)
## EDA: Correlation Matrix
![heatmap](https://user-images.githubusercontent.com/70168968/155885744-f9da5649-bed1-473e-890d-01fc80e2b46d.png)

The variables that are more correlated to the price are:
- Gross Building Area (GBA) (0.41)
- Number of bathrooms (0.42)
- Number of bedrooms (0.27)
- Number of rooms (0.24)
- Roof type (0.14)

## EDA: Scatterplot Matrix
![image](https://user-images.githubusercontent.com/70168968/161561462-2bc8ed86-e728-4a78-8109-e94db93018b1.png)

![image](https://user-images.githubusercontent.com/70168968/161836058-2aa49316-d936-4bbd-8397-5620829ef0c5.png)


GBA, BATHRM and ROOMS have a linear correlation with the price.
There is no linear correlation for the other house characteritics.


# Part 2:  Machine learning evaluation

In this second part, we will now evaluate the dataset and see how well it predicts house prices.
The goal is to predict a price, which is a continuous value: it's a regression problem.
## II.a Split dataset

We will split the dataset with the 80/20: 80% for the the training data and 20% for the test data.
We will have 10 features and 1 target, the price
## II.b Feature importance with Random forest
First, let's measure the feature importance by using the Random Forest ensemble technique
![image](https://user-images.githubusercontent.com/70168968/161578115-ecffdc61-1df2-466a-aa62-7d4f78ac9ff0.png)

- The Gross Building Area (GBA) is the most important feature (37%)
- The number of rooms (13%)
- The roof type (8,6%)
- Structure type (8,2%)
- External wall type (7,2%)

## II.c Machine Learning Techniques

For all the techniques, our two metrics will be the following:

- **R-squared or Coefficient of Determination (R2)**: This metric represents the part of the variance of the dependent variable explained by the independent variables of the model. It measures the strength of the relationship between your model and the dependent variable
- **Mean Absolute Error (MAE)**: This metric evaluates the mean of the absolute values of each prediction error on all instances of the test data-set. Prediction error is the difference between the actual value and the predicted value for that instance.

### II.c.1 Linear Regression model: Ordinal Least Square (OLS)

Our first ML technique is Linear Regression with OLS. Ordinary least squares (OLS) regression is a statistical method of analysis that estimates the relationship between one or more independent variables and a dependent variable; the method estimates the relationship by minimizing the sum of the squares in the difference between the observed and predicted values of the dependent variable configured as a straight line
![image](https://user-images.githubusercontent.com/70168968/161627216-410ee6af-c8b6-4539-9aa6-4adc7ce7e3ae.png)

![image](https://user-images.githubusercontent.com/70168968/161627256-e2ce8375-4ed2-43d1-b1e6-81208da4c50f.png)



R2= 0.288
MAE= 596.87

**Conclusion**: We can see that this model does not perform very well on our dataset, which makes sense since not all the features are linearly correlated to the price.
The R2 error is around 0.29 and the MAE error is 600. The model is not performing very well


### II.c.2 Other Linear Regression models

**Ridge**: Ridge regression is a method of estimating the coefficients of multiple-regression models in scenarios where linearly independent variables are highly correlated

**Lasso**: Lasso regression is a type of linear regression that uses shrinkage. Shrinkage is where data values are shrunk towards a central point, like the mean. The lasso procedure encourages simple, sparse models (i.e. models with fewer parameters)

**Bayesian**: Bayesian regression is an approach to linear regression in which the statistical analysis is undertaken within the context of Bayesian inference. When the regression model has errors that have a normal distribution, and if a particular form of prior distribution is assumed, explicit results are available for the posterior probability distributions of the model's parameters

**ElasticNet**: Elastic Net is a regularized regression method that linearly combines the L1 and L2 penalties of the lasso and ridge methods

![image](https://user-images.githubusercontent.com/70168968/161816836-7efdb640-9ac2-4b27-9c4d-f0cd3b7cb4a0.png)


**Conclusion**: the other linear regression models perform  less well than OLS regression

### II.c.3 Decision Tree

The goal of using a Decision Tree is to create a training model that can use to predict the class or value of the target variable by learning simple decision rules inferred from prior data(training data)
![image](https://user-images.githubusercontent.com/70168968/161627381-410de1e3-8e3a-4b61-8c8f-0c976bb6170d.png)
![image](https://user-images.githubusercontent.com/70168968/161627411-95931674-9d2f-433b-9c27-6ec0a2bd79d4.png)

R2= 0.209
MAE= 601.93


**Conclusion**: The decision tree model performs less well than the OLS regression. 


### II.c.4 Random Forest

Random Forest is a “Tree”-based algorithm that uses the qualities features of multiple Decision Trees for making decisions

![image](https://user-images.githubusercontent.com/70168968/161627570-2296aa5a-a430-4f35-8eb0-7cc43895a7bb.png)

![image](https://user-images.githubusercontent.com/70168968/161627599-a9df3eec-738b-45b5-b001-d20ee9b0f0f7.png)

R2: 0.265
MAE: 603.47 
**Conclusion**: The model performs better than the decision tree but not as well as the OLS method

## II.d Advanced Machine Learning Techniques
Given our results, we can use advanced machine learning techniques to improve the performance

### II.d.1 K-fold cross-validation

In k-fold cross-validation, we randomly split the training dataset into k folds without replacement, where k-1 folds are used for the model training, and one fold is used for performance evaluation. This procedure is repeated k times so that we obtain k models and performances.

The test dataset is used to calculate the accuracy score of the model, which is collected in the scores list to calculate the average accuracy and the standard deviation of the estimate.
![image](https://user-images.githubusercontent.com/70168968/161803319-eff6b394-7db6-4567-9057-54552d4842d2.png)

### II.d.2 Tuning hyperparameters via grid search

The grid search approach is a brute-force exhaustive search paradigm where we specify a list of values for different hyperparameters, and the computer evaluates the model performance for each combination to obtain the optimal combination of values from this set
![image](https://user-images.githubusercontent.com/70168968/161803497-1c447ad8-64ff-4a77-afa8-93f44181ffcc.png)


### II.d.3 Ensemble methods: bagging and boosting

The goal of ensemble methods is to combine different classifiers into a meta-classifier that has better generalization performance than each individual classifier alone

- In bagging, the objective is to create several subsets of data from training sample chosen randomly with replacement. Each collection of subset data is used to train their decision trees. As a result, we get an ensemble of different models. Average of all the predictions from different trees are used which is more robust than a single decision tree classifier

- In boosting, the ensemble consists of very simple base classifiers, also referred to as weak learners. The key concept behind boosting is to focus on training examples that are hard to classify, that is, to let the weak learners subsquently learn from missclassified training examples to improve the performance of the ensemble
![image](https://user-images.githubusercontent.com/70168968/161803730-2bf4deef-9a7e-4db9-b59f-d03dfa5d7570.png)

### II.d.4 Random Forest Classifier
- Best parameters:
Max_depth=1
N_estimators= 50

- The model did not work well on my dataset.

![image](https://user-images.githubusercontent.com/70168968/161812634-b7df68fa-574d-4bbf-a2b5-0158b82c4b6e.png)

![image](https://user-images.githubusercontent.com/70168968/161812682-449a2b86-539a-4e74-9168-271ce576dbb8.png)

### II.d.5Gradient Boosting

- Best parameters according to Grid Search:
Learning_rate: 0.01
Max_depth: 5
N_estimators: 250

![image](https://user-images.githubusercontent.com/70168968/161806804-51ddbf8a-93a0-45d6-9750-8a6f5a8c5121.png)

R2: 0.679
MAE: 573.81

Learning curve

![image](https://user-images.githubusercontent.com/70168968/161806965-215eefc3-1e10-4260-91d3-2e6313ac4c52.png)

**Conclusion**: The model is overfitting (high bias). It performs better on training data than on test data.

## Summary and Conclusion

![image](https://user-images.githubusercontent.com/70168968/162045024-c75c054b-dbbf-4e4e-82cb-7aee82cc3dbd.png)
The application of advanced machine learning improved the performance by more than 100% for the R2.

The model can be further improved by adding more hyperparameters and and by addressing overfitting issue.

Research questions answers:

- What are the attributes that affect the selling prices in DC downtown for houses? The top 5 attributes are
The Gross Building Area (GBA)  (37%)
The number of rooms (13%)
The roof type (8,6%)
Structure type (8,2%)
External wall type (7,2%)


- Are structural characteristics playing a role in the selling price? The top 3 structural characteristics are the roof type, the structure type and the external wall type

- How fast did the prices and the number of houses sold increased over the last two years? 2019-2020: + 13,5% 
2020-2021: + 34,4% 
2021: $726,258  (+8,4 %) 
2020: $670,103 (+ 7,3 %) 
2019: $624,484  (+ 2%) 
The number of houses sold tripled in 2021 as compared to 2020 and the average price as well



- How well can this dataset predict houses price? With normal ML model R2 <0.30
With Advanced model, R2>0.65

# References

Python Machine Learning: Perform Python Machine Learning and Deep Learning with Python,
scikit-learn, and TensorFlow, 3rd Edition by Sebastian Raschka and Vahid Mirjalili (2019).

Medium article: House Price Prediction With Machine Learning in Python (https://medium.com/codex/house-price-prediction-with-machine-learning-in-python-cf9df744f7ff)

Toward Data Science Article: Predicting House Prices with Machine Learning (https://towardsdatascience.com/predicting-house-prices-with-machine-learning-62d5bcd0d68f)

Youtube video: House Price Prediction using Machine Learning (https://www.youtube.com/watch?v=ta3Wd6Q5Byc)


