# Housing Price Prediction for Residential Properties in the DC area

# Introduction
Currently living in the DC area and passionate about real estate and construction, I want to analyze and understand the different criteria that define the selling price for both  residential and condo properties.
The real estate market is every growing with properties more and more expensive.
The goal of this study is to identify the parameters that influence the selling price and map the area in DC with the most expensive houses/condos.

# Unit of Analysis
My unit of analysis is housing in Washington DC at a city level and the unit type (houses or condos).

# Hypothesis / Research Question(s)
- What are the attributes that affect the selling prices in DC downtown for both houses and condos?
- Are structural characteristics playing a role in the selling price?
- Compare the rising in price between houses and condos?
- Is there any pattern/reason as to why the housing selling prices are rising over the years? Is the COVID-19 increased the prices faster than before?
- Where are the areas in DC with the highest selling prices?

# Dataset
- The first dataset contains attribution on housing and structural characteristics for residential properties.
Computer Assisted Mass Appraisal (CAMA) database. 
- The dataset contains attribution on housing characteristics for residential properties, and was created as part of the DC Geographic Information System (DC GIS) for the D.C. Office of the Chief Technology Officer (OCTO) and participating D.C. government agencies.
- Number of rows: 108,197 
- Number of columns: 39
- Examples of attributes: #bathroom, #bedrooms, #kitchens, GBA (Gross building area), saledate, heat type, stories,external walls type, internal walls type,roof type, structure type 
- Web link: https://opendata.dc.gov/datasets/DCGIS::computer-assisted-mass-appraisal-residential/about
- The second dataset is the same as the first one but for condos
- Number of rows: 58,655
- Number of columns: 39
- Web link: https://opendata.dc.gov/datasets/computer-assisted-mass-appraisal-condominium/explore
- The third dataset is the adress residential units
- Number of rows: 272,531
- Number of columns: 8
- Web link: https://opendata.dc.gov/datasets/address-residential-units/explore

# Exploratory Data Analysis (EDA)

## General Statistics

![image](https://user-images.githubusercontent.com/70168968/155884650-797530ef-e449-46ce-9910-c463f3039872.png)

- Max selling price:
         $25,100,000
- Average selling price:
         $450,000
- Average bathrooms: 2
- Average bedrooms: 3
- Average stories: 2
- Average GBA: 1742 sqft

## Sales Frequency
### Year
![image](https://user-images.githubusercontent.com/70168968/155884737-69bcf267-6ac4-40c1-9bbc-5297c1438368.png)

- 2021,2020 and 2019 are the top years: More houses sold during the COVID-19
### Month
![image](https://user-images.githubusercontent.com/70168968/155884759-49ea4dc5-ba1d-4183-990e-91204c97f88f.png)

- More houses sold in January, July and June

## Variables Frequency 
### 1.Heat type
![image](https://user-images.githubusercontent.com/70168968/155884833-653eb12f-af4e-4519-82f3-969be6595162.png)
### 2. House structure
![image](https://user-images.githubusercontent.com/70168968/155884851-97618645-afc7-41f6-afcc-8516c4a64a27.png)





- Handling missing value
- Columns renaming
- Statistical analysis
- Correlation matrix

# ML Techniques
- Split dataset
- Categorical data encoding
- Feature engineering
- Feature importance
- Feature selection with Random forest
- Training the models for continuous values: linear regression (Ridge, Lasso & Elastic Net), decision tree, random forest
- Accuracy methods (precision, recall, F1)
- Predict the housing prices on test dataset
- Visualization of the results
- Map of DC with prices

# Conclusion and lessons learned
